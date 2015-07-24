# [Travis-ci Platform](https://travis-ci.org/)

Test and Deploy with Confidence. Easily sync your GitHub projects with Travis CI and you'll be testing your code in minutes!

## Usages

### [Encryption keys](http://docs.travis-ci.com/user/encryption-keys/)

Travis CI generates a pair of private and public RSA keys which can be used to encrypt information which you will want to put into the `.travis.yml` file and still keep it private. Currently we allow encryption of environment variables, notification settings, and deploy api keys.


The easiest way to encrypt something with the public key is to use Travis CLI. This tool is written in Ruby and published as a gem. First, you need to install the gem:

```bash
gem install travis
```

Then, you can use `encrypt` command to encrypt data (This example assumes you are running the command in your project directory. If not, add `-r owner/project`):

```bash
travis encrypt SOME-DATA
```
This will output a string looking something like:

    secure: ".... encrypted data ...."

Now you can place it in the .travis.yml file.

```yaml
addons:
  code_climate:
    repo_token:
      secure: ".... encrypted data ...."
```


### [NPM Releasing](http://docs.travis-ci.com/user/deployment/npm/)

Travis CI can automatically release your npm package to npmjs.org after a successful build.

all you need to do is add the following to your .travis.yml:

```yaml
deploy:
  provider: npm
  email: "YOUR EMAIL ADDRESS"
  api_key: "YOUR API KEY"
  on:
    tags: true
```

If you tag a commit locally, remember to run `git push --tags` to ensure that your tags are uploaded to Github.
You can find your api key in `~/.npmrc`.

It is recommended to encrypt that key. Assuming you have the Travis CI command line client installed, you can do it like this:

    travis encrypt --add deploy.api_key
