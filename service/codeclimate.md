# [The Code Climate Platform](https://docs.codeclimate.com/article/300-the-codeclimate-platform)


## Usages

### Code Style Analysis

1. From your Dashboard, mouse over the repository's name and click Settings.
2. Select the Analysis tab.
3. Click Enable Code Climate Platform.
4. Write the `.codeclimate.yml` file on the root of your repository.

    ```yml
    # For a list of all available engines, see here:
    # http://docs.codeclimate.com/article/296-engines-available-engines
    engines:
      coffeelint: # enable coffee-script analysis engine.
        enabled: true
        config: coffeelint.json
    # Engines can analyze files and report issues on them, but you can separately
    # decide which files will receive ratings based on those issues. This is
    # specified by path patterns under the ratings key.

    # For more details see here:
    # http://docs.codeclimate.com/article/289-configuring-your-repository-via-codeclimate-yml#platform
    ratings:
      paths:
        - src/**
    # You can globally exclude files from being analyzed by any engine using the
    # exclude_paths key.

    exclude_paths:
      - test/**/*
    #- spec/**/*
    #- vendor/**/*
    ```

### Test Coverage

1. Generate coverage data in [Lcov][lcov] format

    ```bash
    npm i istanbul --save-dev # generate the lcov format.
    npm i coffee-coverage --save-dev # for coffee-script.
    cat ./test/mocha.opts
      --compilers coffee:coffee-script/register
      --require coffee-coverage/register-istanbul
      --ui bdd
      --growl
      --colors
      test/**/*-test.coffee
    cat ./package.json
      ...
      "scripts": {
        "test": "grunt test",
        "test-cov": "mocha --reporter dot && istanbul report text-summary lcovonly"
      },
      ...
    ```
2. Send coverage report to codeclimate
   * Install codeclimate-test-reporter to send it locally:

    ```bash
    npm install -g codeclimate-test-reporter
    # find your CODECLIMATE_REPO_TOKEN on the Test Coverage's settings of your repository
    CODECLIMATE_REPO_TOKEN=XXXXXX codeclimate-test-reporter < ./coverage/lcov.info
    ```
   * Integrate codeclimate test to travis-ci.

     ```bash
     cat .travis.yml
      script: npm run-script test-cov
      after_success:
        - "test -e ./coverage/lcov.info && npm install codeclimate-test-reporter && codeclimate-test-reporter < ./coverage/lcov.info"
      addons:
        code_climate:
          repo_token: YOUR_CODECLIMATE_REPO_TOKEN
     ```
    It is recommended to encrypt that key. Assuming you have the Travis CI command line client installed, you can do it like this:

     ```bash
     travis encrypt YOUR_CODECLIMATE_REPO_TOKEN
     ```
    then copy-paste it to replace the value of repo_token.

### Add the badges link to your README file

 1. From your Dashboard, mouse over the repository's name and click Settings.
 1. Select the Badges tab.
 1. Copy-paste these text snippets to your README file.

[lcov]: http://ltp.sourceforge.net/coverage/lcov/geninfo.1.php
