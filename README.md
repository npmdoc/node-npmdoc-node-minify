# api documentation for  [node-minify (v2.0.3)](https://github.com/srod/node-minify)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-minify.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-minify) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-minify.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-minify)
#### Javascript / CSS minifier based on Babili / YUI Compressor / Google Closure Compiler / UglifyJS2 / Sqwish / Clean-css / CSSO

[![NPM](https://nodei.co/npm/node-minify.png?downloads=true)](https://www.npmjs.com/package/node-minify)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-minify/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-minify_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-minify/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-minify/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-minify/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rodolphe Stoclin",
        "email": "rodolphe@2clics.net",
        "url": "http://2clics.net"
    },
    "bugs": {
        "url": "https://github.com/srod/node-minify/issues"
    },
    "dependencies": {
        "babel-core": "^6.18.0",
        "babel-preset-babili": "0.0.5",
        "bluebird": "^3.4.6",
        "clean-css": "^3.4.19",
        "csso": "^2.3.0",
        "depd": "^1.1.0",
        "glob": "^7.1.1",
        "google-closure-compiler-js": "^20161024.0.0",
        "mkdirp": "^0.5.1",
        "node-version": "^1.0.0",
        "sqwish": "^0.2.2",
        "uglify-js": "^2.7.4",
        "xtend": "^4.0.1"
    },
    "description": "Javascript / CSS minifier based on Babili / YUI Compressor / Google Closure Compiler / UglifyJS2 / Sqwish / Clean-css / CSSO",
    "devDependencies": {
        "babel-preset-es2015": "^6.18.0",
        "chai": "^3.5.0",
        "coveralls": "^2.11.12",
        "decache": "^4.1.0",
        "eslint": "^3.9.1",
        "istanbul": "^0.4.5",
        "mocha": "^3.1.2",
        "should": "^11.1.1",
        "sinon": "^1.17.5"
    },
    "directories": {},
    "dist": {
        "shasum": "8d972fa5d7a2d5bfbf613fa67797c1d59fe4cba5",
        "tarball": "https://registry.npmjs.org/node-minify/-/node-minify-2.0.3.tgz"
    },
    "engines": {
        "iojs": ">=1.0.0",
        "node": ">=0.12.0"
    },
    "gitHead": "e7812e0c434d7f39732063e9fa680addcdda7762",
    "homepage": "https://github.com/srod/node-minify",
    "keywords": [
        "compressor",
        "minify",
        "minifier",
        "yui",
        "gcc",
        "google",
        "closure",
        "compiler",
        "uglifyjs",
        "uglifyjs2",
        "windows",
        "sqwish",
        "clean-css",
        "csso",
        "babili"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "srod",
            "email": "rodolphe@2clics.net"
        }
    ],
    "name": "node-minify",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/srod/node-minify.git"
    },
    "scripts": {
        "clean": "rm -f ./examples/public/dist/*",
        "clean-cov": "npm run clean && rm -Rf ./coverage",
        "eslint": "eslint index.js lib test || true",
        "mocha": "mocha --bail --timeout 60000 --reporter spec || true",
        "posttest": "npm run clean",
        "pretest": "npm run eslint",
        "publish-beta": "npm publish --tag beta",
        "publish-latest": "npm publish",
        "release-major": "npm version major -m 'Bump %s' && git push --tags origin HEAD:develop",
        "release-minor": "npm version minor -m 'Bump %s' && git push --tags origin HEAD:develop",
        "release-patch": "npm version patch -m 'Bump %s' && git push --tags origin HEAD:develop",
        "test": "npm run mocha",
        "test-cov": "npm run pretest && istanbul cover ./node_modules/mocha/bin/_mocha -- -t 60000 -R spec"
    },
    "version": "2.0.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-minify](#apidoc.module.node-minify)
