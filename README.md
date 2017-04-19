# npmtest-rollup

#### basic test coverage for  [rollup (v0.41.6)](https://github.com/rollup/rollup)  [![npm package](https://img.shields.io/npm/v/npmtest-rollup.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-rollup) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-rollup.svg)](https://travis-ci.org/npmtest/node-npmtest-rollup)

#### Next-generation ES6 module bundler

[![NPM](https://nodei.co/npm/rollup.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rollup)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-rollup/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-rollup/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-rollup/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-rollup/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-rollup/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-rollup/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-rollup/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-rollup/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-rollup/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-rollup/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-rollup/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-rollup/build/test-report.html](https://npmtest.github.io/node-npmtest-rollup/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-rollup/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-rollup/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-rollup/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-rollup/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rollup/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rollup/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-rollup/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-rollup/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rich Harris"
    },
    "bin": {
        "rollup": "./bin/rollup"
    },
    "bugs": {
        "url": "https://github.com/rollup/rollup/issues"
    },
    "contributors": [
        {
            "name": "Oskar Segersvärd"
        },
        {
            "name": "Bogdan Chadkin"
        }
    ],
    "dependencies": {
        "source-map-support": "^0.4.0"
    },
    "description": "Next-generation ES6 module bundler",
    "devDependencies": {
        "acorn": "4.0.4",
        "buble": "^0.15.1",
        "chalk": "^1.1.3",
        "codecov.io": "^0.1.6",
        "console-group": "^0.3.1",
        "eslint": "^3.12.2",
        "eslint-plugin-import": "^2.2.0",
        "is-reference": "^1.0.0",
        "istanbul": "^0.4.3",
        "locate-character": "^2.0.0",
        "magic-string": "^0.15.2",
        "minimist": "^1.2.0",
        "mocha": "^3.0.0",
        "remap-istanbul": "^0.6.4",
        "require-relative": "^0.8.7",
        "rollup": "^0.39.0",
        "rollup-plugin-buble": "^0.13.0",
        "rollup-plugin-commonjs": "^7.0.0",
        "rollup-plugin-json": "^2.0.0",
        "rollup-plugin-node-resolve": "^2.0.0",
        "rollup-plugin-replace": "^1.1.0",
        "rollup-plugin-string": "^2.0.0",
        "sander": "^0.6.0",
        "source-map": "^0.5.6",
        "sourcemap-codec": "^1.3.0",
        "uglify-js": "^2.6.2"
    },
    "directories": {},
    "dist": {
        "shasum": "e0d05497877a398c104d816d2733a718a7a94e2a",
        "tarball": "https://registry.npmjs.org/rollup/-/rollup-0.41.6.tgz"
    },
    "files": [
        "dist",
        "bin/rollup",
        "README.md"
    ],
    "gitHead": "a96a923d631b9d2c471137542b9c4f578b8faa53",
    "homepage": "https://github.com/rollup/rollup",
    "jsnext:main": "dist/rollup.es.js",
    "keywords": [
        "modules",
        "bundler",
        "bundling",
        "es6",
        "optimizer"
    ],
    "license": "MIT",
    "main": "dist/rollup.js",
    "maintainers": [
        {
            "name": "eventualbuddha"
        },
        {
            "name": "rich_harris"
        },
        {
            "name": "trysound"
        },
        {
            "name": "victorystick"
        }
    ],
    "module": "dist/rollup.es.js",
    "name": "rollup",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/rollup/rollup.git"
    },
    "scripts": {
        "build": "git rev-parse HEAD > .commithash && rollup -c",
        "build:browser": "git rev-parse HEAD > .commithash && rollup -c rollup.config.browser.js",
        "build:cli": "rollup -c rollup.config.cli.js && chmod a+x bin/rollup",
        "ci": "npm run test-coverage && codecov < coverage/coverage-remapped.lcov",
        "lint": "eslint src browser test/test.js test/utils test/**/_config.js",
        "posttest-coverage": "remap-istanbul -i coverage/coverage-final.json -o coverage/coverage-remapped.json -b dist && remap-istanbul -i coverage/coverage-final.json -o coverage/coverage-remapped.lcov -t lcovonly -b dist && remap-istanbul -i coverage/coverage-final.json -o coverage/coverage-remapped -t html -b dist",
        "prepublish": "npm run lint && npm test && npm run build:browser",
        "pretest": "npm run build && npm run build:cli",
        "pretest-coverage": "npm run build",
        "test": "mocha",
        "test-coverage": "rm -rf coverage/* && istanbul cover --report json node_modules/.bin/_mocha -- -u exports -R spec test/test.js",
        "test:quick": "rollup -c && mocha",
        "watch": "rollup -c -w",
        "watch:browser": "rollup -c rollup.config.browser.js -w",
        "watch:cli": "rollup -c rollup.config.cli.js -w"
    },
    "version": "0.41.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
