# npmtest-node-telegram-bot-api

#### basic test coverage for  [node-telegram-bot-api (v0.27.0)](https://github.com/yagop/node-telegram-bot-api)  [![npm package](https://img.shields.io/npm/v/npmtest-node-telegram-bot-api.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-node-telegram-bot-api) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-node-telegram-bot-api.svg)](https://travis-ci.org/npmtest/node-npmtest-node-telegram-bot-api)

#### Telegram Bot API

[![NPM](https://nodei.co/npm/node-telegram-bot-api.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-telegram-bot-api)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-node-telegram-bot-api/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-node-telegram-bot-api/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/test-report.html](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-node-telegram-bot-api/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-telegram-bot-api/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-telegram-bot-api/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-telegram-bot-api/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-node-telegram-bot-api/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "node-telegram-bot-api",
    "version": "0.27.0",
    "description": "Telegram Bot API",
    "main": "./index.js",
    "directories": {
        "example": "examples",
        "test": "test"
    },
    "keywords": [
        "telegram",
        "telegram bot",
        "telegram bot api",
        "bot"
    ],
    "scripts": {
        "gen-doc": "jsdoc2md --files src/telegram.js --template doc/api.hbs > doc/api.md",
        "build": "babel -d ./lib src",
        "prepublish": "npm run build && npm run gen-doc",
        "eslint": "eslint ./src ./test ./examples",
        "mocha": "mocha",
        "pretest": "npm run build",
        "test": "npm run eslint && istanbul cover ./node_modules/mocha/bin/_mocha"
    },
    "author": "Yago Pérez <yagoperezs@gmail.com>",
    "license": "MIT",
    "engines": {
        "node": ">=0.12"
    },
    "dependencies": {
        "array.prototype.findindex": "^2.0.0",
        "bl": "^1.1.2",
        "bluebird": "^3.3.4",
        "debug": "^2.2.0",
        "depd": "^1.1.0",
        "eventemitter3": "^2.0.2",
        "file-type": "^3.9.0",
        "mime": "^1.3.4",
        "pump": "^1.0.1",
        "request": "^2.69.0",
        "request-promise": "^4.1.1"
    },
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-eslint": "^6.1.2",
        "babel-plugin-transform-class-properties": "^6.6.0",
        "babel-plugin-transform-es2015-destructuring": "^6.6.5",
        "babel-plugin-transform-es2015-parameters": "^6.7.0",
        "babel-plugin-transform-es2015-shorthand-properties": "^6.5.0",
        "babel-plugin-transform-es2015-spread": "^6.6.5",
        "babel-plugin-transform-object-rest-spread": "^6.6.5",
        "babel-plugin-transform-strict-mode": "^6.6.5",
        "babel-preset-es2015": "^6.6.0",
        "babel-register": "^6.7.2",
        "contributor": "^0.1.25",
        "eslint": "^2.13.1",
        "eslint-config-airbnb": "^6.2.0",
        "eslint-plugin-mocha": "^4.8.0",
        "is": "^3.1.0",
        "istanbul": "^1.1.0-alpha.1",
        "jsdoc-to-markdown": "^2.0.1",
        "mocha": "^3.2.0",
        "mocha-lcov-reporter": "^1.2.0",
        "node-static": "^0.7.9"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/yagop/node-telegram-bot-api.git"
    },
    "bugs": {
        "url": "https://github.com/yagop/node-telegram-bot-api/issues"
    },
    "homepage": "https://github.com/yagop/node-telegram-bot-api",
    "contributors": [
        {
            "name": "Anton Mironov",
            "url": "https://github.com/mironov",
            "contributions": 1,
            "additions": 51,
            "deletions": 15,
            "hireable": true
        },
        {
            "name": "Daniil Yastremskiy",
            "url": "https://github.com/TheBeastOfCaerbannog",
            "contributions": 1,
            "additions": 36,
            "deletions": 0,
            "hireable": true
        },
        {
            "name": null,
            "email": null,
            "url": "https://github.com/Ni2c2k",
            "contributions": 1,
            "additions": 4,
            "deletions": 4,
            "hireable": null
        },
        {
            "name": "Alexander Tarmolov",
            "url": "https://github.com/tarmolov",
            "contributions": 1,
            "additions": 5,
            "deletions": 0,
            "hireable": null
        },
        {
            "name": "Plusb Preco",
            "url": "https://github.com/preco21",
            "contributions": 1,
            "additions": 1,
            "deletions": 0,
            "hireable": null
        },
        {
            "name": "Ola Flisbäck",
            "email": null,
            "url": "https://github.com/oflisback",
            "contributions": 1,
            "additions": 3,
            "deletions": 3,
            "hireable": true
        },
        {
            "name": null,
            "email": null,
            "url": "https://github.com/GingerPlusPlus",
            "contributions": 1,
            "additions": 6,
            "deletions": 2,
            "hireable": null
        },
        {
            "name": "Sergey Bogdanov",
            "url": "https://github.com/desunit",
            "contributions": 1,
            "additions": 1,
            "deletions": 1,
            "hireable": null
        },
        {
            "name": "Mikhail Burshteyn",
            "email": null,
            "url": "https://github.com/m-burst",
            "contributions": 1,
            "additions": 12,
            "deletions": 5,
            "hireable": null
        },
        {
            "name": "Horus Lugo",
            "url": "https://github.com/HorusGoul",
            "contributions": 1,
            "additions": 108,
            "deletions": 1,
            "hireable": true
        },
        {
            "name": "Serhii Dmytruk",
            "url": "https://github.com/serhiidmytruk",
            "contributions": 1,
            "additions": 35,
            "deletions": 1,
            "hireable": null
        },
        {
            "name": "Conor Fennell",
            "email": null,
            "url": "https://github.com/conorfennell",
            "contributions": 1,
            "additions": 50,
            "deletions": 1,
            "hireable": null
        },
        {
            "name": "Aleksandr L.",
            "url": "https://github.com/w-site",
            "contributions": 1,
            "additions": 24,
            "deletions": 0,
            "hireable": null
        },
        {
            "name": "Matthew Brandly",
            "url": "https://github.com/brandly",
            "contributions": 1,
            "additions": 1,
            "deletions": 1,
            "hireable": null
        },
        {
            "name": "Anton",
            "email": null,
            "url": "https://github.com/Feverqwe",
            "contributions": 1,
            "additions": 23,
            "deletions": 5,
            "hireable": null
        },
        {
            "name": "Patricio López Juri",
            "url": "https://github.com/mrpatiwi",
            "contributions": 1,
            "additions": 49,
            "deletions": 2,
            "hireable": true
        },
        {
            "name": "Guido García",
            "url": "https://github.com/palmerabollo",
            "contributions": 1,
            "additions": 1,
            "deletions": 1,
            "hireable": true
        },
        {
            "name": "Sebastian Troć",
            "url": "https://github.com/SebastianTroc",
            "contributions": 1,
            "additions": 1,
            "deletions": 1,
            "hireable": null
        },
        {
            "name": "Mohammed Sohail",
            "url": "https://github.com/kamikazechaser",
            "contributions": 2,
            "additions": 20,
            "deletions": 5,
            "hireable": true
        },
        {
            "name": "Jishnu Mohan",
            "url": "https://github.com/jishnu7",
            "contributions": 2,
            "additions": 84,
            "deletions": 0,
            "hireable": true
        },
        {
            "name": "Jérémy Gotteland",
            "email": null,
            "url": "https://github.com/Tketa",
            "contributions": 2,
            "additions": 81,
            "deletions": 3,
            "hireable": null
        },
        {
            "name": "Alex Godko",
            "url": "https://github.com/koloboid",
            "contributions": 2,
            "additions": 2,
            "deletions": 2,
            "hireable": true
        },
        {
            "name": "Dardan Neziri",
            "url": "https://github.com/knock-in",
            "contributions": 2,
            "additions": 22,
            "deletions": 16,
            "hireable": true
        },
        {
            "name": "Cristian Baldi",
            "url": "https://github.com/crisbal",
            "contributions": 2,
            "additions": 26,
            "deletions": 1,
            "hireable": true
        },
        {
            "name": "Vitaly Aminev",
            "email": null,
            "url": "https://github.com/AVVS",
            "contributions": 2,
            "additions": 1065,
            "deletions": 1001,
            "hireable": true
        },
        {
            "name": null,
            "url": "https://github.com/evolun",
            "contributions": 2,
            "additions": 7,
            "deletions": 3,
            "hireable": null
        },
        {
            "name": "Iiro Jäppinen",
            "email": null,
            "url": "https://github.com/iiroj",
            "contributions": 2,
            "additions": 40,
            "deletions": 0,
            "hireable": null
        },
        {
            "name": "TJ Horner",
            "url": "https://github.com/tjhorner",
            "contributions": 2,
            "additions": 223,
            "deletions": 1,
            "hireable": null
        },
        {
            "name": "Rafael Kr",
            "email": null,
            "url": "https://github.com/RafaelKr",
            "contributions": 3,
            "additions": 3,
            "deletions": 2,
            "hireable": null
        },
        {
            "name": "Vítor Augusto da Silva Vasconcellos",
            "url": "https://github.com/HeavenVolkoff",
            "contributions": 2,
            "additions": 12,
            "deletions": 0,
            "hireable": true
        },
        {
            "name": "Rey",
            "email": null,
            "url": "https://github.com/reyy",
            "contributions": 2,
            "additions": 34,
            "deletions": 25,
            "hireable": null
        },
        {
            "name": "Ivan Skorokhodov",
            "url": "https://github.com/universome",
            "contributions": 3,
            "additions": 219,
            "deletions": 5,
            "hireable": null
        },
        {
            "name": "Riddler",
            "email": null,
            "url": "https://github.com/Waterloo",
            "contributions": 3,
            "additions": 64,
            "deletions": 2,
            "hireable": true
        },
        {
            "name": null,
            "url": "https://github.com/EXL",
            "contributions": 4,
            "additions": 4,
            "deletions": 4,
            "hireable": true
        },
        {
            "name": "Yago",
            "url": "https://github.com/yagop",
            "contributions": 194,
            "additions": 3014,
            "deletions": 1173,
            "hireable": true
        },
        {
            "name": "Ilias Ismanalijev",
            "url": "https://github.com/Illyism",
            "contributions": 7,
            "additions": 140,
            "deletions": 10,
            "hireable": true
        },
        {
            "name": "Chris54721",
            "email": null,
            "url": "https://github.com/chris54721",
            "contributions": 5,
            "additions": 22,
            "deletions": 6,
            "hireable": null
        },
        {
            "name": "Gocho Mugo",
            "url": "https://github.com/GochoMugo",
            "contributions": 80,
            "additions": 4590,
            "deletions": 2377,
            "hireable": true
        }
    ]
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
