# api documentation for  [redux-form (v6.6.1)](https://redux-form.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-redux-form.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-redux-form) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-redux-form.svg)](https://travis-ci.org/npmdoc/node-npmdoc-redux-form)
#### A higher order component decorator for forms using Redux and React

[![NPM](https://nodei.co/npm/redux-form.png?downloads=true)](https://www.npmjs.com/package/redux-form)

[![apidoc](https://npmdoc.github.io/node-npmdoc-redux-form/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-redux-form_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-redux-form/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-redux-form/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-redux-form/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Erik Rasmussen",
        "email": "rasmussenerik@gmail.com",
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
        "lodash-es": "^4.17.3"
    },
    "description": "A higher order component decorator for forms using Redux and React",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-core": "^6.21.0",
        "babel-eslint": "^7.2.1",
        "babel-loader": "^6.2.10",
        "babel-plugin-istanbul": "^4.1.1",
        "babel-plugin-lodash": "^3.2.11",
        "babel-plugin-syntax-async-functions": "^6.13.0",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.18.0",
        "babel-plugin-transform-regenerator": "^6.21.0",
        "babel-preset-es2015-no-commonjs": "^0.0.2",
        "babel-preset-react": "^6.16.0",
        "babel-preset-stage-2": "^6.18.0",
        "babel-register": "^6.18.0",
        "codecov.io": "^0.1.6",
        "cross-env": "^3.1.3",
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
        "react": "^15.4.1",
        "react-addons-test-utils": "^15.4.1",
        "react-dom": "^15.4.1",
        "react-redux": "^5.0.1",
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
        "shasum": "368dc4fc41301bfb1cd471b059a2215573649c8c",
        "tarball": "https://registry.npmjs.org/redux-form/-/redux-form-6.6.1.tgz"
    },
    "files": [
        "README.md",
        "es",
        "lib",
        "dist",
        "immutable.js"
    ],
    "gitHead": "2a86b097fe35faa0bbaefec53a5db0d438610ae0",
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
            "name": "erikras",
            "email": "rasmussenerik@gmail.com"
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
    "readme": "ERROR: No README data found!",
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
    "version": "6.6.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module redux-form](#apidoc.module.redux-form)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>Field (props, context)](#apidoc.element.redux-form.Field)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>FieldArray (props, context)](#apidoc.element.redux-form.FieldArray)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>Fields (props, context)](#apidoc.element.redux-form.Fields)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>Form (props, context)](#apidoc.element.redux-form.Form)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>FormSection (props, context)](#apidoc.element.redux-form.FormSection)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>SubmissionError (errors)](#apidoc.element.redux-form.SubmissionError)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayInsert (form, field, index, value)](#apidoc.element.redux-form.arrayInsert)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayMove (form, field, from, to)](#apidoc.element.redux-form.arrayMove)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayPop (form, field)](#apidoc.element.redux-form.arrayPop)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayPush (form, field, value)](#apidoc.element.redux-form.arrayPush)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayRemove (form, field, index)](#apidoc.element.redux-form.arrayRemove)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayRemoveAll (form, field)](#apidoc.element.redux-form.arrayRemoveAll)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayShift (form, field)](#apidoc.element.redux-form.arrayShift)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arraySplice (form, field, index, removeNum, value)](#apidoc.element.redux-form.arraySplice)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arraySwap (form, field, indexA, indexB)](#apidoc.element.redux-form.arraySwap)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>arrayUnshift (form, field, value)](#apidoc.element.redux-form.arrayUnshift)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>autofill (form, field, value)](#apidoc.element.redux-form.autofill)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>blur (form, field, value, touch)](#apidoc.element.redux-form.blur)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>change (form, field, value, touch, persistentSubmitErrors)](#apidoc.element.redux-form.change)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>destroy ()](#apidoc.element.redux-form.destroy)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>focus (form, field)](#apidoc.element.redux-form.focus)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>formValueSelector (form)](#apidoc.element.redux-form.formValueSelector)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>getFormAsyncErrors (form)](#apidoc.element.redux-form.getFormAsyncErrors)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>getFormInitialValues (form)](#apidoc.element.redux-form.getFormInitialValues)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>getFormNames ()](#apidoc.element.redux-form.getFormNames)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>getFormSubmitErrors (form)](#apidoc.element.redux-form.getFormSubmitErrors)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>getFormSyncErrors (form)](#apidoc.element.redux-form.getFormSyncErrors)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>getFormSyncWarnings (form)](#apidoc.element.redux-form.getFormSyncWarnings)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>getFormValues (form)](#apidoc.element.redux-form.getFormValues)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>hasSubmitFailed (form)](#apidoc.element.redux-form.hasSubmitFailed)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>hasSubmitSucceeded (form)](#apidoc.element.redux-form.hasSubmitSucceeded)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>initialize (form, values, keepDirty)](#apidoc.element.redux-form.initialize)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>isDirty (form, getFormState)](#apidoc.element.redux-form.isDirty)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>isInvalid (form, getFormState)](#apidoc.element.redux-form.isInvalid)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>isPristine (form)](#apidoc.element.redux-form.isPristine)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>isSubmitting (form)](#apidoc.element.redux-form.isSubmitting)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>isValid (form)](#apidoc.element.redux-form.isValid)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>propTypes.array ()](#apidoc.element.redux-form.propTypes.array)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>propTypes.error ()](#apidoc.element.redux-form.propTypes.error)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>propTypes.initialValues ()](#apidoc.element.redux-form.propTypes.initialValues)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>propTypes.triggerSubmit ()](#apidoc.element.redux-form.propTypes.triggerSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>reducer ()](#apidoc.element.redux-form.reducer)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>reduxForm (initialConfig)](#apidoc.element.redux-form.reduxForm)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>registerField (form, name, type)](#apidoc.element.redux-form.registerField)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>reset (form)](#apidoc.element.redux-form.reset)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>setSubmitFailed (form)](#apidoc.element.redux-form.setSubmitFailed)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>setSubmitSucceeded (form)](#apidoc.element.redux-form.setSubmitSucceeded)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>startAsyncValidation (form, field)](#apidoc.element.redux-form.startAsyncValidation)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>startSubmit (form)](#apidoc.element.redux-form.startSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>stopAsyncValidation (form, errors)](#apidoc.element.redux-form.stopAsyncValidation)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>stopSubmit (form, errors)](#apidoc.element.redux-form.stopSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>submit (form)](#apidoc.element.redux-form.submit)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>touch (form)](#apidoc.element.redux-form.touch)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>unregisterField (form, name)](#apidoc.element.redux-form.unregisterField)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>untouch (form)](#apidoc.element.redux-form.untouch)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>values (config)](#apidoc.element.redux-form.values)
1.  object <span class="apidocSignatureSpan">redux-form.</span>ConnectedField
1.  object <span class="apidocSignatureSpan">redux-form.</span>ConnectedFieldArray
1.  object <span class="apidocSignatureSpan">redux-form.</span>ConnectedFields
1.  object <span class="apidocSignatureSpan">redux-form.</span>actionTypes
1.  object <span class="apidocSignatureSpan">redux-form.</span>actions
1.  object <span class="apidocSignatureSpan">redux-form.</span>asyncValidation
1.  object <span class="apidocSignatureSpan">redux-form.</span>createAll
1.  object <span class="apidocSignatureSpan">redux-form.</span>createFieldArrayProps
1.  object <span class="apidocSignatureSpan">redux-form.</span>createFieldProps
1.  object <span class="apidocSignatureSpan">redux-form.</span>defaultShouldAsyncValidate
1.  object <span class="apidocSignatureSpan">redux-form.</span>defaultShouldValidate
1.  object <span class="apidocSignatureSpan">redux-form.</span>deleteInWithCleanUp
1.  object <span class="apidocSignatureSpan">redux-form.</span>generateValidator
1.  object <span class="apidocSignatureSpan">redux-form.</span>handleSubmit
1.  object <span class="apidocSignatureSpan">redux-form.</span>hasError
1.  object <span class="apidocSignatureSpan">redux-form.</span>isChecked
1.  object <span class="apidocSignatureSpan">redux-form.</span>propTypes

#### [module redux-form.ConnectedField](#apidoc.module.redux-form.ConnectedField)
1.  [function <span class="apidocSignatureSpan">redux-form.ConnectedField.</span>default (_ref)](#apidoc.element.redux-form.ConnectedField.default)

#### [module redux-form.ConnectedFieldArray](#apidoc.module.redux-form.ConnectedFieldArray)
1.  [function <span class="apidocSignatureSpan">redux-form.ConnectedFieldArray.</span>default (_ref)](#apidoc.element.redux-form.ConnectedFieldArray.default)

#### [module redux-form.ConnectedFields](#apidoc.module.redux-form.ConnectedFields)
1.  [function <span class="apidocSignatureSpan">redux-form.ConnectedFields.</span>default (_ref)](#apidoc.element.redux-form.ConnectedFields.default)

#### [module redux-form.Field](#apidoc.module.redux-form.Field)
1.  [function <span class="apidocSignatureSpan">redux-form.Field.</span>default (_ref)](#apidoc.element.redux-form.Field.default)

#### [module redux-form.FieldArray](#apidoc.module.redux-form.FieldArray)
1.  [function <span class="apidocSignatureSpan">redux-form.FieldArray.</span>default (_ref2)](#apidoc.element.redux-form.FieldArray.default)

#### [module redux-form.Fields](#apidoc.module.redux-form.Fields)
1.  [function <span class="apidocSignatureSpan">redux-form.Fields.</span>default (_ref)](#apidoc.element.redux-form.Fields.default)

#### [module redux-form.Form](#apidoc.module.redux-form.Form)
1.  [function <span class="apidocSignatureSpan">redux-form.Form.</span>default (props, context)](#apidoc.element.redux-form.Form.default)

#### [module redux-form.FormSection](#apidoc.module.redux-form.FormSection)
1.  [function <span class="apidocSignatureSpan">redux-form.FormSection.</span>default (props, context)](#apidoc.element.redux-form.FormSection.default)

#### [module redux-form.SubmissionError](#apidoc.module.redux-form.SubmissionError)
1.  [function <span class="apidocSignatureSpan">redux-form.SubmissionError.</span>default (errors)](#apidoc.element.redux-form.SubmissionError.default)

#### [module redux-form.actions](#apidoc.module.redux-form.actions)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayInsert (form, field, index, value)](#apidoc.element.redux-form.actions.arrayInsert)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayMove (form, field, from, to)](#apidoc.element.redux-form.actions.arrayMove)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayPop (form, field)](#apidoc.element.redux-form.actions.arrayPop)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayPush (form, field, value)](#apidoc.element.redux-form.actions.arrayPush)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayRemove (form, field, index)](#apidoc.element.redux-form.actions.arrayRemove)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayRemoveAll (form, field)](#apidoc.element.redux-form.actions.arrayRemoveAll)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayShift (form, field)](#apidoc.element.redux-form.actions.arrayShift)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arraySplice (form, field, index, removeNum, value)](#apidoc.element.redux-form.actions.arraySplice)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arraySwap (form, field, indexA, indexB)](#apidoc.element.redux-form.actions.arraySwap)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayUnshift (form, field, value)](#apidoc.element.redux-form.actions.arrayUnshift)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>autofill (form, field, value)](#apidoc.element.redux-form.actions.autofill)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>blur (form, field, value, touch)](#apidoc.element.redux-form.actions.blur)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>change (form, field, value, touch, persistentSubmitErrors)](#apidoc.element.redux-form.actions.change)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>clearAsyncError (form, field)](#apidoc.element.redux-form.actions.clearAsyncError)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>clearSubmit (form)](#apidoc.element.redux-form.actions.clearSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>clearSubmitErrors (form)](#apidoc.element.redux-form.actions.clearSubmitErrors)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>destroy ()](#apidoc.element.redux-form.actions.destroy)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>focus (form, field)](#apidoc.element.redux-form.actions.focus)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>initialize (form, values, keepDirty)](#apidoc.element.redux-form.actions.initialize)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>registerField (form, name, type)](#apidoc.element.redux-form.actions.registerField)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>reset (form)](#apidoc.element.redux-form.actions.reset)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>setSubmitFailed (form)](#apidoc.element.redux-form.actions.setSubmitFailed)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>setSubmitSucceeded (form)](#apidoc.element.redux-form.actions.setSubmitSucceeded)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>startAsyncValidation (form, field)](#apidoc.element.redux-form.actions.startAsyncValidation)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>startSubmit (form)](#apidoc.element.redux-form.actions.startSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>stopAsyncValidation (form, errors)](#apidoc.element.redux-form.actions.stopAsyncValidation)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>stopSubmit (form, errors)](#apidoc.element.redux-form.actions.stopSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>submit (form)](#apidoc.element.redux-form.actions.submit)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>touch (form)](#apidoc.element.redux-form.actions.touch)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>unregisterField (form, name)](#apidoc.element.redux-form.actions.unregisterField)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>untouch (form)](#apidoc.element.redux-form.actions.untouch)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>updateSyncErrors (form)](#apidoc.element.redux-form.actions.updateSyncErrors)
1.  [function <span class="apidocSignatureSpan">redux-form.actions.</span>updateSyncWarnings (form)](#apidoc.element.redux-form.actions.updateSyncWarnings)

#### [module redux-form.asyncValidation](#apidoc.module.redux-form.asyncValidation)
1.  [function <span class="apidocSignatureSpan">redux-form.asyncValidation.</span>default (fn, start, stop, field)](#apidoc.element.redux-form.asyncValidation.default)

#### [module redux-form.createAll](#apidoc.module.redux-form.createAll)
1.  [function <span class="apidocSignatureSpan">redux-form.createAll.</span>default (structure)](#apidoc.element.redux-form.createAll.default)

#### [module redux-form.createFieldArrayProps](#apidoc.module.redux-form.createFieldArrayProps)
1.  [function <span class="apidocSignatureSpan">redux-form.createFieldArrayProps.</span>default (getIn, name, form, sectionPrefix, getValue, _ref)](#apidoc.element.redux-form.createFieldArrayProps.default)

#### [module redux-form.createFieldProps](#apidoc.module.redux-form.createFieldProps)
1.  [function <span class="apidocSignatureSpan">redux-form.createFieldProps.</span>default (_ref2, name, _ref)](#apidoc.element.redux-form.createFieldProps.default)

#### [module redux-form.defaultShouldAsyncValidate](#apidoc.module.redux-form.defaultShouldAsyncValidate)
1.  [function <span class="apidocSignatureSpan">redux-form.defaultShouldAsyncValidate.</span>default (_ref)](#apidoc.element.redux-form.defaultShouldAsyncValidate.default)

#### [module redux-form.defaultShouldValidate](#apidoc.module.redux-form.defaultShouldValidate)
1.  [function <span class="apidocSignatureSpan">redux-form.defaultShouldValidate.</span>default (_ref)](#apidoc.element.redux-form.defaultShouldValidate.default)

#### [module redux-form.deleteInWithCleanUp](#apidoc.module.redux-form.deleteInWithCleanUp)
1.  [function <span class="apidocSignatureSpan">redux-form.deleteInWithCleanUp.</span>default (_ref)](#apidoc.element.redux-form.deleteInWithCleanUp.default)

#### [module redux-form.formValueSelector](#apidoc.module.redux-form.formValueSelector)
1.  [function <span class="apidocSignatureSpan">redux-form.formValueSelector.</span>default (_ref)](#apidoc.element.redux-form.formValueSelector.default)

#### [module redux-form.generateValidator](#apidoc.module.redux-form.generateValidator)
1.  [function <span class="apidocSignatureSpan">redux-form.generateValidator.</span>default (validators, _ref)](#apidoc.element.redux-form.generateValidator.default)

#### [module redux-form.handleSubmit](#apidoc.module.redux-form.handleSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.handleSubmit.</span>default (submit, props, valid, asyncValidate, fields)](#apidoc.element.redux-form.handleSubmit.default)

#### [module redux-form.hasError](#apidoc.module.redux-form.hasError)
1.  [function <span class="apidocSignatureSpan">redux-form.hasError.</span>default (_ref)](#apidoc.element.redux-form.hasError.default)

#### [module redux-form.isChecked](#apidoc.module.redux-form.isChecked)
1.  [function <span class="apidocSignatureSpan">redux-form.isChecked.</span>default (value)](#apidoc.element.redux-form.isChecked.default)

#### [module redux-form.propTypes](#apidoc.module.redux-form.propTypes)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>anyTouched ()](#apidoc.element.redux-form.propTypes.anyTouched)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>array ()](#apidoc.element.redux-form.propTypes.array)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>asyncValidate ()](#apidoc.element.redux-form.propTypes.asyncValidate)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>asyncValidating ()](#apidoc.element.redux-form.propTypes.asyncValidating)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>autofill ()](#apidoc.element.redux-form.propTypes.autofill)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>blur ()](#apidoc.element.redux-form.propTypes.blur)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>change ()](#apidoc.element.redux-form.propTypes.change)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>clearAsyncError ()](#apidoc.element.redux-form.propTypes.clearAsyncError)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>clearSubmit ()](#apidoc.element.redux-form.propTypes.clearSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>destroy ()](#apidoc.element.redux-form.propTypes.destroy)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>dirty ()](#apidoc.element.redux-form.propTypes.dirty)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>dispatch ()](#apidoc.element.redux-form.propTypes.dispatch)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>error ()](#apidoc.element.redux-form.propTypes.error)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>form ()](#apidoc.element.redux-form.propTypes.form)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>handleSubmit ()](#apidoc.element.redux-form.propTypes.handleSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialValues ()](#apidoc.element.redux-form.propTypes.initialValues)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialize ()](#apidoc.element.redux-form.propTypes.initialize)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialized ()](#apidoc.element.redux-form.propTypes.initialized)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>invalid ()](#apidoc.element.redux-form.propTypes.invalid)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>pristine ()](#apidoc.element.redux-form.propTypes.pristine)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>pure ()](#apidoc.element.redux-form.propTypes.pure)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>reset ()](#apidoc.element.redux-form.propTypes.reset)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submit ()](#apidoc.element.redux-form.propTypes.submit)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submitFailed ()](#apidoc.element.redux-form.propTypes.submitFailed)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submitSucceeded ()](#apidoc.element.redux-form.propTypes.submitSucceeded)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submitting ()](#apidoc.element.redux-form.propTypes.submitting)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>touch ()](#apidoc.element.redux-form.propTypes.touch)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>triggerSubmit ()](#apidoc.element.redux-form.propTypes.triggerSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>untouch ()](#apidoc.element.redux-form.propTypes.untouch)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>valid ()](#apidoc.element.redux-form.propTypes.valid)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>warning ()](#apidoc.element.redux-form.propTypes.warning)

#### [module redux-form.propTypes.array](#apidoc.module.redux-form.propTypes.array)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>array ()](#apidoc.element.redux-form.propTypes.array.array)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.array.</span>isRequired ()](#apidoc.element.redux-form.propTypes.array.isRequired)

#### [module redux-form.propTypes.error](#apidoc.module.redux-form.propTypes.error)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>error ()](#apidoc.element.redux-form.propTypes.error.error)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.error.</span>isRequired ()](#apidoc.element.redux-form.propTypes.error.isRequired)

#### [module redux-form.propTypes.initialValues](#apidoc.module.redux-form.propTypes.initialValues)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialValues ()](#apidoc.element.redux-form.propTypes.initialValues.initialValues)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.initialValues.</span>isRequired ()](#apidoc.element.redux-form.propTypes.initialValues.isRequired)

#### [module redux-form.propTypes.triggerSubmit](#apidoc.module.redux-form.propTypes.triggerSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.</span>triggerSubmit ()](#apidoc.element.redux-form.propTypes.triggerSubmit.triggerSubmit)
1.  [function <span class="apidocSignatureSpan">redux-form.propTypes.triggerSubmit.</span>isRequired ()](#apidoc.element.redux-form.propTypes.triggerSubmit.isRequired)

#### [module redux-form.reducer](#apidoc.module.redux-form.reducer)
1.  [function <span class="apidocSignatureSpan">redux-form.</span>reducer ()](#apidoc.element.redux-form.reducer.reducer)
1.  [function <span class="apidocSignatureSpan">redux-form.reducer.</span>plugin (reducers)](#apidoc.element.redux-form.reducer.plugin)

#### [module redux-form.reduxForm](#apidoc.module.redux-form.reduxForm)
1.  [function <span class="apidocSignatureSpan">redux-form.reduxForm.</span>default (structure)](#apidoc.element.redux-form.reduxForm.default)

#### [module redux-form.values](#apidoc.module.redux-form.values)
1.  [function <span class="apidocSignatureSpan">redux-form.values.</span>default (_ref)](#apidoc.element.redux-form.values.default)



# <a name="apidoc.module.redux-form"></a>[module redux-form](#apidoc.module.redux-form)

#### <a name="apidoc.element.redux-form.Field"></a>[function <span class="apidocSignatureSpan">redux-form.</span>Field (props, context)](#apidoc.element.redux-form.Field)
- description and source-code
```javascript
function Field(props, context) {
  _classCallCheck(this, Field);

  var _this = _possibleConstructorReturn(this, (Field.__proto__ || Object.getPrototypeOf(Field)).call(this, props, context));

  if (!context._reduxForm) {
    throw new Error('Field must be inside a component decorated with reduxForm()');
  }

  _this.normalize = _this.normalize.bind(_this);
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.FieldArray"></a>[function <span class="apidocSignatureSpan">redux-form.</span>FieldArray (props, context)](#apidoc.element.redux-form.FieldArray)
- description and source-code
```javascript
function FieldArray(props, context) {
  _classCallCheck(this, FieldArray);

  var _this = _possibleConstructorReturn(this, (FieldArray.__proto__ || Object.getPrototypeOf(FieldArray)).call(this, props, context
));

  if (!context._reduxForm) {
    throw new Error('FieldArray must be inside a component decorated with reduxForm()');
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.Fields"></a>[function <span class="apidocSignatureSpan">redux-form.</span>Fields (props, context)](#apidoc.element.redux-form.Fields)
- description and source-code
```javascript
function Fields(props, context) {
  _classCallCheck(this, Fields);

  var _this = _possibleConstructorReturn(this, (Fields.__proto__ || Object.getPrototypeOf(Fields)).call(this, props, context));

  if (!context._reduxForm) {
    throw new Error('Fields must be inside a component decorated with reduxForm()');
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.Form"></a>[function <span class="apidocSignatureSpan">redux-form.</span>Form (props, context)](#apidoc.element.redux-form.Form)
- description and source-code
```javascript
function Form(props, context) {
  _classCallCheck(this, Form);

  var _this = _possibleConstructorReturn(this, (Form.__proto__ || Object.getPrototypeOf(Form)).call(this, props, context));

  if (!context._reduxForm) {
    throw new Error('Form must be inside a component decorated with reduxForm()');
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.FormSection"></a>[function <span class="apidocSignatureSpan">redux-form.</span>FormSection (props, context)](#apidoc.element.redux-form.FormSection)
- description and source-code
```javascript
function FormSection(props, context) {
  _classCallCheck(this, FormSection);

  var _this = _possibleConstructorReturn(this, (FormSection.__proto__ || Object.getPrototypeOf(FormSection)).call(this, props, context
));

  if (!context._reduxForm) {
    throw new Error('FormSection must be inside a component decorated with reduxForm()');
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.SubmissionError"></a>[function <span class="apidocSignatureSpan">redux-form.</span>SubmissionError (errors)](#apidoc.element.redux-form.SubmissionError)
- description and source-code
```javascript
function SubmissionError(errors) {
  _classCallCheck(this, SubmissionError);

  var _this = _possibleConstructorReturn(this, (SubmissionError.__proto__ || Object.getPrototypeOf(SubmissionError)).call(this, '
Submit Validation Failed'));

  _this.errors = errors;
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayInsert"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayInsert (form, field, index, value)](#apidoc.element.redux-form.arrayInsert)
- description and source-code
```javascript
function arrayInsert(form, field, index, value) {
  return { type: _actionTypes.ARRAY_INSERT, meta: { form: form, field: field, index: index }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayMove"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayMove (form, field, from, to)](#apidoc.element.redux-form.arrayMove)
- description and source-code
```javascript
function arrayMove(form, field, from, to) {
  return { type: _actionTypes.ARRAY_MOVE, meta: { form: form, field: field, from: from, to: to } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayPop"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayPop (form, field)](#apidoc.element.redux-form.arrayPop)
- description and source-code
```javascript
function arrayPop(form, field) {
  return { type: _actionTypes.ARRAY_POP, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayPush"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayPush (form, field, value)](#apidoc.element.redux-form.arrayPush)
- description and source-code
```javascript
function arrayPush(form, field, value) {
  return { type: _actionTypes.ARRAY_PUSH, meta: { form: form, field: field }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayRemove"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayRemove (form, field, index)](#apidoc.element.redux-form.arrayRemove)
- description and source-code
```javascript
function arrayRemove(form, field, index) {
  return { type: _actionTypes.ARRAY_REMOVE, meta: { form: form, field: field, index: index } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayRemoveAll"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayRemoveAll (form, field)](#apidoc.element.redux-form.arrayRemoveAll)
- description and source-code
```javascript
function arrayRemoveAll(form, field) {
  return { type: _actionTypes.ARRAY_REMOVE_ALL, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayShift"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayShift (form, field)](#apidoc.element.redux-form.arrayShift)
- description and source-code
```javascript
function arrayShift(form, field) {
  return { type: _actionTypes.ARRAY_SHIFT, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arraySplice"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arraySplice (form, field, index, removeNum, value)](#apidoc.element.redux-form.arraySplice)
- description and source-code
```javascript
function arraySplice(form, field, index, removeNum, value) {
  var action = {
    type: _actionTypes.ARRAY_SPLICE,
    meta: { form: form, field: field, index: index, removeNum: removeNum }
  };
  if (value !== undefined) {
    action.payload = value;
  }
  return action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arraySwap"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arraySwap (form, field, indexA, indexB)](#apidoc.element.redux-form.arraySwap)
- description and source-code
```javascript
function arraySwap(form, field, indexA, indexB) {
  if (indexA === indexB) {
    throw new Error('Swap indices cannot be equal');
  }
  if (indexA < 0 || indexB < 0) {
    throw new Error('Swap indices cannot be negative');
  }
  return { type: _actionTypes.ARRAY_SWAP, meta: { form: form, field: field, indexA: indexA, indexB: indexB } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.arrayUnshift"></a>[function <span class="apidocSignatureSpan">redux-form.</span>arrayUnshift (form, field, value)](#apidoc.element.redux-form.arrayUnshift)
- description and source-code
```javascript
function arrayUnshift(form, field, value) {
  return { type: _actionTypes.ARRAY_UNSHIFT, meta: { form: form, field: field }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.autofill"></a>[function <span class="apidocSignatureSpan">redux-form.</span>autofill (form, field, value)](#apidoc.element.redux-form.autofill)
- description and source-code
```javascript
function autofill(form, field, value) {
  return { type: _actionTypes.AUTOFILL, meta: { form: form, field: field }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.blur"></a>[function <span class="apidocSignatureSpan">redux-form.</span>blur (form, field, value, touch)](#apidoc.element.redux-form.blur)
- description and source-code
```javascript
function blur(form, field, value, touch) {
  return { type: _actionTypes.BLUR, meta: { form: form, field: field, touch: touch }, payload: value };
}
```
- example usage
```shell
...
        return event.preventDefault();
      }
    }), newValue, previousValue);
  }

  if (!defaultPrevented) {
    // dispatch blur action
    dispatch(_reduxForm.blur(name, newValue));

    // call post-blur callback
    if (_reduxForm.asyncValidate) {
      _reduxForm.asyncValidate(name, newValue);
    }
  }
}
...
```

#### <a name="apidoc.element.redux-form.change"></a>[function <span class="apidocSignatureSpan">redux-form.</span>change (form, field, value, touch, persistentSubmitErrors)](#apidoc.element.redux-form.change)
- description and source-code
```javascript
function change(form, field, value, touch, persistentSubmitErrors) {
  return { type: _actionTypes.CHANGE, meta: { form: form, field: field, touch: touch, persistentSubmitErrors: persistentSubmitErrors
 }, payload: value };
}
```
- example usage
```shell
...
          defaultPrevented = true;
          return event.preventDefault();
        }
      }), newValue, previousValue);
    }
    if (!defaultPrevented) {
      // dispatch change action
      dispatch(_reduxForm.change(name, newValue));
    }
  }
}, {
  key: 'handleFocus',
  value: function handleFocus(event) {
    var _props2 = this.props,
        name = _props2.name,
...
```

#### <a name="apidoc.element.redux-form.destroy"></a>[function <span class="apidocSignatureSpan">redux-form.</span>destroy ()](#apidoc.element.redux-form.destroy)
- description and source-code
```javascript
function destroy() {
  for (var _len = arguments.length, form = Array(_len), _key = 0; _key < _len; _key++) {
    form[_key] = arguments[_key];
  }

  return { type: _actionTypes.DESTROY, meta: { form: form } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.focus"></a>[function <span class="apidocSignatureSpan">redux-form.</span>focus (form, field)](#apidoc.element.redux-form.focus)
- description and source-code
```javascript
function focus(form, field) {
  return { type: _actionTypes.FOCUS, meta: { form: form, field: field } };
}
```
- example usage
```shell
...
          defaultPrevented = true;
          return event.preventDefault();
        }
      }));
    }

    if (!defaultPrevented) {
      dispatch(_reduxForm.focus(name));
    }
  }
}, {
  key: 'handleBlur',
  value: function handleBlur(event) {
    var _props3 = this.props,
        name = _props3.name,
...
```

#### <a name="apidoc.element.redux-form.formValueSelector"></a>[function <span class="apidocSignatureSpan">redux-form.</span>formValueSelector (form)](#apidoc.element.redux-form.formValueSelector)
- description and source-code
```javascript
formValueSelector = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };

  (0, _invariant2.default)(form, 'Form value must be specified');
  return function (state) {
    for (var _len = arguments.length, fields = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
      fields[_key - 1] = arguments[_key];
    }

    (0, _invariant2.default)(fields.length, 'No fields specified');
    return fields.length === 1 ?
    // only selecting one field, so return its value
    getIn(getFormState(state), form + '.values.' + fields[0]) :
    // selecting many fields, so return an object of field values
    fields.reduce(function (accumulator, field) {
      var value = getIn(getFormState(state), form + '.values.' + field);
      return value === undefined ? accumulator : _plain2.default.setIn(accumulator, field, value);
    }, {});
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.getFormAsyncErrors"></a>[function <span class="apidocSignatureSpan">redux-form.</span>getFormAsyncErrors (form)](#apidoc.element.redux-form.getFormAsyncErrors)
- description and source-code
```javascript
getFormAsyncErrors = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    return getIn(getFormState(state), form + '.asyncErrors');
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.getFormInitialValues"></a>[function <span class="apidocSignatureSpan">redux-form.</span>getFormInitialValues (form)](#apidoc.element.redux-form.getFormInitialValues)
- description and source-code
```javascript
getFormInitialValues = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    return getIn(getFormState(state), form + '.initial');
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.getFormNames"></a>[function <span class="apidocSignatureSpan">redux-form.</span>getFormNames ()](#apidoc.element.redux-form.getFormNames)
- description and source-code
```javascript
getFormNames = function () {
  var getFormState = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    return keys(getFormState(state));
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.getFormSubmitErrors"></a>[function <span class="apidocSignatureSpan">redux-form.</span>getFormSubmitErrors (form)](#apidoc.element.redux-form.getFormSubmitErrors)
- description and source-code
```javascript
getFormSubmitErrors = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    return getIn(getFormState(state), form + '.submitErrors');
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.getFormSyncErrors"></a>[function <span class="apidocSignatureSpan">redux-form.</span>getFormSyncErrors (form)](#apidoc.element.redux-form.getFormSyncErrors)
- description and source-code
```javascript
getFormSyncErrors = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    return getIn(getFormState(state), form + '.syncErrors');
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.getFormSyncWarnings"></a>[function <span class="apidocSignatureSpan">redux-form.</span>getFormSyncWarnings (form)](#apidoc.element.redux-form.getFormSyncWarnings)
- description and source-code
```javascript
getFormSyncWarnings = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    return getIn(getFormState(state), form + '.syncWarnings');
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.getFormValues"></a>[function <span class="apidocSignatureSpan">redux-form.</span>getFormValues (form)](#apidoc.element.redux-form.getFormValues)
- description and source-code
```javascript
getFormValues = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    return getIn(getFormState(state), form + '.values');
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.hasSubmitFailed"></a>[function <span class="apidocSignatureSpan">redux-form.</span>hasSubmitFailed (form)](#apidoc.element.redux-form.hasSubmitFailed)
- description and source-code
```javascript
hasSubmitFailed = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    var formState = getFormState(state);
    return getIn(formState, form + '.submitFailed') || false;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.hasSubmitSucceeded"></a>[function <span class="apidocSignatureSpan">redux-form.</span>hasSubmitSucceeded (form)](#apidoc.element.redux-form.hasSubmitSucceeded)
- description and source-code
```javascript
hasSubmitSucceeded = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    var formState = getFormState(state);
    return getIn(formState, form + '.submitSucceeded') || false;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.initialize"></a>[function <span class="apidocSignatureSpan">redux-form.</span>initialize (form, values, keepDirty)](#apidoc.element.redux-form.initialize)
- description and source-code
```javascript
function initialize(form, values, keepDirty) {
  var otherMeta = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

  if (keepDirty instanceof Object) {
    otherMeta = keepDirty;
    keepDirty = false;
  }
  return { type: _actionTypes.INITIALIZE, meta: _extends({ form: form, keepDirty: keepDirty }, otherMeta), payload: values };
}
```
- example usage
```shell
...
  key: 'initIfNeeded',
  value: function initIfNeeded(nextProps) {
    var enableReinitialize = this.props.enableReinitialize;

    if (nextProps) {
      if ((enableReinitialize || !nextProps.initialized) && !deepEqual(this.props.initialValues, nextProps.initialValues)) {
        var keepDirty = nextProps.initialized && this.props.keepDirtyOnReinitialize;
        this.props.initialize(nextProps.initialValues, keepDirty);
      }
    } else if (this.props.initialValues && (!this.props.initialized || enableReinitialize)) {
      this.props.initialize(this.props.initialValues, this.props.keepDirtyOnReinitialize);
    }
  }
}, {
  key: 'updateSyncErrorsIfNeeded',
...
```

#### <a name="apidoc.element.redux-form.isDirty"></a>[function <span class="apidocSignatureSpan">redux-form.</span>isDirty (form, getFormState)](#apidoc.element.redux-form.isDirty)
- description and source-code
```javascript
isDirty = function (form, getFormState) {
  var isPristine = (0, _isPristine2.default)(structure)(form, getFormState);
  return function (state) {
    return !isPristine(state);
  };
}
```
- example usage
```shell
...
    return this.props.names.map(function (name) {
      return (0, _prefixName2.default)(context, name);
    });
  }
}, {
  key: 'dirty',
  get: function get() {
    return this.refs.connected.getWrappedInstance().isDirty();
  }
}, {
  key: 'pristine',
  get: function get() {
    return !this.dirty;
  }
}, {
...
```

#### <a name="apidoc.element.redux-form.isInvalid"></a>[function <span class="apidocSignatureSpan">redux-form.</span>isInvalid (form, getFormState)](#apidoc.element.redux-form.isInvalid)
- description and source-code
```javascript
isInvalid = function (form, getFormState) {
  var isValid = (0, _isValid2.default)(structure)(form, getFormState);
  return function (state) {
    return !isValid(state);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.isPristine"></a>[function <span class="apidocSignatureSpan">redux-form.</span>isPristine (form)](#apidoc.element.redux-form.isPristine)
- description and source-code
```javascript
isPristine = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    var formState = getFormState(state);
    var initial = getIn(formState, form + '.initial') || empty;
    var values = getIn(formState, form + '.values') || initial;
    return deepEqual(initial, values);
  };
}
```
- example usage
```shell
...
  key: 'dirty',
  get: function get() {
    return !this.pristine;
  }
}, {
  key: 'pristine',
  get: function get() {
    return this.refs.connected.getWrappedInstance().isPristine();
  }
}, {
  key: 'value',
  get: function get() {
    return this.refs.connected && this.refs.connected.getWrappedInstance().getValue();
  }
}]);
...
```

#### <a name="apidoc.element.redux-form.isSubmitting"></a>[function <span class="apidocSignatureSpan">redux-form.</span>isSubmitting (form)](#apidoc.element.redux-form.isSubmitting)
- description and source-code
```javascript
isSubmitting = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  return function (state) {
    var formState = getFormState(state);
    return getIn(formState, form + '.submitting') || false;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.isValid"></a>[function <span class="apidocSignatureSpan">redux-form.</span>isValid (form)](#apidoc.element.redux-form.isValid)
- description and source-code
```javascript
isValid = function (form) {
  var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
    return getIn(state, 'form');
  };
  var ignoreSubmitErrors = arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : false;
  return function (state) {
    var formState = getFormState(state);
    var syncError = getIn(formState, form + '.syncError');
    if (syncError) {
      return false;
    }
    if (!ignoreSubmitErrors) {
      var error = getIn(formState, form + '.error');
      if (error) {
        return false;
      }
    }
    var syncErrors = getIn(formState, form + '.syncErrors');
    var asyncErrors = getIn(formState, form + '.asyncErrors');
    var submitErrors = ignoreSubmitErrors ? undefined : getIn(formState, form + '.submitErrors');
    if (!syncErrors && !asyncErrors && !submitErrors) {
      return true;
    }

    var registeredFields = getIn(formState, form + '.registeredFields');
    if (!registeredFields) {
      return true;
    }

    return !keys(registeredFields).filter(function (name) {
      return getIn(registeredFields, '[\'' + name + '\'].count') > 0;
    }).some(function (name) {
      return hasError(getIn(registeredFields, '[\'' + name + '\']'), syncErrors, asyncErrors, submitErrors);
    });
  };
}
```
- example usage
```shell
...
      // convert initialValues if need to
      initialValues: fromJS(initialValues)
    }));
  }
}, {
  key: 'valid',
  get: function get() {
    return this.refs.wrapped.getWrappedInstance().isValid();
  }
}, {
  key: 'invalid',
  get: function get() {
    return !this.valid;
  }
}, {
...
```

#### <a name="apidoc.element.redux-form.propTypes.array"></a>[function <span class="apidocSignatureSpan">redux-form.</span>propTypes.array ()](#apidoc.element.redux-form.propTypes.array)
- description and source-code
```javascript
propTypes.array = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.error"></a>[function <span class="apidocSignatureSpan">redux-form.</span>propTypes.error ()](#apidoc.element.redux-form.propTypes.error)
- description and source-code
```javascript
propTypes.error = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.initialValues"></a>[function <span class="apidocSignatureSpan">redux-form.</span>propTypes.initialValues ()](#apidoc.element.redux-form.propTypes.initialValues)
- description and source-code
```javascript
propTypes.initialValues = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.triggerSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.</span>propTypes.triggerSubmit ()](#apidoc.element.redux-form.propTypes.triggerSubmit)
- description and source-code
```javascript
propTypes.triggerSubmit = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.reducer"></a>[function <span class="apidocSignatureSpan">redux-form.</span>reducer ()](#apidoc.element.redux-form.reducer)
- description and source-code
```javascript
reducer = function () {
  var state = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : empty;
  var action = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  var form = action && action.meta && action.meta.form;
  if (!form) {
    return state;
  }
  if (action.type === _actionTypes.DESTROY) {
    return action.meta.form.reduce(function (result, form) {
      return deleteInWithCleanUp(result, form);
    }, state);
  }
  var formState = getIn(state, form);
  var result = reducer(formState, action);
  return result === formState ? state : setIn(state, form, result);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.reduxForm"></a>[function <span class="apidocSignatureSpan">redux-form.</span>reduxForm (initialConfig)](#apidoc.element.redux-form.reduxForm)
- description and source-code
```javascript
reduxForm = function (initialConfig) {
  var config = _extends({
    touchOnBlur: true,
    touchOnChange: false,
    persistentSubmitErrors: false,
    destroyOnUnmount: true,
    shouldAsyncValidate: _defaultShouldAsyncValidate2.default,
    shouldValidate: _defaultShouldValidate2.default,
    enableReinitialize: false,
    keepDirtyOnReinitialize: false,
    getFormState: function getFormState(state) {
      return getIn(state, 'form');
    },
    pure: true,
    forceUnregisterOnUnmount: false
  }, initialConfig);

  return function (WrappedComponent) {
    var Form = function (_Component) {
      _inherits(Form, _Component);

      function Form(props) {
        _classCallCheck(this, Form);

        var _this = _possibleConstructorReturn(this, (Form.__proto__ || Object.getPrototypeOf(Form)).call(this, props));

        _this.submit = _this.submit.bind(_this);
        _this.reset = _this.reset.bind(_this);
        _this.asyncValidate = _this.asyncValidate.bind(_this);
        _this.getValues = _this.getValues.bind(_this);
        _this.register = _this.register.bind(_this);
        _this.unregister = _this.unregister.bind(_this);
        _this.submitCompleted = _this.submitCompleted.bind(_this);
        _this.submitFailed = _this.submitFailed.bind(_this);
        _this.fieldValidators = {};
        _this.lastFieldValidatorKeys = [];
        _this.fieldWarners = {};
        _this.lastFieldWarnerKeys = [];
        return _this;
      }

      _createClass(Form, [{
        key: 'getChildContext',
        value: function getChildContext() {
          var _this2 = this;

          return {
            _reduxForm: _extends({}, this.props, {
              getFormState: function getFormState(state) {
                return getIn(_this2.props.getFormState(state), _this2.props.form);
              },
              asyncValidate: this.asyncValidate,
              getValues: this.getValues,
              sectionPrefix: undefined,
              register: this.register,
              unregister: this.unregister,
              registerInnerOnSubmit: function registerInnerOnSubmit(innerOnSubmit) {
                return _this2.innerOnSubmit = innerOnSubmit;
              }
            })
          };
        }
      }, {
        key: 'initIfNeeded',
        value: function initIfNeeded(nextProps) {
          var enableReinitialize = this.props.enableReinitialize;

          if (nextProps) {
            if ((enableReinitialize || !nextProps.initialized) && !deepEqual(this.props.initialValues, nextProps.initialValues)) {
              var keepDirty = nextProps.initialized && this.props.keepDirtyOnReinitialize;
              this.props.initialize(nextProps.initialValues, keepDirty);
            }
          } else if (this.props.initialValues && (!this.props.initialized || enableReinitialize)) {
            this.props.initialize(this.props.initialValues, this.props.keepDirtyOnReinitialize);
          }
        }
      }, {
        key: 'updateSyncErrorsIfNeeded',
        value: function updateSyncErrorsIfNeeded(nextSyncErrors, nextError) {
          var _props = this.props,
              error = _props.error,
              syncErrors = _props.syncErrors,
              updateSyncErrors = _props.updateSyncErrors;

          var noErrors = (!syncErrors || !Object.keys(syncErrors).length) && !error;
          var nextNoErrors = (!nextSyncErrors || !Object.keys(nextSyncErrors).length) && !nextError;
          if (!(noErrors && nextNoErrors) && (!_plain2.default.deepEqual(syncErrors, nextSyncErrors) || !_plain2.default.deepEqual
(error, nextError))) {
            updateSyncErrors(nextSyncErrors, nextError);
          }
        }
      }, {
        key: 'clearSubmitPromiseIfNeeded',
        value: function clearSubmitPromiseIfNeeded(nextProps) {
          var submitting = this.props.submitting;

          if (this.submitPromise && submitting && !nextProps.submitting) {
            delete this.submitPromise;
          }
        }
      }, {
        key: 'submitIfNeeded',
        value: function submitIfNeeded(nextProps) {
          var _props2 = this.props ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.registerField"></a>[function <span class="apidocSignatureSpan">redux-form.</span>registerField (form, name, type)](#apidoc.element.redux-form.registerField)
- description and source-code
```javascript
function registerField(form, name, type) {
  return { type: _actionTypes.REGISTER_FIELD, meta: { form: form }, payload: { name: name, type: type } };
}
```
- example usage
```shell
...
  key: 'isPristine',
  value: function isPristine() {
    return this.props.pristine;
  }
}, {
  key: 'register',
  value: function register(name, type, getValidator, getWarner) {
    this.props.registerField(name, type);
    if (getValidator) {
      this.fieldValidators[name] = getValidator;
    }
    if (getWarner) {
      this.fieldWarners[name] = getWarner;
    }
  }
...
```

#### <a name="apidoc.element.redux-form.reset"></a>[function <span class="apidocSignatureSpan">redux-form.</span>reset (form)](#apidoc.element.redux-form.reset)
- description and source-code
```javascript
function reset(form) {
  return { type: _actionTypes.RESET, meta: { form: form } };
}
```
- example usage
```shell
...
        return !_this7.submitPromise && _this7.listenToSubmit((0, _handleSubmit2.default)(checkSubmit(submitOrEvent), _extends({},
_this7.props, (0, _redux.bindActionCreators)({ blur: blur, change: change }, dispatch)), validExceptSubmit, _this7.asyncValidate
, _this7.getFieldList({ excludeFieldArray: true })));
      });
    }
  }
}, {
  key: 'reset',
  value: function reset() {
    this.props.reset();
  }
}, {
  key: 'render',
  value: function render() {
    // remove some redux-form config-only props
    /* eslint-disable no-unused-vars */
    var _props9 = this.props,
...
```

#### <a name="apidoc.element.redux-form.setSubmitFailed"></a>[function <span class="apidocSignatureSpan">redux-form.</span>setSubmitFailed (form)](#apidoc.element.redux-form.setSubmitFailed)
- description and source-code
```javascript
function setSubmitFailed(form) {
  for (var _len2 = arguments.length, fields = Array(_len2 > 1 ? _len2 - 1 : 0), _key2 = 1; _key2 < _len2; _key2++) {
    fields[_key2 - 1] = arguments[_key2];
  }

  return { type: _actionTypes.SET_SUBMIT_FAILED, meta: { form: form, fields: fields }, error: true };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.setSubmitSucceeded"></a>[function <span class="apidocSignatureSpan">redux-form.</span>setSubmitSucceeded (form)](#apidoc.element.redux-form.setSubmitSucceeded)
- description and source-code
```javascript
function setSubmitSucceeded(form) {
  for (var _len3 = arguments.length, fields = Array(_len3 > 1 ? _len3 - 1 : 0), _key3 = 1; _key3 < _len3; _key3++) {
    fields[_key3 - 1] = arguments[_key3];
  }

  return { type: _actionTypes.SET_SUBMIT_SUCCEEDED, meta: { form: form, fields: fields }, error: false };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.startAsyncValidation"></a>[function <span class="apidocSignatureSpan">redux-form.</span>startAsyncValidation (form, field)](#apidoc.element.redux-form.startAsyncValidation)
- description and source-code
```javascript
function startAsyncValidation(form, field) {
  return { type: _actionTypes.START_ASYNC_VALIDATION, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.startSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.</span>startSubmit (form)](#apidoc.element.redux-form.startSubmit)
- description and source-code
```javascript
function startSubmit(form) {
  return { type: _actionTypes.START_SUBMIT, meta: { form: form } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.stopAsyncValidation"></a>[function <span class="apidocSignatureSpan">redux-form.</span>stopAsyncValidation (form, errors)](#apidoc.element.redux-form.stopAsyncValidation)
- description and source-code
```javascript
function stopAsyncValidation(form, errors) {
  var action = {
    type: _actionTypes.STOP_ASYNC_VALIDATION,
    meta: { form: form },
    payload: errors
  };
  if (errors && Object.keys(errors).length) {
    action.error = true;
  }
  return action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.stopSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.</span>stopSubmit (form, errors)](#apidoc.element.redux-form.stopSubmit)
- description and source-code
```javascript
function stopSubmit(form, errors) {
  var action = {
    type: _actionTypes.STOP_SUBMIT,
    meta: { form: form },
    payload: errors
  };
  if (errors && Object.keys(errors).length) {
    action.error = true;
  }
  return action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.submit"></a>[function <span class="apidocSignatureSpan">redux-form.</span>submit (form)](#apidoc.element.redux-form.submit)
- description and source-code
```javascript
function submit(form) {
  return { type: _actionTypes.SUBMIT, meta: { form: form } };
}
```
- example usage
```shell
...
  value: function submitIfNeeded(nextProps) {
    var _props2 = this.props,
        clearSubmit = _props2.clearSubmit,
        triggerSubmit = _props2.triggerSubmit;

    if (!triggerSubmit && nextProps.triggerSubmit) {
      clearSubmit();
      this.submit();
    }
  }
}, {
  key: 'validateIfNeeded',
  value: function validateIfNeeded(nextProps) {
    var _props3 = this.props,
        shouldValidate = _props3.shouldValidate,
...
```

#### <a name="apidoc.element.redux-form.touch"></a>[function <span class="apidocSignatureSpan">redux-form.</span>touch (form)](#apidoc.element.redux-form.touch)
- description and source-code
```javascript
function touch(form) {
  for (var _len4 = arguments.length, fields = Array(_len4 > 1 ? _len4 - 1 : 0), _key4 = 1; _key4 < _len4; _key4++) {
    fields[_key4 - 1] = arguments[_key4];
  }

  return { type: _actionTypes.TOUCH, meta: { form: form, fields: fields } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.unregisterField"></a>[function <span class="apidocSignatureSpan">redux-form.</span>unregisterField (form, name)](#apidoc.element.redux-form.unregisterField)
- description and source-code
```javascript
function unregisterField(form, name) {
  var destroyOnUnmount = arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : true;
  return { type: _actionTypes.UNREGISTER_FIELD, meta: { form: form }, payload: { name: name, destroyOnUnmount: destroyOnUnmount } };
}
```
- example usage
```shell
...
    }
  }
}, {
  key: 'unregister',
  value: function unregister(name) {
    if (!this.destroyed) {
      if (this.props.destroyOnUnmount || this.props.forceUnregisterOnUnmount) {
        this.props.unregisterField(name);
        delete this.fieldValidators[name];
        delete this.fieldWarners[name];
      } else {
        this.props.unregisterField(name, false);
      }
    }
  }
...
```

#### <a name="apidoc.element.redux-form.untouch"></a>[function <span class="apidocSignatureSpan">redux-form.</span>untouch (form)](#apidoc.element.redux-form.untouch)
- description and source-code
```javascript
function untouch(form) {
  for (var _len5 = arguments.length, fields = Array(_len5 > 1 ? _len5 - 1 : 0), _key5 = 1; _key5 < _len5; _key5++) {
    fields[_key5 - 1] = arguments[_key5];
  }

  return { type: _actionTypes.UNTOUCH, meta: { form: form, fields: fields } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.values"></a>[function <span class="apidocSignatureSpan">redux-form.</span>values (config)](#apidoc.element.redux-form.values)
- description and source-code
```javascript
values = function (config) {
  var _prop$getFormState$co = _extends({
    prop: 'values',
    getFormState: function getFormState(state) {
      return getIn(state, 'form');
    }
  }, config),
      form = _prop$getFormState$co.form,
      prop = _prop$getFormState$co.prop,
      getFormState = _prop$getFormState$co.getFormState;

  return (0, _reactRedux.connect)(function (state) {
    return _defineProperty({}, prop, getIn(getFormState(state), form + '.values'));
  }, function () {
    return {};
  } // ignore dispatch
  );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.ConnectedField"></a>[module redux-form.ConnectedField](#apidoc.module.redux-form.ConnectedField)

#### <a name="apidoc.element.redux-form.ConnectedField.default"></a>[function <span class="apidocSignatureSpan">redux-form.ConnectedField.</span>default (_ref)](#apidoc.element.redux-form.ConnectedField.default)
- description and source-code
```javascript
function createConnectedField(_ref) {
  var deepEqual = _ref.deepEqual,
      getIn = _ref.getIn,
      toJS = _ref.toJS;


  var getSyncError = function getSyncError(syncErrors, name) {
    var error = getIn(syncErrors, name);
    // Because the error for this field might not be at a level in the error structure where
    // it can be set directly, it might need to be unwrapped from the _error property
    return error && error._error ? error._error : error;
  };

  var getSyncWarning = function getSyncWarning(syncWarnings, name) {
    var warning = getIn(syncWarnings, name);
    // Because the warning for this field might not be at a level in the warning structure where
    // it can be set directly, it might need to be unwrapped from the _warning property
    return warning && warning._warning ? warning._warning : warning;
  };

  var ConnectedField = function (_Component) {
    _inherits(ConnectedField, _Component);

    function ConnectedField(props) {
      _classCallCheck(this, ConnectedField);

      var _this = _possibleConstructorReturn(this, (ConnectedField.__proto__ || Object.getPrototypeOf(ConnectedField)).call(this
, props));

      _this.handleChange = _this.handleChange.bind(_this);
      _this.handleFocus = _this.handleFocus.bind(_this);
      _this.handleBlur = _this.handleBlur.bind(_this);
      _this.handleDragStart = _this.handleDragStart.bind(_this);
      _this.handleDrop = _this.handleDrop.bind(_this);
      return _this;
    }

    _createClass(ConnectedField, [{
      key: 'shouldComponentUpdate',
      value: function shouldComponentUpdate(nextProps) {
        var _this2 = this;

        var nextPropsKeys = Object.keys(nextProps);
        var thisPropsKeys = Object.keys(this.props);
        return nextPropsKeys.length !== thisPropsKeys.length || nextPropsKeys.some(function (prop) {
          return !~propsToNotUpdateFor.indexOf(prop) && !deepEqual(_this2.props[prop], nextProps[prop]);
        });
      }
    }, {
      key: 'isPristine',
      value: function isPristine() {
        return this.props.pristine;
      }
    }, {
      key: 'getValue',
      value: function getValue() {
        return this.props.value;
      }
    }, {
      key: 'getRenderedComponent',
      value: function getRenderedComponent() {
        return this.refs.renderedComponent;
      }
    }, {
      key: 'handleChange',
      value: function handleChange(event) {
        var _props = this.props,
            name = _props.name,
            dispatch = _props.dispatch,
            parse = _props.parse,
            normalize = _props.normalize,
            onChange = _props.onChange,
            _reduxForm = _props._reduxForm,
            previousValue = _props.value;

        var newValue = (0, _onChangeValue2.default)(event, { name: name, parse: parse, normalize: normalize });

        var defaultPrevented = false;
        if (onChange) {
          onChange(_extends({}, event, {
            preventDefault: function preventDefault() {
              defaultPrevented = true;
              return event.preventDefault();
            }
          }), newValue, previousValue);
        }
        if (!defaultPrevented) {
          // dispatch change action
          dispatch(_reduxForm.change(name, newValue));
        }
      }
    }, {
      key: 'handleFocus',
      value: function handleFocus(event) {
        var _props2 = this.props,
            name = _props2.name,
            dispatch = _props2.dispatch,
            onFocus = _props2.onFocus,
            _reduxForm = _props2._reduxForm;


        var defaultPrevented = false;
        if (onFocus) {
          onFocus(_extends({}, event, {
            preventDefault: function preventDefault() {
              defaultPrevented = true;
              return event.preventDefault();
            }
          }));
        }

        if (!defaultPrevented) {
          dispatch(_reduxForm.focus(name));
        }
      }
    }, {
      key: 'handleBlur',
      value: function handleBlur(event) {
        var _props3 = this.props,
            name = _props3.name,
            dispatch = _ ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.ConnectedFieldArray"></a>[module redux-form.ConnectedFieldArray](#apidoc.module.redux-form.ConnectedFieldArray)

#### <a name="apidoc.element.redux-form.ConnectedFieldArray.default"></a>[function <span class="apidocSignatureSpan">redux-form.ConnectedFieldArray.</span>default (_ref)](#apidoc.element.redux-form.ConnectedFieldArray.default)
- description and source-code
```javascript
function createConnectedFieldArray(_ref) {
  var deepEqual = _ref.deepEqual,
      getIn = _ref.getIn,
      size = _ref.size;


  var getSyncError = function getSyncError(syncErrors, name) {
    // For an array, the error can _ONLY_ be under _error.
    // This is why this getSyncError is not the same as the
    // one in Field.
    return getIn(syncErrors, name + '._error');
  };

  var getSyncWarning = function getSyncWarning(syncWarnings, name) {
    // For an array, the warning can _ONLY_ be under _warning.
    // This is why this getSyncError is not the same as the
    // one in Field.
    return getIn(syncWarnings, name + '._warning');
  };

  var ConnectedFieldArray = function (_Component) {
    _inherits(ConnectedFieldArray, _Component);

    function ConnectedFieldArray() {
      _classCallCheck(this, ConnectedFieldArray);

      var _this = _possibleConstructorReturn(this, (ConnectedFieldArray.__proto__ || Object.getPrototypeOf(ConnectedFieldArray)).
call(this));

      _this.getValue = _this.getValue.bind(_this);
      return _this;
    }

    _createClass(ConnectedFieldArray, [{
      key: 'shouldComponentUpdate',
      value: function shouldComponentUpdate(nextProps) {
        var _this2 = this;

        // Update if the elements of the value array was updated.
        var thisValue = this.props.value;
        var nextValue = nextProps.value;

        if (thisValue && nextValue) {
          if (thisValue.length !== nextValue.length || thisValue.every(function (val) {
            return nextValue.some(function (next) {
              return deepEqual(val, next);
            });
          })) {
            return true;
          }
        }

        var nextPropsKeys = Object.keys(nextProps);
        var thisPropsKeys = Object.keys(this.props);
        return nextPropsKeys.length !== thisPropsKeys.length || nextPropsKeys.some(function (prop) {
          // useful to debug rerenders
          // if (!plain.deepEqual(this.props[ prop ], nextProps[ prop ])) {
          //   console.info(prop, 'changed', this.props[ prop ], '==>', nextProps[ prop ])
          // }
          return !~propsToNotUpdateFor.indexOf(prop) && !deepEqual(_this2.props[prop], nextProps[prop]);
        });
      }
    }, {
      key: 'getRenderedComponent',
      value: function getRenderedComponent() {
        return this.refs.renderedComponent;
      }
    }, {
      key: 'getValue',
      value: function getValue(index) {
        return this.props.value && getIn(this.props.value, index);
      }
    }, {
      key: 'render',
      value: function render() {
        var _props = this.props,
            component = _props.component,
            withRef = _props.withRef,
            name = _props.name,
            _reduxForm = _props._reduxForm,
            validate = _props.validate,
            warn = _props.warn,
            rest = _objectWithoutProperties(_props, ['component', 'withRef', 'name', '_reduxForm', 'validate', 'warn']);

        var props = (0, _createFieldArrayProps2.default)(getIn, name, _reduxForm.form, _reduxForm.sectionPrefix, this.getValue,
rest);
        if (withRef) {
          props.ref = 'renderedComponent';
        }
        return (0, _react.createElement)(component, props);
      }
    }, {
      key: 'dirty',
      get: function get() {
        return this.props.dirty;
      }
    }, {
      key: 'pristine',
      get: function get() {
        return this.props.pristine;
      }
    }, {
      key: 'value',
      get: function get() {
        return this.props.value;
      }
    }]);

    return ConnectedFieldArray;
  }(_react.Component);

  ConnectedFieldArray.propTypes = {
    component: _react.PropTypes.oneOfType([_react.PropTypes.func, _react.PropTypes.string]).isRequired,
    props: _react.PropTypes.object
  };

  ConnectedFieldArray.contextTypes = {
    _reduxForm: _react.PropTypes.object
  };

  var connector = (0, _reactRedux.connect)(function (state, ownProps) {
    var name = ownProps.name,
        _ownProps$_reduxForm = ownProps._reduxForm,
        initialValues = _ownProps$_reduxForm.initialValues, ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.ConnectedFields"></a>[module redux-form.ConnectedFields](#apidoc.module.redux-form.ConnectedFields)

#### <a name="apidoc.element.redux-form.ConnectedFields.default"></a>[function <span class="apidocSignatureSpan">redux-form.ConnectedFields.</span>default (_ref)](#apidoc.element.redux-form.ConnectedFields.default)
- description and source-code
```javascript
function createConnectedFields(_ref) {
  var deepEqual = _ref.deepEqual,
      getIn = _ref.getIn,
      toJS = _ref.toJS,
      size = _ref.size;


  var getSyncError = function getSyncError(syncErrors, name) {
    var error = getIn(syncErrors, name);
    // Because the error for this field might not be at a level in the error structure where
    // it can be set directly, it might need to be unwrapped from the _error property
    return error && error._error ? error._error : error;
  };

  var getSyncWarning = function getSyncWarning(syncWarnings, name) {
    var warning = getIn(syncWarnings, name);
    // Because the warning for this field might not be at a level in the warning structure where
    // it can be set directly, it might need to be unwrapped from the _warning property
    return warning && warning._warning ? warning._warning : warning;
  };

  var ConnectedFields = function (_Component) {
    _inherits(ConnectedFields, _Component);

    function ConnectedFields(props) {
      _classCallCheck(this, ConnectedFields);

      var _this = _possibleConstructorReturn(this, (ConnectedFields.__proto__ || Object.getPrototypeOf(ConnectedFields)).call(this
, props));

      _this.handleChange = _this.handleChange.bind(_this);
      _this.handleFocus = _this.handleFocus.bind(_this);
      _this.handleBlur = _this.handleBlur.bind(_this);

      _this.onChangeFns = props.names.reduce(function (acc, name) {
        acc[name] = function (event) {
          return _this.handleChange(name, event);
        };
        return acc;
      }, {});

      _this.onFocusFns = props.names.reduce(function (acc, name) {
        acc[name] = function () {
          return _this.handleFocus(name);
        };
        return acc;
      }, {});

      _this.onBlurFns = props.names.reduce(function (acc, name) {
        acc[name] = function (event) {
          return _this.handleBlur(name, event);
        };
        return acc;
      }, {});
      return _this;
    }

    _createClass(ConnectedFields, [{
      key: 'componentWillReceiveProps',
      value: function componentWillReceiveProps(nextProps) {
        var _this2 = this;

        if (this.props.names !== nextProps.names && (size(this.props.names) !== size(nextProps.names) || nextProps.names.some(function
 (nextName) {
          return !_this2.props._fields[nextName];
        }))) {

          // names is changed. The cached event handlers need to be updated
          this.onChangeFns = nextProps.names.reduce(function (acc, name) {
            acc[name] = function (event) {
              return _this2.handleChange(name, event);
            };
            return acc;
          }, {});

          this.onFocusFns = nextProps.names.reduce(function (acc, name) {
            acc[name] = function () {
              return _this2.handleFocus(name);
            };
            return acc;
          }, {});

          this.onBlurFns = nextProps.names.reduce(function (acc, name) {
            acc[name] = function (event) {
              return _this2.handleBlur(name, event);
            };
            return acc;
          }, {});
        }
      }
    }, {
      key: 'shouldComponentUpdate',
      value: function shouldComponentUpdate(nextProps) {
        var _this3 = this;

        var nextPropsKeys = Object.keys(nextProps);
        var thisPropsKeys = Object.keys(this.props);
        return nextPropsKeys.length !== thisPropsKeys.length || nextPropsKeys.some(function (prop) {
          return !~propsToNotUpdateFor.indexOf(prop) && !deepEqual(_this3.props[prop], nextProps[prop]);
        });
      }
    }, {
      key: 'isDirty',
      value: function isDirty() {
        var _fields = this.props._fields;

        return Object.keys(_fields).some(function (name) {
          return _fields[name].dirty;
        });
      }
    }, {
      key: 'getValues',
      value: function getValues() {
        var _fields = this.props._fields;

        return Object.keys(_fields).reduce(function (accumulator, name) {
          return _plain2.default.setIn(accumulator, name, _fields[name].value);
        }, {}); ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.Field"></a>[module redux-form.Field](#apidoc.module.redux-form.Field)

#### <a name="apidoc.element.redux-form.Field.default"></a>[function <span class="apidocSignatureSpan">redux-form.Field.</span>default (_ref)](#apidoc.element.redux-form.Field.default)
- description and source-code
```javascript
function createField(_ref) {
  var deepEqual = _ref.deepEqual,
      getIn = _ref.getIn,
      setIn = _ref.setIn,
      toJS = _ref.toJS;


  var ConnectedField = (0, _ConnectedField2.default)({
    deepEqual: deepEqual,
    getIn: getIn,
    toJS: toJS
  });

  var Field = function (_Component) {
    _inherits(Field, _Component);

    function Field(props, context) {
      _classCallCheck(this, Field);

      var _this = _possibleConstructorReturn(this, (Field.__proto__ || Object.getPrototypeOf(Field)).call(this, props, context));

      if (!context._reduxForm) {
        throw new Error('Field must be inside a component decorated with reduxForm()');
      }

      _this.normalize = _this.normalize.bind(_this);
      return _this;
    }

    _createClass(Field, [{
      key: 'shouldComponentUpdate',
      value: function shouldComponentUpdate(nextProps, nextState) {
        return (0, _shallowCompare2.default)(this, nextProps, nextState);
      }
    }, {
      key: 'componentWillMount',
      value: function componentWillMount() {
        var _this2 = this;

        this.context._reduxForm.register(this.name, 'Field', function () {
          return _this2.props.validate;
        }, function () {
          return _this2.props.warn;
        });
      }
    }, {
      key: 'componentWillReceiveProps',
      value: function componentWillReceiveProps(nextProps) {
        if (this.props.name !== nextProps.name) {
          // unregister old name
          this.context._reduxForm.unregister(this.name);
          // register new name
          this.context._reduxForm.register((0, _prefixName2.default)(this.context, nextProps.name), 'Field');
        }
      }
    }, {
      key: 'componentWillUnmount',
      value: function componentWillUnmount() {
        this.context._reduxForm.unregister(this.name);
      }
    }, {
      key: 'getRenderedComponent',
      value: function getRenderedComponent() {
        (0, _invariant2.default)(this.props.withRef, 'If you want to access getRenderedComponent(), ' + 'you must specify a withRef
 prop to Field');
        return this.refs.connected.getWrappedInstance().getRenderedComponent();
      }
    }, {
      key: 'normalize',
      value: function normalize(name, value) {
        var normalize = this.props.normalize;

        if (!normalize) {
          return value;
        }
        var previousValues = this.context._reduxForm.getValues();
        var previousValue = this.value;
        var nextValues = setIn(previousValues, name, value);
        return normalize(value, previousValue, nextValues, previousValues);
      }
    }, {
      key: 'render',
      value: function render() {
        return (0, _react.createElement)(ConnectedField, _extends({}, this.props, {
          name: this.name,
          normalize: this.normalize,
          _reduxForm: this.context._reduxForm,
          ref: 'connected'
        }));
      }
    }, {
      key: 'name',
      get: function get() {
        return (0, _prefixName2.default)(this.context, this.props.name);
      }
    }, {
      key: 'dirty',
      get: function get() {
        return !this.pristine;
      }
    }, {
      key: 'pristine',
      get: function get() {
        return this.refs.connected.getWrappedInstance().isPristine();
      }
    }, {
      key: 'value',
      get: function get() {
        return this.refs.connected && this.refs.connected.getWrappedInstance().getValue();
      }
    }]);

    return Field;
  }(_react.Component);

  Field.propTypes = {
    name: _react.PropTypes.string.isRequired,
    component: _react.PropTypes.oneOfType([_react.PropTypes.func, _react.PropTypes.string]).isRequired,
    format: _react.PropTypes.func,
    normalize: _react.PropTypes.func,
    onBlur: _react.PropTypes.func,
    onChange: _react.PropTypes.func,
    onFocus: _react.PropTypes.func,
    onDragStart: _react.PropTypes.func,
    onDrop: _react.PropTypes.func,
    parse: _react.PropTypes.func,
    props: _react.PropTypes.object,
    validate: _react.PropTypes.oneOfType([_react.PropTypes.func, _react.PropTypes.arrayOf(_react.PropTypes.fu ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.FieldArray"></a>[module redux-form.FieldArray](#apidoc.module.redux-form.FieldArray)

#### <a name="apidoc.element.redux-form.FieldArray.default"></a>[function <span class="apidocSignatureSpan">redux-form.FieldArray.</span>default (_ref2)](#apidoc.element.redux-form.FieldArray.default)
- description and source-code
```javascript
function createFieldArray(_ref2) {
  var deepEqual = _ref2.deepEqual,
      getIn = _ref2.getIn,
      size = _ref2.size;


  var ConnectedFieldArray = (0, _ConnectedFieldArray2.default)({ deepEqual: deepEqual, getIn: getIn, size: size });

  var FieldArray = function (_Component) {
    _inherits(FieldArray, _Component);

    function FieldArray(props, context) {
      _classCallCheck(this, FieldArray);

      var _this = _possibleConstructorReturn(this, (FieldArray.__proto__ || Object.getPrototypeOf(FieldArray)).call(this, props,
context));

      if (!context._reduxForm) {
        throw new Error('FieldArray must be inside a component decorated with reduxForm()');
      }
      return _this;
    }

    _createClass(FieldArray, [{
      key: 'shouldComponentUpdate',
      value: function shouldComponentUpdate(nextProps, nextState) {
        return (0, _shallowCompare2.default)(this, nextProps, nextState);
      }
    }, {
      key: 'componentWillMount',
      value: function componentWillMount() {
        var _this2 = this;

        this.context._reduxForm.register(this.name, 'FieldArray', function () {
          return wrapError(_this2.props.validate, '_error');
        }, function () {
          return wrapError(_this2.props.warn, '_warning');
        });
      }
    }, {
      key: 'componentWillReceiveProps',
      value: function componentWillReceiveProps(nextProps) {
        if (this.props.name !== nextProps.name) {
          // unregister old name
          this.context._reduxForm.unregister(this.name);
          // register new name
          this.context._reduxForm.register((0, _prefixName2.default)(this.context, nextProps.name), 'FieldArray');
        }
      }
    }, {
      key: 'componentWillUnmount',
      value: function componentWillUnmount() {
        this.context._reduxForm.unregister(this.name);
      }
    }, {
      key: 'getRenderedComponent',
      value: function getRenderedComponent() {
        (0, _invariant2.default)(this.props.withRef, 'If you want to access getRenderedComponent(), ' + 'you must specify a withRef
 prop to FieldArray');
        return this.refs.connected.getWrappedInstance().getRenderedComponent();
      }
    }, {
      key: 'render',
      value: function render() {
        return (0, _react.createElement)(ConnectedFieldArray, _extends({}, this.props, {
          name: this.name,
          syncError: this.syncError,
          syncWarning: this.syncWarning,
          _reduxForm: this.context._reduxForm,
          ref: 'connected'
        }));
      }
    }, {
      key: 'name',
      get: function get() {
        return (0, _prefixName2.default)(this.context, this.props.name);
      }
    }, {
      key: 'dirty',
      get: function get() {
        return this.refs.connected.getWrappedInstance().dirty;
      }
    }, {
      key: 'pristine',
      get: function get() {
        return this.refs.connected.getWrappedInstance().pristine;
      }
    }, {
      key: 'value',
      get: function get() {
        return this.refs.connected.getWrappedInstance().value;
      }
    }]);

    return FieldArray;
  }(_react.Component);

  FieldArray.propTypes = {
    name: _react.PropTypes.string.isRequired,
    component: _react.PropTypes.func.isRequired,
    props: _react.PropTypes.object,
    validate: _react.PropTypes.func,
    warn: _react.PropTypes.func,
    withRef: _react.PropTypes.bool
  };
  FieldArray.contextTypes = {
    _reduxForm: _react.PropTypes.object
  };

  return FieldArray;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.Fields"></a>[module redux-form.Fields](#apidoc.module.redux-form.Fields)

#### <a name="apidoc.element.redux-form.Fields.default"></a>[function <span class="apidocSignatureSpan">redux-form.Fields.</span>default (_ref)](#apidoc.element.redux-form.Fields.default)
- description and source-code
```javascript
function createFields(_ref) {
  var deepEqual = _ref.deepEqual,
      getIn = _ref.getIn,
      toJS = _ref.toJS,
      size = _ref.size;


  var ConnectedFields = (0, _ConnectedFields2.default)({
    deepEqual: deepEqual,
    getIn: getIn,
    toJS: toJS,
    size: size
  });

  var Fields = function (_Component) {
    _inherits(Fields, _Component);

    function Fields(props, context) {
      _classCallCheck(this, Fields);

      var _this = _possibleConstructorReturn(this, (Fields.__proto__ || Object.getPrototypeOf(Fields)).call(this, props, context
));

      if (!context._reduxForm) {
        throw new Error('Fields must be inside a component decorated with reduxForm()');
      }
      return _this;
    }

    _createClass(Fields, [{
      key: 'shouldComponentUpdate',
      value: function shouldComponentUpdate(nextProps, nextState) {
        return (0, _shallowCompare2.default)(this, nextProps, nextState);
      }
    }, {
      key: 'componentWillMount',
      value: function componentWillMount() {
        var error = validateNameProp(this.props.names);
        if (error) {
          throw error;
        }
        var context = this.context;
        var register = context._reduxForm.register;

        this.names.forEach(function (name) {
          return register(name, 'Field');
        });
      }
    }, {
      key: 'componentWillReceiveProps',
      value: function componentWillReceiveProps(nextProps) {
        if (!_plain2.default.deepEqual(this.props.names, nextProps.names)) {
          var context = this.context;
          var _context$_reduxForm = context._reduxForm,
              register = _context$_reduxForm.register,
              unregister = _context$_reduxForm.unregister;
          // unregister old name

          this.props.names.forEach(function (name) {
            return unregister((0, _prefixName2.default)(context, name));
          });
          // register new name
          nextProps.names.forEach(function (name) {
            return register((0, _prefixName2.default)(context, name), 'Field');
          });
        }
      }
    }, {
      key: 'componentWillUnmount',
      value: function componentWillUnmount() {
        var context = this.context;
        var unregister = context._reduxForm.unregister;

        this.props.names.forEach(function (name) {
          return unregister((0, _prefixName2.default)(context, name));
        });
      }
    }, {
      key: 'getRenderedComponent',
      value: function getRenderedComponent() {
        (0, _invariant2.default)(this.props.withRef, 'If you want to access getRenderedComponent(), ' + 'you must specify a withRef
 prop to Fields');
        return this.refs.connected.getWrappedInstance().getRenderedComponent();
      }
    }, {
      key: 'render',
      value: function render() {
        var context = this.context;

        return (0, _react.createElement)(ConnectedFields, _extends({}, this.props, {
          names: this.props.names.map(function (name) {
            return (0, _prefixName2.default)(context, name);
          }),
          _reduxForm: this.context._reduxForm,
          ref: 'connected'
        }));
      }
    }, {
      key: 'names',
      get: function get() {
        var context = this.context;

        return this.props.names.map(function (name) {
          return (0, _prefixName2.default)(context, name);
        });
      }
    }, {
      key: 'dirty',
      get: function get() {
        return this.refs.connected.getWrappedInstance().isDirty();
      }
    }, {
      key: 'pristine',
      get: function get() {
        return !this.dirty;
      }
    }, {
      key: 'values',
      get: function get() {
        return this.refs.connected && this.refs.connected.getWrappedInstance().getValues();
      }
    }]);

    return Fields;
  }(_react.Component);

  Fields.propTypes = {
    names: function names(props, propName) {
      return validateNameProp(props[propName]);
    },
    component: _react.PropTypes.oneOfType([_react.PropTypes.func, _react.PropTypes.string]).isRequired,
    format: _react.PropTypes.func,
    parse ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.Form"></a>[module redux-form.Form](#apidoc.module.redux-form.Form)

#### <a name="apidoc.element.redux-form.Form.default"></a>[function <span class="apidocSignatureSpan">redux-form.Form.</span>default (props, context)](#apidoc.element.redux-form.Form.default)
- description and source-code
```javascript
function Form(props, context) {
  _classCallCheck(this, Form);

  var _this = _possibleConstructorReturn(this, (Form.__proto__ || Object.getPrototypeOf(Form)).call(this, props, context));

  if (!context._reduxForm) {
    throw new Error('Form must be inside a component decorated with reduxForm()');
  }
  return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.FormSection"></a>[module redux-form.FormSection](#apidoc.module.redux-form.FormSection)

#### <a name="apidoc.element.redux-form.FormSection.default"></a>[function <span class="apidocSignatureSpan">redux-form.FormSection.</span>default (props, context)](#apidoc.element.redux-form.FormSection.default)
- description and source-code
```javascript
function FormSection(props, context) {
  _classCallCheck(this, FormSection);

  var _this = _possibleConstructorReturn(this, (FormSection.__proto__ || Object.getPrototypeOf(FormSection)).call(this, props, context
));

  if (!context._reduxForm) {
    throw new Error('FormSection must be inside a component decorated with reduxForm()');
  }
  return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.SubmissionError"></a>[module redux-form.SubmissionError](#apidoc.module.redux-form.SubmissionError)

#### <a name="apidoc.element.redux-form.SubmissionError.default"></a>[function <span class="apidocSignatureSpan">redux-form.SubmissionError.</span>default (errors)](#apidoc.element.redux-form.SubmissionError.default)
- description and source-code
```javascript
function SubmissionError(errors) {
  _classCallCheck(this, SubmissionError);

  var _this = _possibleConstructorReturn(this, (SubmissionError.__proto__ || Object.getPrototypeOf(SubmissionError)).call(this, '
Submit Validation Failed'));

  _this.errors = errors;
  return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.actions"></a>[module redux-form.actions](#apidoc.module.redux-form.actions)

#### <a name="apidoc.element.redux-form.actions.arrayInsert"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayInsert (form, field, index, value)](#apidoc.element.redux-form.actions.arrayInsert)
- description and source-code
```javascript
function arrayInsert(form, field, index, value) {
  return { type: _actionTypes.ARRAY_INSERT, meta: { form: form, field: field, index: index }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arrayMove"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayMove (form, field, from, to)](#apidoc.element.redux-form.actions.arrayMove)
- description and source-code
```javascript
function arrayMove(form, field, from, to) {
  return { type: _actionTypes.ARRAY_MOVE, meta: { form: form, field: field, from: from, to: to } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arrayPop"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayPop (form, field)](#apidoc.element.redux-form.actions.arrayPop)
- description and source-code
```javascript
function arrayPop(form, field) {
  return { type: _actionTypes.ARRAY_POP, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arrayPush"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayPush (form, field, value)](#apidoc.element.redux-form.actions.arrayPush)
- description and source-code
```javascript
function arrayPush(form, field, value) {
  return { type: _actionTypes.ARRAY_PUSH, meta: { form: form, field: field }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arrayRemove"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayRemove (form, field, index)](#apidoc.element.redux-form.actions.arrayRemove)
- description and source-code
```javascript
function arrayRemove(form, field, index) {
  return { type: _actionTypes.ARRAY_REMOVE, meta: { form: form, field: field, index: index } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arrayRemoveAll"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayRemoveAll (form, field)](#apidoc.element.redux-form.actions.arrayRemoveAll)
- description and source-code
```javascript
function arrayRemoveAll(form, field) {
  return { type: _actionTypes.ARRAY_REMOVE_ALL, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arrayShift"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayShift (form, field)](#apidoc.element.redux-form.actions.arrayShift)
- description and source-code
```javascript
function arrayShift(form, field) {
  return { type: _actionTypes.ARRAY_SHIFT, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arraySplice"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arraySplice (form, field, index, removeNum, value)](#apidoc.element.redux-form.actions.arraySplice)
- description and source-code
```javascript
function arraySplice(form, field, index, removeNum, value) {
  var action = {
    type: _actionTypes.ARRAY_SPLICE,
    meta: { form: form, field: field, index: index, removeNum: removeNum }
  };
  if (value !== undefined) {
    action.payload = value;
  }
  return action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arraySwap"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arraySwap (form, field, indexA, indexB)](#apidoc.element.redux-form.actions.arraySwap)
- description and source-code
```javascript
function arraySwap(form, field, indexA, indexB) {
  if (indexA === indexB) {
    throw new Error('Swap indices cannot be equal');
  }
  if (indexA < 0 || indexB < 0) {
    throw new Error('Swap indices cannot be negative');
  }
  return { type: _actionTypes.ARRAY_SWAP, meta: { form: form, field: field, indexA: indexA, indexB: indexB } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.arrayUnshift"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>arrayUnshift (form, field, value)](#apidoc.element.redux-form.actions.arrayUnshift)
- description and source-code
```javascript
function arrayUnshift(form, field, value) {
  return { type: _actionTypes.ARRAY_UNSHIFT, meta: { form: form, field: field }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.autofill"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>autofill (form, field, value)](#apidoc.element.redux-form.actions.autofill)
- description and source-code
```javascript
function autofill(form, field, value) {
  return { type: _actionTypes.AUTOFILL, meta: { form: form, field: field }, payload: value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.blur"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>blur (form, field, value, touch)](#apidoc.element.redux-form.actions.blur)
- description and source-code
```javascript
function blur(form, field, value, touch) {
  return { type: _actionTypes.BLUR, meta: { form: form, field: field, touch: touch }, payload: value };
}
```
- example usage
```shell
...
        return event.preventDefault();
      }
    }), newValue, previousValue);
  }

  if (!defaultPrevented) {
    // dispatch blur action
    dispatch(_reduxForm.blur(name, newValue));

    // call post-blur callback
    if (_reduxForm.asyncValidate) {
      _reduxForm.asyncValidate(name, newValue);
    }
  }
}
...
```

#### <a name="apidoc.element.redux-form.actions.change"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>change (form, field, value, touch, persistentSubmitErrors)](#apidoc.element.redux-form.actions.change)
- description and source-code
```javascript
function change(form, field, value, touch, persistentSubmitErrors) {
  return { type: _actionTypes.CHANGE, meta: { form: form, field: field, touch: touch, persistentSubmitErrors: persistentSubmitErrors
 }, payload: value };
}
```
- example usage
```shell
...
          defaultPrevented = true;
          return event.preventDefault();
        }
      }), newValue, previousValue);
    }
    if (!defaultPrevented) {
      // dispatch change action
      dispatch(_reduxForm.change(name, newValue));
    }
  }
}, {
  key: 'handleFocus',
  value: function handleFocus(event) {
    var _props2 = this.props,
        name = _props2.name,
...
```

#### <a name="apidoc.element.redux-form.actions.clearAsyncError"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>clearAsyncError (form, field)](#apidoc.element.redux-form.actions.clearAsyncError)
- description and source-code
```javascript
function clearAsyncError(form, field) {
  return { type: _actionTypes.CLEAR_ASYNC_ERROR, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.clearSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>clearSubmit (form)](#apidoc.element.redux-form.actions.clearSubmit)
- description and source-code
```javascript
function clearSubmit(form) {
  return { type: _actionTypes.CLEAR_SUBMIT, meta: { form: form } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.clearSubmitErrors"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>clearSubmitErrors (form)](#apidoc.element.redux-form.actions.clearSubmitErrors)
- description and source-code
```javascript
function clearSubmitErrors(form) {
  return { type: _actionTypes.CLEAR_SUBMIT_ERRORS, meta: { form: form } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.destroy"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>destroy ()](#apidoc.element.redux-form.actions.destroy)
- description and source-code
```javascript
function destroy() {
  for (var _len = arguments.length, form = Array(_len), _key = 0; _key < _len; _key++) {
    form[_key] = arguments[_key];
  }

  return { type: _actionTypes.DESTROY, meta: { form: form } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.focus"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>focus (form, field)](#apidoc.element.redux-form.actions.focus)
- description and source-code
```javascript
function focus(form, field) {
  return { type: _actionTypes.FOCUS, meta: { form: form, field: field } };
}
```
- example usage
```shell
...
          defaultPrevented = true;
          return event.preventDefault();
        }
      }));
    }

    if (!defaultPrevented) {
      dispatch(_reduxForm.focus(name));
    }
  }
}, {
  key: 'handleBlur',
  value: function handleBlur(event) {
    var _props3 = this.props,
        name = _props3.name,
...
```

#### <a name="apidoc.element.redux-form.actions.initialize"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>initialize (form, values, keepDirty)](#apidoc.element.redux-form.actions.initialize)
- description and source-code
```javascript
function initialize(form, values, keepDirty) {
  var otherMeta = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

  if (keepDirty instanceof Object) {
    otherMeta = keepDirty;
    keepDirty = false;
  }
  return { type: _actionTypes.INITIALIZE, meta: _extends({ form: form, keepDirty: keepDirty }, otherMeta), payload: values };
}
```
- example usage
```shell
...
  key: 'initIfNeeded',
  value: function initIfNeeded(nextProps) {
    var enableReinitialize = this.props.enableReinitialize;

    if (nextProps) {
      if ((enableReinitialize || !nextProps.initialized) && !deepEqual(this.props.initialValues, nextProps.initialValues)) {
        var keepDirty = nextProps.initialized && this.props.keepDirtyOnReinitialize;
        this.props.initialize(nextProps.initialValues, keepDirty);
      }
    } else if (this.props.initialValues && (!this.props.initialized || enableReinitialize)) {
      this.props.initialize(this.props.initialValues, this.props.keepDirtyOnReinitialize);
    }
  }
}, {
  key: 'updateSyncErrorsIfNeeded',
...
```

#### <a name="apidoc.element.redux-form.actions.registerField"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>registerField (form, name, type)](#apidoc.element.redux-form.actions.registerField)
- description and source-code
```javascript
function registerField(form, name, type) {
  return { type: _actionTypes.REGISTER_FIELD, meta: { form: form }, payload: { name: name, type: type } };
}
```
- example usage
```shell
...
  key: 'isPristine',
  value: function isPristine() {
    return this.props.pristine;
  }
}, {
  key: 'register',
  value: function register(name, type, getValidator, getWarner) {
    this.props.registerField(name, type);
    if (getValidator) {
      this.fieldValidators[name] = getValidator;
    }
    if (getWarner) {
      this.fieldWarners[name] = getWarner;
    }
  }
...
```

#### <a name="apidoc.element.redux-form.actions.reset"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>reset (form)](#apidoc.element.redux-form.actions.reset)
- description and source-code
```javascript
function reset(form) {
  return { type: _actionTypes.RESET, meta: { form: form } };
}
```
- example usage
```shell
...
        return !_this7.submitPromise && _this7.listenToSubmit((0, _handleSubmit2.default)(checkSubmit(submitOrEvent), _extends({},
_this7.props, (0, _redux.bindActionCreators)({ blur: blur, change: change }, dispatch)), validExceptSubmit, _this7.asyncValidate
, _this7.getFieldList({ excludeFieldArray: true })));
      });
    }
  }
}, {
  key: 'reset',
  value: function reset() {
    this.props.reset();
  }
}, {
  key: 'render',
  value: function render() {
    // remove some redux-form config-only props
    /* eslint-disable no-unused-vars */
    var _props9 = this.props,
...
```

#### <a name="apidoc.element.redux-form.actions.setSubmitFailed"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>setSubmitFailed (form)](#apidoc.element.redux-form.actions.setSubmitFailed)
- description and source-code
```javascript
function setSubmitFailed(form) {
  for (var _len2 = arguments.length, fields = Array(_len2 > 1 ? _len2 - 1 : 0), _key2 = 1; _key2 < _len2; _key2++) {
    fields[_key2 - 1] = arguments[_key2];
  }

  return { type: _actionTypes.SET_SUBMIT_FAILED, meta: { form: form, fields: fields }, error: true };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.setSubmitSucceeded"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>setSubmitSucceeded (form)](#apidoc.element.redux-form.actions.setSubmitSucceeded)
- description and source-code
```javascript
function setSubmitSucceeded(form) {
  for (var _len3 = arguments.length, fields = Array(_len3 > 1 ? _len3 - 1 : 0), _key3 = 1; _key3 < _len3; _key3++) {
    fields[_key3 - 1] = arguments[_key3];
  }

  return { type: _actionTypes.SET_SUBMIT_SUCCEEDED, meta: { form: form, fields: fields }, error: false };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.startAsyncValidation"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>startAsyncValidation (form, field)](#apidoc.element.redux-form.actions.startAsyncValidation)
- description and source-code
```javascript
function startAsyncValidation(form, field) {
  return { type: _actionTypes.START_ASYNC_VALIDATION, meta: { form: form, field: field } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.startSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>startSubmit (form)](#apidoc.element.redux-form.actions.startSubmit)
- description and source-code
```javascript
function startSubmit(form) {
  return { type: _actionTypes.START_SUBMIT, meta: { form: form } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.stopAsyncValidation"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>stopAsyncValidation (form, errors)](#apidoc.element.redux-form.actions.stopAsyncValidation)
- description and source-code
```javascript
function stopAsyncValidation(form, errors) {
  var action = {
    type: _actionTypes.STOP_ASYNC_VALIDATION,
    meta: { form: form },
    payload: errors
  };
  if (errors && Object.keys(errors).length) {
    action.error = true;
  }
  return action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.stopSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>stopSubmit (form, errors)](#apidoc.element.redux-form.actions.stopSubmit)
- description and source-code
```javascript
function stopSubmit(form, errors) {
  var action = {
    type: _actionTypes.STOP_SUBMIT,
    meta: { form: form },
    payload: errors
  };
  if (errors && Object.keys(errors).length) {
    action.error = true;
  }
  return action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.submit"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>submit (form)](#apidoc.element.redux-form.actions.submit)
- description and source-code
```javascript
function submit(form) {
  return { type: _actionTypes.SUBMIT, meta: { form: form } };
}
```
- example usage
```shell
...
  value: function submitIfNeeded(nextProps) {
    var _props2 = this.props,
        clearSubmit = _props2.clearSubmit,
        triggerSubmit = _props2.triggerSubmit;

    if (!triggerSubmit && nextProps.triggerSubmit) {
      clearSubmit();
      this.submit();
    }
  }
}, {
  key: 'validateIfNeeded',
  value: function validateIfNeeded(nextProps) {
    var _props3 = this.props,
        shouldValidate = _props3.shouldValidate,
...
```

#### <a name="apidoc.element.redux-form.actions.touch"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>touch (form)](#apidoc.element.redux-form.actions.touch)
- description and source-code
```javascript
function touch(form) {
  for (var _len4 = arguments.length, fields = Array(_len4 > 1 ? _len4 - 1 : 0), _key4 = 1; _key4 < _len4; _key4++) {
    fields[_key4 - 1] = arguments[_key4];
  }

  return { type: _actionTypes.TOUCH, meta: { form: form, fields: fields } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.unregisterField"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>unregisterField (form, name)](#apidoc.element.redux-form.actions.unregisterField)
- description and source-code
```javascript
function unregisterField(form, name) {
  var destroyOnUnmount = arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : true;
  return { type: _actionTypes.UNREGISTER_FIELD, meta: { form: form }, payload: { name: name, destroyOnUnmount: destroyOnUnmount } };
}
```
- example usage
```shell
...
    }
  }
}, {
  key: 'unregister',
  value: function unregister(name) {
    if (!this.destroyed) {
      if (this.props.destroyOnUnmount || this.props.forceUnregisterOnUnmount) {
        this.props.unregisterField(name);
        delete this.fieldValidators[name];
        delete this.fieldWarners[name];
      } else {
        this.props.unregisterField(name, false);
      }
    }
  }
...
```

#### <a name="apidoc.element.redux-form.actions.untouch"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>untouch (form)](#apidoc.element.redux-form.actions.untouch)
- description and source-code
```javascript
function untouch(form) {
  for (var _len5 = arguments.length, fields = Array(_len5 > 1 ? _len5 - 1 : 0), _key5 = 1; _key5 < _len5; _key5++) {
    fields[_key5 - 1] = arguments[_key5];
  }

  return { type: _actionTypes.UNTOUCH, meta: { form: form, fields: fields } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.updateSyncErrors"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>updateSyncErrors (form)](#apidoc.element.redux-form.actions.updateSyncErrors)
- description and source-code
```javascript
function updateSyncErrors(form) {
  var syncErrors = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};
  var error = arguments[2];
  return { type: _actionTypes.UPDATE_SYNC_ERRORS, meta: { form: form }, payload: { syncErrors: syncErrors, error: error } };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.actions.updateSyncWarnings"></a>[function <span class="apidocSignatureSpan">redux-form.actions.</span>updateSyncWarnings (form)](#apidoc.element.redux-form.actions.updateSyncWarnings)
- description and source-code
```javascript
function updateSyncWarnings(form) {
  var syncWarnings = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};
  var warning = arguments[2];
  return { type: _actionTypes.UPDATE_SYNC_WARNINGS, meta: { form: form }, payload: { syncWarnings: syncWarnings, warning: warning
 } };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.asyncValidation"></a>[module redux-form.asyncValidation](#apidoc.module.redux-form.asyncValidation)

#### <a name="apidoc.element.redux-form.asyncValidation.default"></a>[function <span class="apidocSignatureSpan">redux-form.asyncValidation.</span>default (fn, start, stop, field)](#apidoc.element.redux-form.asyncValidation.default)
- description and source-code
```javascript
function asyncValidation(fn, start, stop, field) {
  start(field);
  var promise = fn();
  if (!(0, _isPromise2.default)(promise)) {
    throw new Error('asyncValidate function passed to reduxForm must return a promise');
  }
  var handleErrors = function handleErrors(rejected) {
    return function (errors) {
      if (errors && Object.keys(errors).length) {
        stop(errors);
        return errors;
      } else if (rejected) {
        stop();
        throw new Error('Asynchronous validation promise was rejected without errors.');
      }
      stop();
      return Promise.resolve();
    };
  };
  return promise.then(handleErrors(false), handleErrors(true));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.createAll"></a>[module redux-form.createAll](#apidoc.module.redux-form.createAll)

#### <a name="apidoc.element.redux-form.createAll.default"></a>[function <span class="apidocSignatureSpan">redux-form.createAll.</span>default (structure)](#apidoc.element.redux-form.createAll.default)
- description and source-code
```javascript
function createAll(structure) {
  return _extends({
    // separate out field actions
    actionTypes: actionTypes
  }, actions, {
    Field: (0, _Field2.default)(structure),
    Fields: (0, _Fields2.default)(structure),
    FieldArray: (0, _FieldArray2.default)(structure),
    Form: _Form2.default,
    FormSection: _FormSection2.default,
    formValueSelector: (0, _formValueSelector2.default)(structure),
    getFormNames: (0, _getFormNames2.default)(structure),
    getFormValues: (0, _getFormValues2.default)(structure),
    getFormInitialValues: (0, _getFormInitialValues2.default)(structure),
    getFormSyncErrors: (0, _getFormSyncErrors2.default)(structure),
    getFormAsyncErrors: (0, _getFormAsyncErrors2.default)(structure),
    getFormSyncWarnings: (0, _getFormSyncWarnings2.default)(structure),
    getFormSubmitErrors: (0, _getFormSubmitErrors2.default)(structure),
    isDirty: (0, _isDirty2.default)(structure),
    isInvalid: (0, _isInvalid2.default)(structure),
    isPristine: (0, _isPristine2.default)(structure),
    isValid: (0, _isValid2.default)(structure),
    isSubmitting: (0, _isSubmitting2.default)(structure),
    hasSubmitSucceeded: (0, _hasSubmitSucceeded2.default)(structure),
    hasSubmitFailed: (0, _hasSubmitFailed2.default)(structure),
    propTypes: _propTypes2.default,
    reduxForm: (0, _reduxForm2.default)(structure),
    reducer: (0, _reducer2.default)(structure),
    SubmissionError: _SubmissionError2.default,
    values: (0, _values2.default)(structure)
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.createFieldArrayProps"></a>[module redux-form.createFieldArrayProps](#apidoc.module.redux-form.createFieldArrayProps)

#### <a name="apidoc.element.redux-form.createFieldArrayProps.default"></a>[function <span class="apidocSignatureSpan">redux-form.createFieldArrayProps.</span>default (getIn, name, form, sectionPrefix, getValue, _ref)](#apidoc.element.redux-form.createFieldArrayProps.default)
- description and source-code
```javascript
function createFieldArrayProps(getIn, name, form, sectionPrefix, getValue, _ref) {
  var arrayInsert = _ref.arrayInsert,
      arrayMove = _ref.arrayMove,
      arrayPop = _ref.arrayPop,
      arrayPush = _ref.arrayPush,
      arrayRemove = _ref.arrayRemove,
      arrayRemoveAll = _ref.arrayRemoveAll,
      arrayShift = _ref.arrayShift,
      arraySplice = _ref.arraySplice,
      arraySwap = _ref.arraySwap,
      arrayUnshift = _ref.arrayUnshift,
      asyncError = _ref.asyncError,
      dirty = _ref.dirty,
      length = _ref.length,
      pristine = _ref.pristine,
      submitError = _ref.submitError,
      state = _ref.state,
      submitFailed = _ref.submitFailed,
      submitting = _ref.submitting,
      syncError = _ref.syncError,
      syncWarning = _ref.syncWarning,
      value = _ref.value,
      props = _ref.props,
      rest = _objectWithoutProperties(_ref, ['arrayInsert', 'arrayMove', 'arrayPop', 'arrayPush', 'arrayRemove', 'arrayRemoveAll
', 'arrayShift', 'arraySplice', 'arraySwap', 'arrayUnshift', 'asyncError', 'dirty', 'length', 'pristine', 'submitError', 'state', '
submitFailed', 'submitting', 'syncError', 'syncWarning', 'value', 'props']);

  var error = syncError || asyncError || submitError;
  var warning = syncWarning;
  var fieldName = sectionPrefix ? name.replace(sectionPrefix + '.', '') : name;
  var finalProps = _extends({
    fields: {
      _isFieldArray: true,
      forEach: function forEach(callback) {
        return (value || []).forEach(function (item, index) {
          return callback(fieldName + '[' + index + ']', index, finalProps.fields);
        });
      },
      get: getValue,
      getAll: function getAll() {
        return value;
      },
      insert: arrayInsert,
      length: length,
      map: function map(callback) {
        return (value || []).map(function (item, index) {
          return callback(fieldName + '[' + index + ']', index, finalProps.fields);
        });
      },
      move: arrayMove,
      name: name,
      pop: function pop() {
        arrayPop();
        return getIn(value, length - 1);
      },
      push: arrayPush,
      reduce: function reduce(callback, initial) {
        return (value || []).reduce(function (accumulator, item, index) {
          return callback(accumulator, fieldName + '[' + index + ']', index, finalProps.fields);
        }, initial);
      },
      remove: arrayRemove,
      removeAll: arrayRemoveAll,
      shift: function shift() {
        arrayShift();
        return getIn(value, 0);
      },
      swap: arraySwap,
      unshift: arrayUnshift
    },
    meta: {
      dirty: dirty,
      error: error,
      form: form,
      warning: warning,
      invalid: !!error,
      pristine: pristine,
      submitting: submitting,
      submitFailed: submitFailed,
      touched: !!(state && getIn(state, 'touched')),
      valid: !error
    }
  }, props, rest);
  return finalProps;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.createFieldProps"></a>[module redux-form.createFieldProps](#apidoc.module.redux-form.createFieldProps)

#### <a name="apidoc.element.redux-form.createFieldProps.default"></a>[function <span class="apidocSignatureSpan">redux-form.createFieldProps.</span>default (_ref2, name, _ref)](#apidoc.element.redux-form.createFieldProps.default)
- description and source-code
```javascript
function createFieldProps(_ref2, name, _ref) {
  var getIn = _ref2.getIn,
      toJS = _ref2.toJS;

  var asyncError = _ref.asyncError,
      asyncValidating = _ref.asyncValidating,
      onBlur = _ref.onBlur,
      onChange = _ref.onChange,
      onDrop = _ref.onDrop,
      onDragStart = _ref.onDragStart,
      dirty = _ref.dirty,
      dispatch = _ref.dispatch,
      onFocus = _ref.onFocus,
      form = _ref.form,
      format = _ref.format,
      parse = _ref.parse,
      pristine = _ref.pristine,
      props = _ref.props,
      state = _ref.state,
      submitError = _ref.submitError,
      submitFailed = _ref.submitFailed,
      submitting = _ref.submitting,
      syncError = _ref.syncError,
      syncWarning = _ref.syncWarning,
      validate = _ref.validate,
      value = _ref.value,
      _value = _ref._value,
      warn = _ref.warn,
      custom = _objectWithoutProperties(_ref, ['asyncError', 'asyncValidating', 'onBlur', 'onChange', 'onDrop', 'onDragStart', '
dirty', 'dispatch', 'onFocus', 'form', 'format', 'parse', 'pristine', 'props', 'state', 'submitError', 'submitFailed', 'submitting
', 'syncError', 'syncWarning', 'validate', 'value', '_value', 'warn']);

  var error = syncError || asyncError || submitError;
  var warning = syncWarning;

  var formatFieldValue = function formatFieldValue(value, format) {
    if (format === null) {
      return value;
    }
    var defaultFormattedValue = value == null ? '' : value;
    return format ? format(value, name) : defaultFormattedValue;
  };

  var formattedFieldValue = formatFieldValue(value, format);

  return {
    input: processProps(custom.type, {
      name: name,
      onBlur: onBlur,
      onChange: onChange,
      onDragStart: onDragStart,
      onDrop: onDrop,
      onFocus: onFocus,
      value: formattedFieldValue
    }, _value),
    meta: _extends({}, toJS(state), {
      active: !!(state && getIn(state, 'active')),
      asyncValidating: asyncValidating,
      autofilled: !!(state && getIn(state, 'autofilled')),
      dirty: dirty,
      dispatch: dispatch,
      error: error,
      form: form,
      warning: warning,
      invalid: !!error,
      pristine: pristine,
      submitting: !!submitting,
      submitFailed: !!submitFailed,
      touched: !!(state && getIn(state, 'touched')),
      valid: !error,
      visited: !!(state && getIn(state, 'visited'))
    }),
    custom: _extends({}, custom, props)
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.defaultShouldAsyncValidate"></a>[module redux-form.defaultShouldAsyncValidate](#apidoc.module.redux-form.defaultShouldAsyncValidate)

#### <a name="apidoc.element.redux-form.defaultShouldAsyncValidate.default"></a>[function <span class="apidocSignatureSpan">redux-form.defaultShouldAsyncValidate.</span>default (_ref)](#apidoc.element.redux-form.defaultShouldAsyncValidate.default)
- description and source-code
```javascript
function defaultShouldAsyncValidate(_ref) {
  var initialized = _ref.initialized,
      trigger = _ref.trigger,
      pristine = _ref.pristine,
      syncValidationPasses = _ref.syncValidationPasses;

  if (!syncValidationPasses) {
    return false;
  }
  switch (trigger) {
    case 'blur':
      // blurring
      return true;
    case 'submit':
      // submitting, so only async validate if form is dirty or was never initialized
      // conversely, DON'T async validate if the form is pristine just as it was initialized
      return !pristine || !initialized;
    default:
      return false;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.defaultShouldValidate"></a>[module redux-form.defaultShouldValidate](#apidoc.module.redux-form.defaultShouldValidate)

#### <a name="apidoc.element.redux-form.defaultShouldValidate.default"></a>[function <span class="apidocSignatureSpan">redux-form.defaultShouldValidate.</span>default (_ref)](#apidoc.element.redux-form.defaultShouldValidate.default)
- description and source-code
```javascript
function defaultShouldValidate(_ref) {
  var values = _ref.values,
      nextProps = _ref.nextProps,
      initialRender = _ref.initialRender,
      lastFieldValidatorKeys = _ref.lastFieldValidatorKeys,
      fieldValidatorKeys = _ref.fieldValidatorKeys,
      structure = _ref.structure;

  if (initialRender) {
    return true;
  }
  return !structure.deepEqual(values, nextProps.values) || !structure.deepEqual(lastFieldValidatorKeys, fieldValidatorKeys);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.deleteInWithCleanUp"></a>[module redux-form.deleteInWithCleanUp](#apidoc.module.redux-form.deleteInWithCleanUp)

#### <a name="apidoc.element.redux-form.deleteInWithCleanUp.default"></a>[function <span class="apidocSignatureSpan">redux-form.deleteInWithCleanUp.</span>default (_ref)](#apidoc.element.redux-form.deleteInWithCleanUp.default)
- description and source-code
```javascript
function createDeleteInWithCleanUp(_ref) {
  var deepEqual = _ref.deepEqual,
      empty = _ref.empty,
      getIn = _ref.getIn,
      deleteIn = _ref.deleteIn,
      setIn = _ref.setIn;


  var deleteInWithCleanUp = function deleteInWithCleanUp(state, path) {
    if (path[path.length - 1] === ']') {
      // array path
      var pathTokens = (0, _toPath3.default)(path);
      pathTokens.pop();
      var parent = getIn(state, pathTokens.join('.'));
      return parent ? setIn(state, path, undefined) : state;
    }
    var result = deleteIn(state, path);
    var dotIndex = path.lastIndexOf('.');
    if (dotIndex > 0) {
      var parentPath = path.substring(0, dotIndex);
      if (parentPath[parentPath.length - 1] !== ']') {
        var _parent = getIn(result, parentPath);
        if (deepEqual(_parent, empty)) {
          return deleteInWithCleanUp(result, parentPath);
        }
      }
    }
    return result;
  };

  return deleteInWithCleanUp;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.formValueSelector"></a>[module redux-form.formValueSelector](#apidoc.module.redux-form.formValueSelector)

#### <a name="apidoc.element.redux-form.formValueSelector.default"></a>[function <span class="apidocSignatureSpan">redux-form.formValueSelector.</span>default (_ref)](#apidoc.element.redux-form.formValueSelector.default)
- description and source-code
```javascript
function createFormValueSelector(_ref) {
  var getIn = _ref.getIn;
  return function (form) {
    var getFormState = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : function (state) {
      return getIn(state, 'form');
    };

    (0, _invariant2.default)(form, 'Form value must be specified');
    return function (state) {
      for (var _len = arguments.length, fields = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
        fields[_key - 1] = arguments[_key];
      }

      (0, _invariant2.default)(fields.length, 'No fields specified');
      return fields.length === 1 ?
      // only selecting one field, so return its value
      getIn(getFormState(state), form + '.values.' + fields[0]) :
      // selecting many fields, so return an object of field values
      fields.reduce(function (accumulator, field) {
        var value = getIn(getFormState(state), form + '.values.' + field);
        return value === undefined ? accumulator : _plain2.default.setIn(accumulator, field, value);
      }, {});
    };
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.generateValidator"></a>[module redux-form.generateValidator](#apidoc.module.redux-form.generateValidator)

#### <a name="apidoc.element.redux-form.generateValidator.default"></a>[function <span class="apidocSignatureSpan">redux-form.generateValidator.</span>default (validators, _ref)](#apidoc.element.redux-form.generateValidator.default)
- description and source-code
```javascript
function generateValidator(validators, _ref) {
  var getIn = _ref.getIn;
  return function (values, props) {
    var errors = {};
    Object.keys(validators).forEach(function (name) {
      var value = getIn(values, name);
      var error = getError(value, values, props, validators[name]);
      if (error) {
        errors = _plain2.default.setIn(errors, name, error);
      }
    });
    return errors;
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.handleSubmit"></a>[module redux-form.handleSubmit](#apidoc.module.redux-form.handleSubmit)

#### <a name="apidoc.element.redux-form.handleSubmit.default"></a>[function <span class="apidocSignatureSpan">redux-form.handleSubmit.</span>default (submit, props, valid, asyncValidate, fields)](#apidoc.element.redux-form.handleSubmit.default)
- description and source-code
```javascript
function handleSubmit(submit, props, valid, asyncValidate, fields) {
  var dispatch = props.dispatch,
      onSubmitFail = props.onSubmitFail,
      onSubmitSuccess = props.onSubmitSuccess,
      startSubmit = props.startSubmit,
      stopSubmit = props.stopSubmit,
      setSubmitFailed = props.setSubmitFailed,
      setSubmitSucceeded = props.setSubmitSucceeded,
      syncErrors = props.syncErrors,
      touch = props.touch,
      values = props.values,
      persistentSubmitErrors = props.persistentSubmitErrors;


  touch.apply(undefined, _toConsumableArray(fields)); // mark all fields as touched

  if (valid || persistentSubmitErrors) {
    var doSubmit = function doSubmit() {
      var result = void 0;
      try {
        result = submit(values, dispatch, props);
      } catch (submitError) {
        var error = submitError instanceof _SubmissionError2.default ? submitError.errors : undefined;
        stopSubmit(error);
        setSubmitFailed.apply(undefined, _toConsumableArray(fields));
        if (onSubmitFail) {
          onSubmitFail(error, dispatch, submitError, props);
        }
        if (error || onSubmitFail) {
          // if you've provided an onSubmitFail callback, don't re-throw the error
          return error;
        } else {
          throw submitError;
        }
      }
      if ((0, _isPromise2.default)(result)) {
        startSubmit();
        return result.then(function (submitResult) {
          stopSubmit();
          setSubmitSucceeded();
          if (onSubmitSuccess) {
            onSubmitSuccess(submitResult, dispatch, props);
          }
          return submitResult;
        }, function (submitError) {
          var error = submitError instanceof _SubmissionError2.default ? submitError.errors : undefined;
          stopSubmit(error);
          setSubmitFailed.apply(undefined, _toConsumableArray(fields));
          if (onSubmitFail) {
            onSubmitFail(error, dispatch, submitError, props);
          }
          if (error || onSubmitFail) {
            // if you've provided an onSubmitFail callback, don't re-throw the error
            return error;
          } else {
            throw submitError;
          }
        });
      } else {
        setSubmitSucceeded();
        if (onSubmitSuccess) {
          onSubmitSuccess(result, dispatch, props);
        }
      }
      return result;
    };

    var asyncValidateResult = asyncValidate && asyncValidate();
    if (asyncValidateResult) {
      return asyncValidateResult.then(function (asyncErrors) {
        if (asyncErrors) {
          throw asyncErrors;
        }
        return doSubmit();
      }).catch(function (asyncErrors) {
        setSubmitFailed.apply(undefined, _toConsumableArray(fields));
        if (onSubmitFail) {
          onSubmitFail(asyncErrors, dispatch, null, props);
        }
        return Promise.reject(asyncErrors);
      });
    } else {
      return doSubmit();
    }
  } else {
    setSubmitFailed.apply(undefined, _toConsumableArray(fields));
    if (onSubmitFail) {
      onSubmitFail(syncErrors, dispatch, null, props);
    }
    return syncErrors;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.hasError"></a>[module redux-form.hasError](#apidoc.module.redux-form.hasError)

#### <a name="apidoc.element.redux-form.hasError.default"></a>[function <span class="apidocSignatureSpan">redux-form.hasError.</span>default (_ref)](#apidoc.element.redux-form.hasError.default)
- description and source-code
```javascript
function createHasError(_ref) {
  var getIn = _ref.getIn;

  var hasError = function hasError(field, syncErrors, asyncErrors, submitErrors) {
    if (!syncErrors && !asyncErrors && !submitErrors) {
      return false;
    }

    var name = getIn(field, 'name');
    var type = getIn(field, 'type');
    return getErrorKeys(name, type).some(function (key) {
      return getIn(syncErrors, key) || getIn(asyncErrors, key) || getIn(submitErrors, key);
    });
  };
  return hasError;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.isChecked"></a>[module redux-form.isChecked](#apidoc.module.redux-form.isChecked)

#### <a name="apidoc.element.redux-form.isChecked.default"></a>[function <span class="apidocSignatureSpan">redux-form.isChecked.</span>default (value)](#apidoc.element.redux-form.isChecked.default)
- description and source-code
```javascript
function isChecked(value) {
  if (typeof value === 'boolean') {
    return value;
  }
  if (typeof value === 'string') {
    var lower = value.toLowerCase();
    if (lower === 'true') {
      return true;
    }
    if (lower === 'false') {
      return false;
    }
  }
  return undefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.propTypes"></a>[module redux-form.propTypes](#apidoc.module.redux-form.propTypes)

#### <a name="apidoc.element.redux-form.propTypes.anyTouched"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>anyTouched ()](#apidoc.element.redux-form.propTypes.anyTouched)
- description and source-code
```javascript
anyTouched = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.array"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>array ()](#apidoc.element.redux-form.propTypes.array)
- description and source-code
```javascript
array = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.asyncValidate"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>asyncValidate ()](#apidoc.element.redux-form.propTypes.asyncValidate)
- description and source-code
```javascript
asyncValidate = function () { [native code] }
```
- example usage
```shell
...

    if (!defaultPrevented) {
      // dispatch blur action
      dispatch(_reduxForm.blur(name, newValue));

      // call post-blur callback
      if (_reduxForm.asyncValidate) {
        _reduxForm.asyncValidate(name, newValue);
      }
    }
  }
}, {
  key: 'handleDragStart',
  value: function handleDragStart(event) {
    var _props4 = this.props,
...
```

#### <a name="apidoc.element.redux-form.propTypes.asyncValidating"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>asyncValidating ()](#apidoc.element.redux-form.propTypes.asyncValidating)
- description and source-code
```javascript
asyncValidating = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.autofill"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>autofill ()](#apidoc.element.redux-form.propTypes.autofill)
- description and source-code
```javascript
autofill = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.blur"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>blur ()](#apidoc.element.redux-form.propTypes.blur)
- description and source-code
```javascript
blur = function () { [native code] }
```
- example usage
```shell
...
        return event.preventDefault();
      }
    }), newValue, previousValue);
  }

  if (!defaultPrevented) {
    // dispatch blur action
    dispatch(_reduxForm.blur(name, newValue));

    // call post-blur callback
    if (_reduxForm.asyncValidate) {
      _reduxForm.asyncValidate(name, newValue);
    }
  }
}
...
```

#### <a name="apidoc.element.redux-form.propTypes.change"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>change ()](#apidoc.element.redux-form.propTypes.change)
- description and source-code
```javascript
change = function () { [native code] }
```
- example usage
```shell
...
          defaultPrevented = true;
          return event.preventDefault();
        }
      }), newValue, previousValue);
    }
    if (!defaultPrevented) {
      // dispatch change action
      dispatch(_reduxForm.change(name, newValue));
    }
  }
}, {
  key: 'handleFocus',
  value: function handleFocus(event) {
    var _props2 = this.props,
        name = _props2.name,
...
```

#### <a name="apidoc.element.redux-form.propTypes.clearAsyncError"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>clearAsyncError ()](#apidoc.element.redux-form.propTypes.clearAsyncError)
- description and source-code
```javascript
clearAsyncError = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.clearSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>clearSubmit ()](#apidoc.element.redux-form.propTypes.clearSubmit)
- description and source-code
```javascript
clearSubmit = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.destroy"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>destroy ()](#apidoc.element.redux-form.propTypes.destroy)
- description and source-code
```javascript
destroy = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.dirty"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>dirty ()](#apidoc.element.redux-form.propTypes.dirty)
- description and source-code
```javascript
dirty = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.dispatch"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>dispatch ()](#apidoc.element.redux-form.propTypes.dispatch)
- description and source-code
```javascript
dispatch = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.error"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>error ()](#apidoc.element.redux-form.propTypes.error)
- description and source-code
```javascript
error = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.form"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>form ()](#apidoc.element.redux-form.propTypes.form)
- description and source-code
```javascript
form = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.handleSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>handleSubmit ()](#apidoc.element.redux-form.propTypes.handleSubmit)
- description and source-code
```javascript
handleSubmit = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.initialValues"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialValues ()](#apidoc.element.redux-form.propTypes.initialValues)
- description and source-code
```javascript
initialValues = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.initialize"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialize ()](#apidoc.element.redux-form.propTypes.initialize)
- description and source-code
```javascript
initialize = function () { [native code] }
```
- example usage
```shell
...
  key: 'initIfNeeded',
  value: function initIfNeeded(nextProps) {
    var enableReinitialize = this.props.enableReinitialize;

    if (nextProps) {
      if ((enableReinitialize || !nextProps.initialized) && !deepEqual(this.props.initialValues, nextProps.initialValues)) {
        var keepDirty = nextProps.initialized && this.props.keepDirtyOnReinitialize;
        this.props.initialize(nextProps.initialValues, keepDirty);
      }
    } else if (this.props.initialValues && (!this.props.initialized || enableReinitialize)) {
      this.props.initialize(this.props.initialValues, this.props.keepDirtyOnReinitialize);
    }
  }
}, {
  key: 'updateSyncErrorsIfNeeded',
...
```

#### <a name="apidoc.element.redux-form.propTypes.initialized"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialized ()](#apidoc.element.redux-form.propTypes.initialized)
- description and source-code
```javascript
initialized = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.invalid"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>invalid ()](#apidoc.element.redux-form.propTypes.invalid)
- description and source-code
```javascript
invalid = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.pristine"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>pristine ()](#apidoc.element.redux-form.propTypes.pristine)
- description and source-code
```javascript
pristine = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.pure"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>pure ()](#apidoc.element.redux-form.propTypes.pure)
- description and source-code
```javascript
pure = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.reset"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>reset ()](#apidoc.element.redux-form.propTypes.reset)
- description and source-code
```javascript
reset = function () { [native code] }
```
- example usage
```shell
...
        return !_this7.submitPromise && _this7.listenToSubmit((0, _handleSubmit2.default)(checkSubmit(submitOrEvent), _extends({},
_this7.props, (0, _redux.bindActionCreators)({ blur: blur, change: change }, dispatch)), validExceptSubmit, _this7.asyncValidate
, _this7.getFieldList({ excludeFieldArray: true })));
      });
    }
  }
}, {
  key: 'reset',
  value: function reset() {
    this.props.reset();
  }
}, {
  key: 'render',
  value: function render() {
    // remove some redux-form config-only props
    /* eslint-disable no-unused-vars */
    var _props9 = this.props,
...
```

#### <a name="apidoc.element.redux-form.propTypes.submit"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submit ()](#apidoc.element.redux-form.propTypes.submit)
- description and source-code
```javascript
submit = function () { [native code] }
```
- example usage
```shell
...
  value: function submitIfNeeded(nextProps) {
    var _props2 = this.props,
        clearSubmit = _props2.clearSubmit,
        triggerSubmit = _props2.triggerSubmit;

    if (!triggerSubmit && nextProps.triggerSubmit) {
      clearSubmit();
      this.submit();
    }
  }
}, {
  key: 'validateIfNeeded',
  value: function validateIfNeeded(nextProps) {
    var _props3 = this.props,
        shouldValidate = _props3.shouldValidate,
...
```

#### <a name="apidoc.element.redux-form.propTypes.submitFailed"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submitFailed ()](#apidoc.element.redux-form.propTypes.submitFailed)
- description and source-code
```javascript
submitFailed = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.submitSucceeded"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submitSucceeded ()](#apidoc.element.redux-form.propTypes.submitSucceeded)
- description and source-code
```javascript
submitSucceeded = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.submitting"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>submitting ()](#apidoc.element.redux-form.propTypes.submitting)
- description and source-code
```javascript
submitting = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.touch"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>touch ()](#apidoc.element.redux-form.propTypes.touch)
- description and source-code
```javascript
touch = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.triggerSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>triggerSubmit ()](#apidoc.element.redux-form.propTypes.triggerSubmit)
- description and source-code
```javascript
triggerSubmit = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.untouch"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>untouch ()](#apidoc.element.redux-form.propTypes.untouch)
- description and source-code
```javascript
untouch = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.valid"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>valid ()](#apidoc.element.redux-form.propTypes.valid)
- description and source-code
```javascript
valid = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.warning"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>warning ()](#apidoc.element.redux-form.propTypes.warning)
- description and source-code
```javascript
warning = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.propTypes.array"></a>[module redux-form.propTypes.array](#apidoc.module.redux-form.propTypes.array)

#### <a name="apidoc.element.redux-form.propTypes.array.array"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>array ()](#apidoc.element.redux-form.propTypes.array.array)
- description and source-code
```javascript
array = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.array.isRequired"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.array.</span>isRequired ()](#apidoc.element.redux-form.propTypes.array.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.propTypes.error"></a>[module redux-form.propTypes.error](#apidoc.module.redux-form.propTypes.error)

#### <a name="apidoc.element.redux-form.propTypes.error.error"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>error ()](#apidoc.element.redux-form.propTypes.error.error)
- description and source-code
```javascript
error = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.error.isRequired"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.error.</span>isRequired ()](#apidoc.element.redux-form.propTypes.error.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.propTypes.initialValues"></a>[module redux-form.propTypes.initialValues](#apidoc.module.redux-form.propTypes.initialValues)

#### <a name="apidoc.element.redux-form.propTypes.initialValues.initialValues"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>initialValues ()](#apidoc.element.redux-form.propTypes.initialValues.initialValues)
- description and source-code
```javascript
initialValues = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.initialValues.isRequired"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.initialValues.</span>isRequired ()](#apidoc.element.redux-form.propTypes.initialValues.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.propTypes.triggerSubmit"></a>[module redux-form.propTypes.triggerSubmit](#apidoc.module.redux-form.propTypes.triggerSubmit)

#### <a name="apidoc.element.redux-form.propTypes.triggerSubmit.triggerSubmit"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.</span>triggerSubmit ()](#apidoc.element.redux-form.propTypes.triggerSubmit.triggerSubmit)
- description and source-code
```javascript
triggerSubmit = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.propTypes.triggerSubmit.isRequired"></a>[function <span class="apidocSignatureSpan">redux-form.propTypes.triggerSubmit.</span>isRequired ()](#apidoc.element.redux-form.propTypes.triggerSubmit.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.reducer"></a>[module redux-form.reducer](#apidoc.module.redux-form.reducer)

#### <a name="apidoc.element.redux-form.reducer.reducer"></a>[function <span class="apidocSignatureSpan">redux-form.</span>reducer ()](#apidoc.element.redux-form.reducer.reducer)
- description and source-code
```javascript
reducer = function () {
  var state = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : empty;
  var action = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  var form = action && action.meta && action.meta.form;
  if (!form) {
    return state;
  }
  if (action.type === _actionTypes.DESTROY) {
    return action.meta.form.reduce(function (result, form) {
      return deleteInWithCleanUp(result, form);
    }, state);
  }
  var formState = getIn(state, form);
  var result = reducer(formState, action);
  return result === formState ? state : setIn(state, form, result);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-form.reducer.plugin"></a>[function <span class="apidocSignatureSpan">redux-form.reducer.</span>plugin (reducers)](#apidoc.element.redux-form.reducer.plugin)
- description and source-code
```javascript
function plugin(reducers) {
  var _this = this;

  // use 'function' keyword to enable 'this'
  return decorate(function () {
    var state = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : empty;
    var action = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};
    return Object.keys(reducers).reduce(function (accumulator, key) {
      var previousState = getIn(accumulator, key);
      var nextState = reducers[key](previousState, action, getIn(state, key));
      return nextState === previousState ? accumulator : setIn(accumulator, key, nextState);
    }, _this(state, action));
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.reduxForm"></a>[module redux-form.reduxForm](#apidoc.module.redux-form.reduxForm)

#### <a name="apidoc.element.redux-form.reduxForm.default"></a>[function <span class="apidocSignatureSpan">redux-form.reduxForm.</span>default (structure)](#apidoc.element.redux-form.reduxForm.default)
- description and source-code
```javascript
function createReduxForm(structure) {
  var deepEqual = structure.deepEqual,
      empty = structure.empty,
      getIn = structure.getIn,
      setIn = structure.setIn,
      keys = structure.keys,
      fromJS = structure.fromJS;

  var isValid = (0, _isValid2.default)(structure);
  return function (initialConfig) {
    var config = _extends({
      touchOnBlur: true,
      touchOnChange: false,
      persistentSubmitErrors: false,
      destroyOnUnmount: true,
      shouldAsyncValidate: _defaultShouldAsyncValidate2.default,
      shouldValidate: _defaultShouldValidate2.default,
      enableReinitialize: false,
      keepDirtyOnReinitialize: false,
      getFormState: function getFormState(state) {
        return getIn(state, 'form');
      },
      pure: true,
      forceUnregisterOnUnmount: false
    }, initialConfig);

    return function (WrappedComponent) {
      var Form = function (_Component) {
        _inherits(Form, _Component);

        function Form(props) {
          _classCallCheck(this, Form);

          var _this = _possibleConstructorReturn(this, (Form.__proto__ || Object.getPrototypeOf(Form)).call(this, props));

          _this.submit = _this.submit.bind(_this);
          _this.reset = _this.reset.bind(_this);
          _this.asyncValidate = _this.asyncValidate.bind(_this);
          _this.getValues = _this.getValues.bind(_this);
          _this.register = _this.register.bind(_this);
          _this.unregister = _this.unregister.bind(_this);
          _this.submitCompleted = _this.submitCompleted.bind(_this);
          _this.submitFailed = _this.submitFailed.bind(_this);
          _this.fieldValidators = {};
          _this.lastFieldValidatorKeys = [];
          _this.fieldWarners = {};
          _this.lastFieldWarnerKeys = [];
          return _this;
        }

        _createClass(Form, [{
          key: 'getChildContext',
          value: function getChildContext() {
            var _this2 = this;

            return {
              _reduxForm: _extends({}, this.props, {
                getFormState: function getFormState(state) {
                  return getIn(_this2.props.getFormState(state), _this2.props.form);
                },
                asyncValidate: this.asyncValidate,
                getValues: this.getValues,
                sectionPrefix: undefined,
                register: this.register,
                unregister: this.unregister,
                registerInnerOnSubmit: function registerInnerOnSubmit(innerOnSubmit) {
                  return _this2.innerOnSubmit = innerOnSubmit;
                }
              })
            };
          }
        }, {
          key: 'initIfNeeded',
          value: function initIfNeeded(nextProps) {
            var enableReinitialize = this.props.enableReinitialize;

            if (nextProps) {
              if ((enableReinitialize || !nextProps.initialized) && !deepEqual(this.props.initialValues, nextProps.initialValues
)) {
                var keepDirty = nextProps.initialized && this.props.keepDirtyOnReinitialize;
                this.props.initialize(nextProps.initialValues, keepDirty);
              }
            } else if (this.props.initialValues && (!this.props.initialized || enableReinitialize)) {
              this.props.initialize(this.props.initialValues, this.props.keepDirtyOnReinitialize);
            }
          }
        }, {
          key: 'updateSyncErrorsIfNeeded',
          value: function updateSyncErrorsIfNeeded(nextSyncErrors, nextError) {
            var _props = this.props,
                error = _props.error,
                syncErrors = _props.syncErrors,
                updateSyncErrors = _props.updateSyncErrors;

            var noErrors = (!syncErrors || !Object.keys(syncErrors).length) && !error;
            var nextNoErrors = (!nextSyncErrors || !Object.keys(nextSyncErrors).length) && !nextError;
            if (!(noErrors && nextNoErrors) && (!_plain2.default.deepEqual(syncErrors, nextSyncErrors) || !_plain2.default.deepEqual
(error, nextError))) {
              updateSyncErrors(nextSyncErrors, nextError); ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-form.values"></a>[module redux-form.values](#apidoc.module.redux-form.values)

#### <a name="apidoc.element.redux-form.values.default"></a>[function <span class="apidocSignatureSpan">redux-form.values.</span>default (_ref)](#apidoc.element.redux-form.values.default)
- description and source-code
```javascript
function createValues(_ref) {
  var getIn = _ref.getIn;
  return function (config) {
    var _prop$getFormState$co = _extends({
      prop: 'values',
      getFormState: function getFormState(state) {
        return getIn(state, 'form');
      }
    }, config),
        form = _prop$getFormState$co.form,
        prop = _prop$getFormState$co.prop,
        getFormState = _prop$getFormState$co.getFormState;

    return (0, _reactRedux.connect)(function (state) {
      return _defineProperty({}, prop, getIn(getFormState(state), form + '.values'));
    }, function () {
      return {};
    } // ignore dispatch
    );
  };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
