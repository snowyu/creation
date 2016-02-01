# 汇聚创新 [![加入我们的聊天室 https://gitter.im/teamhost/creation](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/teamhost/creation?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

我们在这里讨论各种创新的主意、产品、服务甚至开发和架构以及对他们的分析，无论是什么，只要他们和创新相关都可以在这里讨论。

非常欢迎贡献你的主意，你所发现的和创新相关的东西。在贡献之前请先阅读下 [CONTRIBUTING.md][contributing] 文件。


* Services(服务)
  * [Slack](service/slack.cn.md) - 分析[slack][slack]的创新点和它的竟品们，新鲜出笼，生态圈尚在发展之中
  * [Github]() - 这虽然不是新东西，但它代表一个转折点，如今围绕它的生态圈已经完善，竟品丰富，已经存在完全开源的方案
  * [travis](https://travis-ci.org) - 线上集成测试服务，不用多说，一直在用, push到github后， travis会自动运行CI
    * [![Build Status](https://img.shields.io/travis/snowyu/property-manager.js/master.svg)](http://travis-ci.org/snowyu/property-manager.js)
  * [Code Climate](service/codeclimate.md) - 代码质量和代码覆盖率显示服务.
    * [Code Climate Web Site][codeclimate]
    * 和 travis 类似，支持badge图标:
    * 代码质量评分(总4分): [![Code Climate](https://codeclimate.com/github/snowyu/property-manager.js/badges/gpa.svg)](https://codeclimate.com/github/snowyu/property-manager.js)
    * 测试覆盖率:[![Test Coverage](https://codeclimate.com/github/snowyu/property-manager.js/badges/coverage.svg)](https://codeclimate.com/github/snowyu/property-manager.js/coverage)
    * 在这个项目中刚用上的，效果还不错: https://github.com/snowyu/property-manager.js
    * 类似产品
      * [Coveralls](https://coveralls.io/) 仅支持测试代码覆盖率显示服务(以前用过一次，现在似乎出问题了，上传测试报告后显示无数据，换用Code Climate)
* WYSIWYG Form Builder: 所见即所得的表单生成服务,不知道多少提供OpenAPI的
    可以用于调查，邀请函(比如slack的邀请: http://nodeslackers.io/)，甚至工资单
    我感觉的趋势是UI也在被服务化，成为一种服务。
    * TypeForm: 设计核心是简化虚拟线上投票环节，让创建投票和传播变得更为简便。
    * Formstack
    * JotForm
    * SurveyMonkey
    * [screendoor](http://www.dobt.co/screendoor/): Smarter online forms
  * [bip.io - Web Automation For People and Robots](https://bip.io/):Open Source, Rapidly create workflows with the cloud components you love, no programming required.
  * [IFTTT](https://ifttt.com/)
  * [OpenBazaar](https://openbazaar.org/): OpenBazaar is an open source project to create a decentralized network for commerce online, using Bitcoin, that has no fees and cannot be censored.
  * [Gratipay - Gittip](https://gratipay.com): [Open Company][OpenCompany], 按周支付给信任的个体或团队. 培养感恩，慷慨和爱心的经济。
    * 只支持周期付款，不支持单次支付，（可以在网上开工资了）
    * http://inside.gratipay.com/: 如何运作gittip
    * [An Open Source Grant with a Difference](https://blog.engineyard.com/2014/gittip-open-source-grant)
    * 简单的团队成员付工具(利用Gittip API): https://github.com/engineyard/gittip-collab
    * 实际客户方:
      1. 利用外包人员降低成本的公司
      1. 跨国跨地区的新型创业公司
      1. 各类基金会和慈善组织
* [开源硬件](https://en.wikipedia.org/wiki/Open-source_hardware)
  * 积木块
    * MakeBlock - http://www.makeblock.cc/
  * 主板
    * Arduino - https://www.arduino.cc/ - 传感控制器
      * Microduino - https://www.microduino.cc/
      * Netduino - http://www.netduino.com/netduino - an open-source electronics platform using the .NET Micro Framework.
    * Raspberry Pi - https://www.raspberrypi.org/ - 高清机顶盒
      * CubieBoard - http://cubieboard.org/
    * [NL6621 ARM Wifi Soc](http://www.nufrontsoft.com/index.php/project/index/id/16.html)
      * 160 MHz ARM Cortex-M3 with 448 KB of RAM. The module has 32 GPIOs, SPI, I2C, I2S digital audio.
      * 802.11 b/g/n/p/e
      * https://github.com/NufrontIOT/NL6621_StandardSDK
      * https://www.gitbook.com/@nufrontiot
    * [ESP 8266 Wifi SoC](https://anxinke.taobao.com/)
      * http://bbs.ai-thinker.com/
      * [NodeMCU](http://www.nodemcu.com/): An open-source firmware and development kit that helps you to prototype your IOT product within a few Lua script lines
        * NodeMCU 0.9 ESP-12 Module
        * NodeMCU 1.0 ESP-12E Module
      * [Arduino UNO R3 ESP8266 WiFi shiled(ESP-12E)](https://item.taobao.com/item.htm?id=521217451908)
      * ESP8266选型特点：
        1. ESP-01：PCB天线，经过匹配，距离做到空旷400米左右，简单易用
        2. ESP-02：贴片封装，适合提交限制，天线可以用IPX头引出壳体。
        3. ESP-03：贴片封装，内置陶瓷天线工艺，所有可用IO引出。
        4. ESP-04：贴片封装，客户可自定义天线类型，灵活设计，所有可IO引出。
        5. ESP-05：贴片封装，只引出串口和RST脚，体积小，天线可外置。
        6. ESP-06：底贴工艺，所有IO口引出，带金属屏蔽壳，可过FCC  CE认证，推荐使用。
        7. ESP-07：半孔贴片工艺，所有IO引出，带金属屏蔽壳，可过FCC  CE认证，可外接IPX天线，也可用内置陶瓷天线。
        8. ESP-08：同ESP-07，不同在于天线形式客户可自己定义。
        9. ESP-09：超小体积封装，只有10*10毫米，四层板工艺!1M字节。
        10. ESP-10：贴片接口，窄体设计，10毫米宽，适合做灯带控制器。
        11. ESP-11：贴片接口，陶瓷天线，小体积。
        12. ESP-12：半孔贴片工艺,全IO引出，带金属屏蔽壳，已过FCC &CE认证，内置PCB板载天线，4M字节Flash。
        13. ESP-12E:在ESP-12的基础上多引出6个脚，抗干扰能力大大增强，
        14. ESP-12F：突破性的设计，又有新突破。全新四层板设计，天线全新改版 射频性能优化，相较于ESP-12E的通讯距离增加30%-50%！半孔贴片工艺,全IO引出，带金属屏蔽壳，已过FCC &CE&RoHS认证，内置PCB板载天线，4M字节Flash。
        14. ESP-13: 全新4层板设计，半孔贴片工艺,全IO引出，带金属屏蔽壳，天线重新设计，射频性能更好！
        15. ESP14: 以ESP-12E为设计原型，内部增加了STM8S003F3P6，并通过STM8S对ESP8266进行AT指令控制.该模块就是一个完整的STM8S的单片机，可以通过STM8单片机编程进行WIFI操作。
    * WRTnode - http://wrtnode.com/ - 无线路由器
      * Vocore - http://vocore.io/
    * HackRF - https://github.com/mossmann/hackrf - 软件定义无线电 Software defined Radio(SDR)
      * GSM
      * Bluetooth
      * Wifi
    * OpenPilot - https://www.openpilot.org/ - 飞行控制器(电脑自驾) Flight-controller
      * CC3D - OpenPilot推出的低端控制器，价格便宜，秒杀大疆
        * 飛行模式
          * Attitude：遙控放桿後自動水平自穩
          * Rate：飛機保持目前角度 加油門可暴力飛行
          * AxisLock：飛機保持目前角度 如飛控偵測向左偏移五度則會向右偏移五度角修正
          * WeakLeveling：同RATE 但緩慢自穩水平
          * Horizon：同MWC的Horizon模式
      * ArduPilot - http://ardupilot.com/
      * Blog - http://www.rchacker.com/
      * KK2 - https://code.google.com/p/nextcopterplus/wiki/OpenAero2_Getting_Started
      * MultiWii(MWC) - http://www.multiwii.com/
        * NanoWii - http://www.nanowii.com/
  * Robot
    * Simplebot - https://github.com/nodebotsau/simplebot
  * Software
    * IoT Platform
      * AllSeen -https://allseenalliance.org/ - 为了解决困扰物联网领域的协作性问题（不同领域和品牌的设备不能互相识别和协作）。高通创新中心推动的。主要成员：微软，LG，海尔，松下，夏普，索尼，思科，D-Link，TP-LINK，HTC，乐视TV等。AllSeen聯盟最終希望打造一個開放的軟體架構，可以讓家中的電視、機上盒、路由器、智慧照明系統和其他設備無縫地連接起來，並跨越iOS、Android、Windows 或 Mac 等不同的作業系統。
      * OpenInterconnect - http://openinterconnect.org/ - 开放互联联盟，以开放性和参与性为侧重点，来自思科系统公司 (Cisco Systems Inc.)、英特尔公司 (Intel Corporation)、联发科 (MediaTek) 和三星电子有限公司 (Samsung Electronics Co., Ltd.) 的行业领导者将共同确定连接需求，以提高接入物联网 (IoT) 的数十亿台设备之间的互操作性。OIC致力于定义基于工业标准技术的公共通讯框架，规范个人计算和新兴IoT设备之间的无线连接和智能管理信息流程。
      * IoT.js - http://github.com/Samsung/iotjs
        IoT.js aims to provide inter-operable service platform in the world of IoT, based on web technology
    * firmware
      * JerryScript - https://github.com/Samsung/jerryscript
        轻量级的 JavaScript 引擎可运行与内存受限设备(如微控制器)
        * (<64 KB RAM)
        * (<200 KB ROM)
      * Forth - My Favorite MicroController Language
        * FlashForth - http://flashforth.com/ - https://github.com/oh2aun/flashforth.git
        * AmForth - http://amforth.sourceforge.net/
        * avrforth - http://krue.net/avrforth/
      * Microsoft .NET Micro Framework - https://netmf.github.io/
        * at least 256 KBytes of flash and 64 KBytes of RAM. A memory footprint of about 300 KB
        * Can run directly "on the metal" without an operating system
        * Running on an OS is also possible
        * ARM architecture processors (including ARM7, ARM9 and Cortex-M architectures)
        * Analog Devices Blackfin
      * OpenWRT -
    * protocol
      * MQTT - MQTT is a publish/subscribe messaging protocol designed for lightweight M2M communications. via IBM
        * http://mqtt.org/
        * [Specification](http://www.ibm.com/developerworks/webservices/library/ws-mqtt/index.html)
        * https://github.com/adamvr/MQTT.js/
      * CoAP - Constrained Application Protocol from the CoRE (Constrained Resource Environments) IETF group.
        * http://coap.technology/
        * Like HTTP, CoAP is a document transfer protocol. Unlike HTTP, CoAP is designed for the needs of constrained devices.
        * CoAP runs over UDP
        * [IP for Smart Objects Alliance](http://www.ipso-alliance.org/)
        * [Specification](http://tools.ietf.org/html/draft-ietf-core-coap)
        * Open source implementations:
          * http://sourceforge.net/projects/libcoap/
          * https://github.com/morkai/h5.coap
          * http://www.contiki-os.org/
      * Firmata - http://www.firmata.org/wiki/Main_Page
      * CAN -
    * IDE
      * processing with Firmata
      * node-red - https://github.com/node-red/node-red
      * scratch
      * snap


* Programming(编程)
  * 异步编程，流与架构 (Asynchronous, Stream and Architecture)
    * [ReactiveX.io](http://ReactiveX.io): 流式事件，让事件的抽象复用(Observable)到达一个新的高度
      * [cycle.js](http://cycle.js.org):将人机交互抽象为两个函数(human, computer)的互动,
        这点超赞。但是将UI(DOM)变成了数据，这我就不知道是好是坏了，至少这不是其所擅长的。
    * [Gulp 4](https://github.com/gulpjs/gulp/tree/4.0) Keep It Simple and Stupid(KISS)
  * Stupid compiler and smart compiler


## License

[![CC BY 4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)][CCBY4]

本作品采用[知识共享署名 4.0 国际许可协议][CCBY4]进行许可。

[slack]: https://slack.com/
[bacon.js]: https://github.com/baconjs/bacon.js
[rxjs]: http://reactive-extensions.github.io/RxJS/
[codeclimate]:https://codeclimate.com
[contributing]: https://github.com/teamhost/creation/blob/master/CONTRIBUTING.md
[OpenCompany]: http://www.opencompany.org
[CCBY4]: https://creativecommons.org/licenses/by/4.0/
