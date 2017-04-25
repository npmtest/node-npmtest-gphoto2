# npmtest-gphoto2

#### basic test coverage for  [gphoto2 (v0.1.7)](https://github.com/lwille/node-gphoto2)  [![npm package](https://img.shields.io/npm/v/npmtest-gphoto2.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-gphoto2) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-gphoto2.svg)](https://travis-ci.org/npmtest/node-npmtest-gphoto2)

#### Node.js wrapper for libgphoto2

[![NPM](https://nodei.co/npm/gphoto2.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gphoto2)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-gphoto2/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-gphoto2/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-gphoto2/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-gphoto2/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-gphoto2/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-gphoto2/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-gphoto2/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-gphoto2/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-gphoto2/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-gphoto2/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-gphoto2/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-gphoto2/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-gphoto2/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-gphoto2/build/test-report.html](https://npmtest.github.io/node-npmtest-gphoto2/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-gphoto2/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-gphoto2/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-gphoto2/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gphoto2/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gphoto2/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gphoto2/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-gphoto2/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-gphoto2/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": "Leonhardt Wille <wille@riverlabs.de>",
    "name": "gphoto2",
    "description": "Node.js wrapper for libgphoto2",
    "version": "0.1.7",
    "homepage": "https://github.com/lwille/node-gphoto2",
    "repository": {
        "type": "git",
        "url": "git://github.com/lwille/node-gphoto2.git"
    },
    "engines": {
        "node": "~0.10.0"
    },
    "os": [
        "darwin",
        "linux"
    ],
    "main": "build/Release/gphoto2.node",
    "dependencies": {},
    "devDependencies": {
        "async": "^0.2.10",
        "coffee-script": "^1.7.1",
        "express": "^3.1.2",
        "jade": "^0.28.2",
        "mocha": "^1.9.0",
        "pre-commit": "^0.0.8",
        "should": "^1.2.2",
        "sinon": "^1.6.0",
        "superagent": "^0.14.9",
        "underscore": "^1.4.4"
    },
    "pre-commit": [
        "cpplint"
    ],
    "scripts": {
        "cpplint": "util/cpplint.sh",
        "prepublish": "npm run cpplint",
        "preinstall": "((which pkg-config && pkg-config libgphoto2) || (which dpkg && dpkg -s libgphoto2-2-dev) || (which brew && brew list libgphoto2) || (echo 'ERROR: libgphoto2 seems not to be installed.' 1>&2; exit 1)) && node-gyp rebuild",
        "test": "node_modules/mocha/bin/mocha"
    },
    "license": "MIT",
    "contributors": [
        {
            "name": "Leonhardt Wille",
            "url": "https://github.com/lwille"
        },
        {
            "name": "Aaron Israel",
            "url": "https://github.com/a0n"
        },
        {
            "name": "Luigi Pinca",
            "url": "https://github.com/lpinca"
        },
        {
            "name": "Michael Kötter",
            "url": "https://github.com/michaelkoetter"
        },
        {
            "name": "david noelte",
            "url": "https://github.com/marvin"
        },
        {
            "name": "Brian White",
            "url": "https://github.com/mscdex"
        }
    ],
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
