# npmtest-cfonts

#### basic test coverage for  [cfonts (v1.1.2)](https://github.com/dominikwilkowski/cfonts)  [![npm package](https://img.shields.io/npm/v/npmtest-cfonts.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-cfonts) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-cfonts.svg)](https://travis-ci.org/npmtest/node-npmtest-cfonts)

#### Sexy fonts for the console

[![NPM](https://nodei.co/npm/cfonts.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cfonts)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-cfonts/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-cfonts/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-cfonts/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-cfonts/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-cfonts/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-cfonts/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-cfonts/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-cfonts/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-cfonts/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-cfonts/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-cfonts/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-cfonts/build/test-report.html](https://npmtest.github.io/node-npmtest-cfonts/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-cfonts/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-cfonts/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-cfonts/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cfonts/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cfonts/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cfonts/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-cfonts/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-cfonts/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "cfonts",
    "description": "Sexy fonts for the console",
    "version": "1.1.2",
    "homepage": "https://github.com/dominikwilkowski/cfonts",
    "author": {
        "name": "Dominik Wilkowski",
        "url": "http://dominik-wilkowski.com/"
    },
    "contributors": {
        "name": "Dominik Wilkowski",
        "url": "http://dominik-wilkowski.com/"
    },
    "repository": {
        "type": "git",
        "url": "git://github.com/dominikwilkowski/cfonts.git"
    },
    "bugs": {
        "url": "https://github.com/dominikwilkowski/cfonts/issues"
    },
    "licenses": [
        {
            "type": "GNU-GPL",
            "url": "https://github.com/dominikwilkowski/cfonts/blob/master/LICENSE"
        }
    ],
    "engines": {
        "node": ">=0.12.15"
    },
    "scripts": {
        "prepublish": "npm run build",
        "test": "node ./test/fonttest.js",
        "build": "npm run build:bin & npm run build:lib",
        "build:bin": "babel src/bin.js --out-file bin/font.js --presets=es2015 --plugins transform-runtime",
        "build:lib": "babel src/lib.js --out-file index.js --presets=es2015 --plugins transform-runtime",
        "watch": "npm run build && onchange 'src/**/*' -- npm run build"
    },
    "devDependencies": {
        "babel-cli": "^6.22.2",
        "babel-plugin-transform-runtime": "^6.22.0",
        "babel-preset-es2015": "^6.22.0",
        "grunt": "~1.0.1",
        "grunt-contrib-jshint": "^1.0.0",
        "grunt-exec": "^1.0.0",
        "onchange": "^3.2.1"
    },
    "peerDependencies": {},
    "dependencies": {
        "babel-runtime": "6.22.0",
        "chalk": "1.0.0",
        "change-case": "3.0.0",
        "commander": "2.9.0",
        "window-size": "0.3.0"
    },
    "keywords": [
        "font",
        "banner",
        "logo",
        "CLI",
        "console",
        "ascii",
        "pretty"
    ],
    "files": [
        "index.js",
        "bin/*",
        "fonts/*"
    ],
    "main": "index.js",
    "bin": {
        "cfonts": "./bin/font.js"
    },
    "license": "GNU-GPLv2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
