# npmtest-weather-js

#### basic test coverage for  [weather-js (v2.0.0)](http://github.com/devfacet/weather)  [![npm package](https://img.shields.io/npm/v/npmtest-weather-js.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-weather-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-weather-js.svg)](https://travis-ci.org/npmtest/node-npmtest-weather-js)

#### A module for obtaining weather information

[![NPM](https://nodei.co/npm/weather-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/weather-js)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-weather-js/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-weather-js/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-weather-js/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-weather-js/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-weather-js/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-weather-js/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-weather-js/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-weather-js/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-weather-js/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-weather-js/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-weather-js/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-weather-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-weather-js/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-weather-js/build/test-report.html](https://npmtest.github.io/node-npmtest-weather-js/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-weather-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-weather-js/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-weather-js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-weather-js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-weather-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-weather-js/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-weather-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-weather-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "devfacet"
    },
    "bugs": {
        "url": "https://github.com/devfacet/weather/issues"
    },
    "dependencies": {
        "request": "2.x.x",
        "xml2js": "0.4.x"
    },
    "description": "A module for obtaining weather information",
    "devDependencies": {
        "chai": "3.5.x",
        "coveralls": "^2.11.16",
        "dependency-check": "2.8.x",
        "istanbul": "0.4.x",
        "jshint": "2.9.x",
        "jshint-stylish": "2.2.x",
        "mocha": "3.2.x",
        "mocha-multi": "0.10.x"
    },
    "directories": {},
    "dist": {
        "shasum": "0d9bcdb05a4f84d06b9b9f3990028a601ea4a1fc",
        "tarball": "https://registry.npmjs.org/weather-js/-/weather-js-2.0.0.tgz"
    },
    "gitHead": "7f9325f461e24ca9e902612535b2602a6294bb52",
    "homepage": "http://github.com/devfacet/weather",
    "keywords": [
        "weather",
        "forecast"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "devfacet"
        }
    ],
    "name": "weather-js",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/devfacet/weather.git"
    },
    "scripts": {
        "depcheck": "dependency-check . *.js",
        "depcheck:unused": "dependency-check ./package.json --unused --no-dev *.js",
        "lint": "jshint --reporter node_modules/jshint-stylish *.js test/*.js",
        "lint:build": "jshint --reporter checkstyle *.js test/*.js > reports/jshint-checkstyle.xml",
        "test": "npm run lint && npm run test:unit",
        "test:coveralls": "cat reports/coverage/lcov.info | node_modules/coveralls/bin/coveralls.js",
        "test:unit": "mkdir -p reports/ && NODE_ENV=test multi='spec=- xunit=reports/mocha-xunit.xml' istanbul cover _mocha -- --timeout 10000 -R mocha-multi && istanbul check-coverage"
    },
    "version": "2.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
