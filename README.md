# api documentation for  [sleep (v5.1.0)](http://github.com/erikdubbelboer/node-sleep)  [![npm package](https://img.shields.io/npm/v/npmdoc-sleep.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-sleep) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sleep.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sleep)
#### Add sleep() and usleep() to nodejs

[![NPM](https://nodei.co/npm/sleep.png?downloads=true)](https://www.npmjs.com/package/sleep)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sleep/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-sleep_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sleep/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sleep/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sleep/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Erik Dubbelboer",
        "email": "erik@dubbelboer.com"
    },
    "bugs": {
        "url": "https://github.com/erikdubbelboer/node-sleep/issues"
    },
    "dependencies": {
        "nan": ">=2.0.0"
    },
    "description": "Add sleep() and usleep() to nodejs",
    "devDependencies": {
        "mocha": "^3.0.2"
    },
    "directories": {},
    "dist": {
        "shasum": "0e0b16205d9f9e3b0a95357744b103e797b4c7c1",
        "tarball": "https://registry.npmjs.org/sleep/-/sleep-5.1.0.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "gitHead": "b5e4fb12e2cf7aa5f1b734720c0d9c1b17acaea1",
    "gypfile": true,
    "homepage": "http://github.com/erikdubbelboer/node-sleep",
    "keywords": [
        "sleep",
        "usleep"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "erikdubbelboer",
            "email": "erik@dubbelboer.com"
        }
    ],
    "name": "sleep",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/erikdubbelboer/node-sleep.git"
    },
    "scripts": {
        "install": "node-gyp rebuild",
        "test": "mocha"
    },
    "version": "5.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module sleep](#apidoc.module.sleep)
1.  [function <span class="apidocSignatureSpan"></span>sleep ()](#apidoc.element.sleep.sleep)
1.  [function <span class="apidocSignatureSpan">sleep.</span>msleep (miliseconds)](#apidoc.element.sleep.msleep)
1.  [function <span class="apidocSignatureSpan">sleep.</span>usleep ()](#apidoc.element.sleep.usleep)



# <a name="apidoc.module.sleep"></a>[module sleep](#apidoc.module.sleep)

#### <a name="apidoc.element.sleep.sleep"></a>[function <span class="apidocSignatureSpan"></span>sleep ()](#apidoc.element.sleep.sleep)
- description and source-code
```javascript
sleep = function () { [native code] }
```
- example usage
```shell
...
**These calls will block execution of all JavaScript by halting Node.js' event loop!**

Usage
-----

    var sleep = require('sleep');

* 'sleep.sleep(n)': sleep for 'n' seconds
* 'sleep.msleep(n)': sleep for 'n' miliseconds
* 'sleep.usleep(n)': sleep for 'n' microseconds (1 second is 1000000 microseconds)


[1]: http://linux.die.net/man/3/sleep
[2]: http://linux.die.net/man/3/usleep
...
```

#### <a name="apidoc.element.sleep.msleep"></a>[function <span class="apidocSignatureSpan">sleep.</span>msleep (miliseconds)](#apidoc.element.sleep.msleep)
- description and source-code
```javascript
msleep = function (miliseconds) {
  if (miliseconds < 1 || miliseconds % 1 != 0) {
    throw new Exception('Expected number of miliseconds');
  }
  sleep.usleep(miliseconds * 1000);
}
```
- example usage
```shell
...

Usage
-----

    var sleep = require('sleep');

* 'sleep.sleep(n)': sleep for 'n' seconds
* 'sleep.msleep(n)': sleep for 'n' miliseconds
* 'sleep.usleep(n)': sleep for 'n' microseconds (1 second is 1000000 microseconds)


[1]: http://linux.die.net/man/3/sleep
[2]: http://linux.die.net/man/3/usleep
...
```

#### <a name="apidoc.element.sleep.usleep"></a>[function <span class="apidocSignatureSpan">sleep.</span>usleep ()](#apidoc.element.sleep.usleep)
- description and source-code
```javascript
usleep = function () { [native code] }
```
- example usage
```shell
...
Usage
-----

    var sleep = require('sleep');

* 'sleep.sleep(n)': sleep for 'n' seconds
* 'sleep.msleep(n)': sleep for 'n' miliseconds
* 'sleep.usleep(n)': sleep for 'n' microseconds (1 second is 1000000 microseconds)


[1]: http://linux.die.net/man/3/sleep
[2]: http://linux.die.net/man/3/usleep
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
