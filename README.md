# npmdoc-node-minify

#### api documentation for  [node-minify (v2.0.4)](https://github.com/srod/node-minify)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-minify.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-minify) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-minify.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-minify)

#### Javascript / CSS minifier based on Babili / YUI Compressor / Google Closure Compiler / UglifyJS2 / Sqwish / Clean-css / CSSO

[![NPM](https://nodei.co/npm/node-minify.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-minify)

- [https://npmdoc.github.io/node-npmdoc-node-minify/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-minify/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-minify/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-minify/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-minify/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-minify/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rodolphe Stoclin",
        "url": "http://2clics.net"
    },
    "bugs": {
        "url": "https://github.com/srod/node-minify/issues"
    },
    "dependencies": {
        "babel-core": "6.22.1",
        "babel-preset-babili": "0.0.11",
        "bluebird": "3.4.7",
        "clean-css": "4.0.6",
        "csso": "2.3.1",
        "depd": "1.1.0",
        "glob": "7.1.1",
        "google-closure-compiler-js": "20170124.0.0",
        "mkdirp": "0.5.1",
        "node-version": "1.0.0",
        "sqwish": "0.2.2",
        "uglify-js": "2.7.5",
        "xtend": "4.0.1"
    },
    "description": "Javascript / CSS minifier based on Babili / YUI Compressor / Google Closure Compiler / UglifyJS2 / Sqwish / Clean-css / CSSO",
    "devDependencies": {
        "babel-preset-es2015": "6.24.1",
        "chai": "3.5.0",
        "coveralls": "2.13.0",
        "decache": "4.1.0",
        "eslint": "3.19.0",
        "istanbul": "0.4.5",
        "mocha": "3.2.0",
        "should": "11.2.1",
        "sinon": "2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "d2fb460af56e13b17a85b8fd1a59380c1776386c",
        "tarball": "https://registry.npmjs.org/node-minify/-/node-minify-2.0.4.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "0d4d92eda61aa935aee745c206d417eeeb4d3151",
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
            "name": "srod"
        }
    ],
    "name": "node-minify",
    "optionalDependencies": {},
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
        "release-major": "npm version major -m 'Bump %s' && git push --tags origin HEAD:master",
        "release-minor": "npm version minor -m 'Bump %s' && git push --tags origin HEAD:master",
        "release-patch": "npm version patch -m 'Bump %s' && git push --tags origin HEAD:master",
        "test": "npm run mocha",
        "test-cov": "npm run pretest && istanbul cover ./node_modules/mocha/bin/_mocha -- -t 60000 -R spec"
    },
    "version": "2.0.4"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