1.  [function <span class="apidocSignatureSpan">node-minify.</span>minify (settings)](#apidoc.element.node-minify.minify)
1.  object <span class="apidocSignatureSpan">node-minify.</span>utils

#### [module node-minify.utils](#apidoc.module.node-minify.utils)
1.  [function <span class="apidocSignatureSpan">node-minify.utils.</span>buildArgs (options)](#apidoc.element.node-minify.utils.buildArgs)
1.  [function <span class="apidocSignatureSpan">node-minify.utils.</span>clone (obj)](#apidoc.element.node-minify.utils.clone)
1.  [function <span class="apidocSignatureSpan">node-minify.utils.</span>isNodeV4AndHigher ()](#apidoc.element.node-minify.utils.isNodeV4AndHigher)
1.  [function <span class="apidocSignatureSpan">node-minify.utils.</span>readFile (file)](#apidoc.element.node-minify.utils.readFile)
1.  [function <span class="apidocSignatureSpan">node-minify.utils.</span>writeFile (file, content)](#apidoc.element.node-minify.utils.writeFile)



# <a name="apidoc.module.node-minify"></a>[module node-minify](#apidoc.module.node-minify)

#### <a name="apidoc.element.node-minify.minify"></a>[function <span class="apidocSignatureSpan">node-minify.</span>minify (settings)](#apidoc.element.node-minify.minify)
- description and source-code
```javascript
function minify(settings) {
  deprecated(this.constructor.name, settings);
  settings = setup(settings);
  return compress(settings).nodeify(settings.callback);
}
```
- example usage
```shell
...

## Quick Start

'''js
var compressor = require('node-minify');

// Using Google Closure Compiler
compressor.minify({
  compressor: 'gcc',
  input: 'foo.js',
  output: 'bar.js',
  callback: function (err, min) {}
});

// Using UglifyJS
...
```



# <a name="apidoc.module.node-minify.utils"></a>[module node-minify.utils](#apidoc.module.node-minify.utils)

#### <a name="apidoc.element.node-minify.utils.buildArgs"></a>[function <span class="apidocSignatureSpan">node-minify.utils.</span>buildArgs (options)](#apidoc.element.node-minify.utils.buildArgs)
- description and source-code
```javascript
function buildArgs(options) {
  var args = [];

  Object.keys(options).forEach(function(key) {
    if (options[key] && options[key] !== false) {
      args.push('--' + key);
    }

    if (options[key] && options[key] !== true) {
      args.push(options[key]);
    }
  });

  return args;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-minify.utils.clone"></a>[function <span class="apidocSignatureSpan">node-minify.utils.</span>clone (obj)](#apidoc.element.node-minify.utils.clone)
- description and source-code
```javascript
function clone(obj) {
  return JSON.parse(JSON.stringify(obj));
}
```
- example usage
```shell
...
 * @param {Object} inputSettings
 * @return {Object}
 */

function setup(inputSettings) {
  checkMandatories(inputSettings);

  var settings = extend(utils.clone(defaultSettings), inputSettings);
  settings = extend(settings, wildcards(settings.input, settings.publicFolder));
  settings = extend(settings, setPublicFolder(settings.input, settings.publicFolder));

  return settings;
}

/**
...
```

#### <a name="apidoc.element.node-minify.utils.isNodeV4AndHigher"></a>[function <span class="apidocSignatureSpan">node-minify.utils.</span>isNodeV4AndHigher ()](#apidoc.element.node-minify.utils.isNodeV4AndHigher)
- description and source-code
```javascript
function isNodeV4AndHigher() {
  return parseInt(nodeVersion.major, 10) >= 4;
}
```
- example usage
```shell
...
var gcc;
var gccJava = require('./compressors/gcc-java');
var noCompress = require('./compressors/no-compress');
var sqwish = require('./compressors/sqwish');
var uglifyjs = require('./compressors/uglifyjs');
var yui = require('./compressors/yui');

if ((process.execArgv && process.execArgv.indexOf('--use_strict') > -1) || !utils.isNodeV4AndHigher()) {
 gcc = require('./compressors/gcc-java');
} else {
 gcc = require('./compressors/gcc');
}

/**
* Mapping input compressors to functions
...
```

#### <a name="apidoc.element.node-minify.utils.readFile"></a>[function <span class="apidocSignatureSpan">node-minify.utils.</span>readFile (file)](#apidoc.element.node-minify.utils.readFile)
- description and source-code
```javascript
function readFile(file) {
  return fs.readFileSync(file, 'utf8');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-minify.utils.writeFile"></a>[function <span class="apidocSignatureSpan">node-minify.utils.</span>writeFile (file, content)](#apidoc.element.node-minify.utils.writeFile)
- description and source-code
```javascript
function writeFile(file, content) {
  fs.writeFileSync(file, content, 'utf8');
  return content;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
