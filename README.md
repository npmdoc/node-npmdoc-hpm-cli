# npmdoc-hpm-cli

#### api documentation for  [hpm-cli (v2.0.1)](https://github.com/zeit/hpm#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-hpm-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-hpm-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-hpm-cli.svg)](https://travis-ci.org/npmdoc/node-npmdoc-hpm-cli)

#### A plugin manager for Hyper.app

[![NPM](https://nodei.co/npm/hpm-cli.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/hpm-cli)

- [https://npmdoc.github.io/node-npmdoc-hpm-cli/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "hpm-cli",
    "version": "2.0.1",
    "description": "A plugin manager for Hyper.app",
    "main": "index.js",
    "scripts": {
        "test": "xo && nyc ava",
        "coverage": "nyc report --reporter=text-lcov | coveralls"
    },
    "bin": {
        "hpm": "./index.js"
    },
    "files": [
        "api.js",
        "index.js"
    ],
    "engines": {
        "node": ">=6"
    },
    "repository": "zeit/hpm",
    "keywords": [
        "hyper.app",
        "hyperapp",
        "hyperterm",
        "package",
        "manager",
        "terminal",
        "cli",
        "🦁"
    ],
    "author": {
        "name": "Matheus Fernandes",
        "url": "http://matheus.top"
    },
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/zeit/hpm/issues"
    },
    "homepage": "https://github.com/zeit/hpm#readme",
    "dependencies": {
        "args": "^2.0.0",
        "chalk": "^1.1.3",
        "columnify": "^1.5.4",
        "execa": "^0.5.0",
        "file-exists": "^2.0.0",
        "got": "^6.3.0",
        "npm-name": "^3.0.0",
        "opn": "^4.0.2",
        "ora": "^0.3.0",
        "pify": "^2.3.0",
        "recast": "^0.11.10",
        "update-notifier": "^1.0.2"
    },
    "devDependencies": {
        "ava": "^0.16.0",
        "coveralls": "^2.11.11",
        "is-ci": "^1.0.9",
        "mock-fs": "^3.11.0",
        "nyc": "^8.3.0",
        "xo": "^0.17.0"
    },
    "xo": {
        "space": 2,
        "semicolon": false,
        "esnext": true
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
