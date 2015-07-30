# Promise

Promise是简化异步编程的重要概念。这篇文章介绍得不错：http://know.cujojs.com/tutorials/async/simplifying-async-with-promises.

简单的说，Promise（又名 Future, Delayed value, Deferred value）代表一个尚不可用的值。
因为产生这个值的计算过程尚未完成。一个 Promise 是最终的成功结果或失败原因的占位符。

* promise只有三种状态，未完成，完成(fulfilled)和失败(rejected)。
* promise的状态可以由未完成转换成完成，或者未完成转换成失败。
* promise的状态转换只发生一次
* promise有一个then方法，
  * then方法可以接受3个函数作为参数。
  * 前两个函数对应promise的两种状态fulfilled, rejected的回调函数。
  * 第三个函数用于处理进度信息。

  ```js
  .then(function(fulfilled){
          //当promise状态变成fulfilled时，调用此函数
      },function(rejected){
          //当promise状态变成rejected时，调用此函数
      },function(progress){
          //当返回进度信息时，调用此函数
      });
  ```

  ```coffee
  .then ((fulfilled)->), ((rejected)->), ((progress)->)
  ```


Promise API 标准存在多个提案，目前看啦，[Promises/A+][promisesAplus] 已经正在成为事实上的标准。

Bluebird 号称速度是所有 Promise 库里最快的 [Promises/A+][promisesAplus] 实现，里面做了许多的扩展。 想知道内部实现，也许阅读这个[yaku](https://github.com/ysmood/yaku)简单的实现（coffee-script)。



### Promise.any and Promise.some

* some是其中一些promise成功返回，可以指定个数。返回结果为一个数组.
* any是任意一个promise成功返回，是some个数固定为1的结果，另外它的返回结果是一个单值，不是数组。

注意：它们是向**所有**的promises同时发起执行请求(并行)，但是只取最先返回结果的。不是顺序执行，
直到得到成功结果的个数，就不继续了。


```coffee
Promise = require 'bluebird'

readFile = Promise.promisify (aPath, done) ->
  console.log 'readFile', aPath
  if aPath != 'c' then done(new Error('no such file')) else done(null, 'ok')

files = ['a', 'b', 'c', 'd', 'e']

Promise.any files.map (file)->readFile(file)
.then (content)-> console.log 'content=',content

```
显示结果如下:

```bash
readFile a
readFile b
readFile c
readFile d
readFile e
content= ok
```

那么如何做到顺序执行？可以用reduce实现：

```coffee
Promise.reduce files, (content, file)->
  content = readFile(file).caught(->) unless content
  return content
, null
.then (content)->console.log 'content=', content
```

显示结果如下:

```bash
readFile a
readFile b
readFile c
content= ok
```

[promisesAplus]:https://promisesaplus.com/

