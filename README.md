# npmdoc-redux-form

#### basic api documentation for  [redux-form (v6.6.3)](https://redux-form.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-redux-form.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-redux-form) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-redux-form.svg)](https://travis-ci.org/npmdoc/node-npmdoc-redux-form)

#### A higher order component decorator for forms using Redux and React

[![NPM](https://nodei.co/npm/redux-form.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/redux-form)

- [https://npmdoc.github.io/node-npmdoc-redux-form/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-redux-form/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-redux-form/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-redux-form/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-redux-form/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-redux-form/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Erik Rasmussen",
        "url": "http://github.com/erikras"
    },
    "bugs": {
        "url": "https://github.com/erikras/redux-form/issues"
    },
    "dependencies": {
        "deep-equal": "^1.0.1",
        "es6-error": "^4.0.0",
        "hoist-non-react-statics": "^1.2.0",
        "invariant": "^2.2.2",
        "is-promise": "^2.1.0",
        "lodash": "^4.17.3",
        "lodash-es": "^4.17.3",
        "prop-types": "^15.5.6"
    },
    "description": "A higher order component decorator for forms using Redux and React",
    "devDependencies": {
        "babel-cli": "^6.24.1",
        "babel-core": "^6.24.1",
        "babel-eslint": "^7.2.2",
        "babel-loader": "^6.2.10",
        "babel-plugin-istanbul": "^4.1.1",
        "babel-plugin-lodash": "^3.2.11",
        "babel-plugin-syntax-async-functions": "^6.13.0",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.24.1",
        "babel-plugin-transform-regenerator": "^6.24.1",
        "babel-preset-es2015-no-commonjs": "^0.0.2",
        "babel-preset-react": "^6.24.1",
        "babel-preset-stage-2": "^6.24.1",
        "babel-register": "^6.24.1",
        "codecov.io": "^0.1.6",
        "cross-env": "^4.0.0",
        "eslint": "^3.17.1",
        "eslint-config-react-app": "^0.6.2",
        "eslint-plugin-flowtype": "^2.30.4",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-jsx-a11y": "^4.0.0",
        "eslint-plugin-react": "^6.10.3",
        "expect": "^1.20.2",
        "expect-element": "^1.1.1",
        "expect-immutable": "^0.0.3",
        "expect-predicate": "^1.0.0",
        "flux-standard-action": "^1.0.0",
        "jsdom": "^9.9.1",
        "lodash-webpack-plugin": "^0.11.2",
        "mocha": "^3.2.0",
        "nyc": "^10.2.0",
        "react": "^15.5.4",
        "react-dom": "^15.5.4",
        "react-redux": "^5.0.4",
        "redux": "^3.6.0",
        "redux-immutablejs": "^0.0.8",
        "rifraf": "^2.0.3",
        "rimraf": "^2.5.4",
        "stringstream": "^0.0.5",
        "tmp": "0.0.31",
        "webpack": "^2.3.2"
    },
    "directories": {},
    "dist": {
        "shasum": "62362654f2214c83a8f9fcb8313702bb46f92205",
        "tarball": "https://registry.npmjs.org/redux-form/-/redux-form-6.6.3.tgz"
    },
    "files": [
        "README.md",
        "es",
        "lib",
        "dist",
        "immutable.js"
    ],
    "gitHead": "38382a4e5db639637ed3740b2168083cd05d1226",
    "homepage": "https://redux-form.com/",
    "jsnext:main": "./es/index.js",
    "keywords": [
        "react",
        "reactjs",
        "flux",
        "redux",
        "react-redux",
        "redux-form",
        "form",
        "decorator"
    ],
    "license": "MIT",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "erikras"
        }
    ],
    "module": "./es/index.js",
    "name": "redux-form",
    "npmFileMap": [
        {
            "basePath": "/dist/",
            "files": [
                "*.js"
            ]
        }
    ],
    "npmName": "redux-form",
    "nyc": {
        "include": [
            "src/**/*.js"
        ],
        "sourceMap": false,
        "instrument": false
    },
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^15.0.0",
        "react-redux": "^4.3.0 || ^5.0.0",
        "redux": "^3.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/erikras/redux-form.git"
    },
    "scripts": {
        "build": "npm run build:lib && npm run build:es && npm run build:umd && npm run build:umd:min",
        "build:es": "cross-env BABEL_ENV=es babel src --out-dir es",
        "build:lib": "babel src --out-dir lib",
        "build:umd": "cross-env NODE_ENV=development webpack src/index.js dist/redux-form.js",
        "build:umd:min": "cross-env NODE_ENV=production webpack src/index.js dist/redux-form.min.js",
        "clean": "rimraf dist lib",
        "example": "npm --prefix ./examples/$form install && npm --prefix ./examples/$form start",
        "example:asyncValidation": "form=asyncValidation npm run example",
        "example:fieldArrays": "form=fieldArrays npm run example",
        "example:fieldLevelValidation": "form=fieldLevelValidation npm run example",
        "example:immutable": "form=immutable npm run example",
        "example:initializeFromState": "form=initializeFromState npm run example",
        "example:material-ui": "form=material-ui npm run example",
        "example:normalizing": "form=normalizing npm run example",
        "example:react-widgets": "form=react-widgets npm run example",
        "example:selectingFormValues": "form=selectingFormValues npm run example",
        "example:simple": "form=simple npm run example",
        "example:submitValidation": "form=submitValidation npm run example",
        "example:syncValidation": "form=syncValidation npm run example",
        "example:wizard": "form=wizard npm run example",
        "lint": "eslint src",
        "prepublish": "npm run test && npm run clean && npm run build",
        "test": "mocha --compilers js:babel-register --recursive --recursive \"src/**/__tests__/*\" --require src/__tests__/setup.js",
        "test:codecov": "cat ./coverage/lcov.info | ./node_modules/codecov.io/bin/codecov.io.js",
        "test:cov": "cross-env NODE_ENV=test nyc --reporter=lcov --reporter=text npm test",
        "test:watch": "npm test -- --watch"
    },
    "version": "6.6.3",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
