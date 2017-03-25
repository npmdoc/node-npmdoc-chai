# api documentation for  [chai (v3.5.0)](http://chaijs.com)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-chai.svg)](https://travis-ci.org/npmdoc/node-npmdoc-chai)
#### BDD/TDD assertion library for node.js and the browser. Test framework agnostic.

[![NPM](https://nodei.co/npm/chai.png?downloads=true)](https://www.npmjs.com/package/chai)

[![apidoc](https://npmdoc.github.io/node-npmdoc-chai/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-chai_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-chai/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-chai/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Jake Luer",
        "email": "jake@alogicalparadox.com"
    },
    "bugs": {
        "url": "https://github.com/chaijs/chai/issues"
    },
    "contributors": [
        {
            "name": "Jake Luer",
            "email": "jake@alogicalparadox.com"
        },
        {
            "name": "Domenic Denicola",
            "email": "domenic@domenicdenicola.com",
            "url": "http://domenicdenicola.com"
        },
        {
            "name": "Veselin Todorov",
            "email": "hi@vesln.com"
        },
        {
            "name": "John Firebaugh",
            "email": "john.firebaugh@gmail.com"
        }
    ],
    "dependencies": {
        "assertion-error": "^1.0.1",
        "deep-eql": "^0.1.3",
        "type-detect": "^1.0.0"
    },
    "description": "BDD/TDD assertion library for node.js and the browser. Test framework agnostic.",
    "devDependencies": {
        "browserify": "^10.2.1",
        "bump-cli": "^1.1.3",
        "istanbul": "^0.3.14",
        "karma": "^0.13.16",
        "karma-firefox-launcher": "^0.1.6",
        "karma-mocha": "^0.1.10",
        "karma-phantomjs-launcher": "^0.2.0",
        "karma-sauce-launcher": "^0.2.11",
        "mocha": "^2.2.5"
    },
    "directories": {},
    "dist": {
        "shasum": "4d02637b067fe958bdbfdd3a40ec56fef7373247",
        "tarball": "https://registry.npmjs.org/chai/-/chai-3.5.0.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "gitHead": "4ca0218391cf947c6cfac2d1a7424a63a4b4c232",
    "homepage": "http://chaijs.com",
    "keywords": [
        "test",
        "assertion",
        "assert",
        "testing",
        "chai"
    ],
    "license": "MIT",
    "main": "./index",
    "maintainers": [
        {
            "name": "jakeluer",
            "email": "jake@alogicalparadox.com"
        },
        {
            "name": "chaijs",
            "email": "chaijs@keithcirkel.co.uk"
        }
    ],
    "name": "chai",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/chaijs/chai.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "3.5.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module chai](#apidoc.module.chai)
1.  [function <span class="apidocSignatureSpan">chai.</span>Assertion (obj, msg, stack)](#apidoc.element.chai.Assertion)
1.  [function <span class="apidocSignatureSpan">chai.</span>AssertionError (message, _props, ssf)](#apidoc.element.chai.AssertionError)
1.  [function <span class="apidocSignatureSpan">chai.</span>Should ()](#apidoc.element.chai.Should)
1.  [function <span class="apidocSignatureSpan">chai.</span>assert (express, errmsg)](#apidoc.element.chai.assert)
1.  [function <span class="apidocSignatureSpan">chai.</span>expect (val, message)](#apidoc.element.chai.expect)
1.  [function <span class="apidocSignatureSpan">chai.</span>should ()](#apidoc.element.chai.should)
1.  [function <span class="apidocSignatureSpan">chai.</span>use (fn)](#apidoc.element.chai.use)
1.  [function <span class="apidocSignatureSpan">chai.</span>util.type (obj)](#apidoc.element.chai.util.type)
1.  object <span class="apidocSignatureSpan">chai.</span>Assertion.prototype
1.  object <span class="apidocSignatureSpan">chai.</span>AssertionError.prototype
1.  object <span class="apidocSignatureSpan">chai.</span>config
1.  object <span class="apidocSignatureSpan">chai.</span>util
1.  object <span class="apidocSignatureSpan">chai.</span>util.type.Library.prototype
1.  string <span class="apidocSignatureSpan">chai.</span>version

#### [module chai.Assertion](#apidoc.module.chai.Assertion)
1.  [function <span class="apidocSignatureSpan">chai.</span>Assertion (obj, msg, stack)](#apidoc.element.chai.Assertion.Assertion)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.</span>addChainableMethod (name, fn, chainingBehavior)](#apidoc.element.chai.Assertion.addChainableMethod)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.</span>addMethod (name, fn)](#apidoc.element.chai.Assertion.addMethod)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.</span>addProperty (name, fn)](#apidoc.element.chai.Assertion.addProperty)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.</span>overwriteChainableMethod (name, fn, chainingBehavior)](#apidoc.element.chai.Assertion.overwriteChainableMethod)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.</span>overwriteMethod (name, fn)](#apidoc.element.chai.Assertion.overwriteMethod)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.</span>overwriteProperty (name, fn)](#apidoc.element.chai.Assertion.overwriteProperty)

#### [module chai.Assertion.prototype](#apidoc.module.chai.Assertion.prototype)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>Throw ()](#apidoc.element.chai.Assertion.prototype.Throw)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>above ()](#apidoc.element.chai.Assertion.prototype.above)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>approximately ()](#apidoc.element.chai.Assertion.prototype.approximately)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>assert (expr, msg, negateMsg, expected, _actual, showDiff)](#apidoc.element.chai.Assertion.prototype.assert)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>below ()](#apidoc.element.chai.Assertion.prototype.below)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>closeTo ()](#apidoc.element.chai.Assertion.prototype.closeTo)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>eq ()](#apidoc.element.chai.Assertion.prototype.eq)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>eql ()](#apidoc.element.chai.Assertion.prototype.eql)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>eqls ()](#apidoc.element.chai.Assertion.prototype.eqls)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>equal ()](#apidoc.element.chai.Assertion.prototype.equal)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>equals ()](#apidoc.element.chai.Assertion.prototype.equals)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>greaterThan ()](#apidoc.element.chai.Assertion.prototype.greaterThan)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>gt ()](#apidoc.element.chai.Assertion.prototype.gt)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>gte ()](#apidoc.element.chai.Assertion.prototype.gte)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>haveOwnProperty ()](#apidoc.element.chai.Assertion.prototype.haveOwnProperty)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>haveOwnPropertyDescriptor ()](#apidoc.element.chai.Assertion.prototype.haveOwnPropertyDescriptor)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>instanceOf ()](#apidoc.element.chai.Assertion.prototype.instanceOf)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>instanceof ()](#apidoc.element.chai.Assertion.prototype.instanceof)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>key ()](#apidoc.element.chai.Assertion.prototype.key)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>keys ()](#apidoc.element.chai.Assertion.prototype.keys)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>least ()](#apidoc.element.chai.Assertion.prototype.least)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lengthOf ()](#apidoc.element.chai.Assertion.prototype.lengthOf)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lessThan ()](#apidoc.element.chai.Assertion.prototype.lessThan)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lt ()](#apidoc.element.chai.Assertion.prototype.lt)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lte ()](#apidoc.element.chai.Assertion.prototype.lte)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>match ()](#apidoc.element.chai.Assertion.prototype.match)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>matches ()](#apidoc.element.chai.Assertion.prototype.matches)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>members ()](#apidoc.element.chai.Assertion.prototype.members)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>most ()](#apidoc.element.chai.Assertion.prototype.most)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>oneOf ()](#apidoc.element.chai.Assertion.prototype.oneOf)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>ownProperty ()](#apidoc.element.chai.Assertion.prototype.ownProperty)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>ownPropertyDescriptor ()](#apidoc.element.chai.Assertion.prototype.ownPropertyDescriptor)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>property ()](#apidoc.element.chai.Assertion.prototype.property)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>respondTo ()](#apidoc.element.chai.Assertion.prototype.respondTo)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>respondsTo ()](#apidoc.element.chai.Assertion.prototype.respondsTo)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>satisfies ()](#apidoc.element.chai.Assertion.prototype.satisfies)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>satisfy ()](#apidoc.element.chai.Assertion.prototype.satisfy)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>string ()](#apidoc.element.chai.Assertion.prototype.string)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>throw ()](#apidoc.element.chai.Assertion.prototype.throw)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>throws ()](#apidoc.element.chai.Assertion.prototype.throws)
1.  [function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>within ()](#apidoc.element.chai.Assertion.prototype.within)
1.  object <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>__methods

#### [module chai.AssertionError](#apidoc.module.chai.AssertionError)
1.  [function <span class="apidocSignatureSpan">chai.</span>AssertionError (message, _props, ssf)](#apidoc.element.chai.AssertionError.AssertionError)

#### [module chai.AssertionError.prototype](#apidoc.module.chai.AssertionError.prototype)
1.  [function <span class="apidocSignatureSpan">chai.AssertionError.prototype.</span>constructor (message, _props, ssf)](#apidoc.element.chai.AssertionError.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">chai.AssertionError.prototype.</span>toJSON (stack)](#apidoc.element.chai.AssertionError.prototype.toJSON)
1.  string <span class="apidocSignatureSpan">chai.AssertionError.prototype.</span>name

#### [module chai.assert](#apidoc.module.chai.assert)
1.  [function <span class="apidocSignatureSpan">chai.</span>assert (express, errmsg)](#apidoc.element.chai.assert.assert)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>Throw (fn, errt, errs, msg)](#apidoc.element.chai.assert.Throw)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>approximately (act, exp, delta, msg)](#apidoc.element.chai.assert.approximately)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>changes (fn, obj, prop)](#apidoc.element.chai.assert.changes)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>closeTo (act, exp, delta, msg)](#apidoc.element.chai.assert.closeTo)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>decreases (fn, obj, prop)](#apidoc.element.chai.assert.decreases)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>deepEqual (act, exp, msg)](#apidoc.element.chai.assert.deepEqual)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>deepProperty (obj, prop, msg)](#apidoc.element.chai.assert.deepProperty)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>deepPropertyNotVal (obj, prop, val, msg)](#apidoc.element.chai.assert.deepPropertyNotVal)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>deepPropertyVal (obj, prop, val, msg)](#apidoc.element.chai.assert.deepPropertyVal)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>doesNotChange (fn, obj, prop)](#apidoc.element.chai.assert.doesNotChange)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>doesNotDecrease (fn, obj, prop)](#apidoc.element.chai.assert.doesNotDecrease)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>doesNotIncrease (fn, obj, prop)](#apidoc.element.chai.assert.doesNotIncrease)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>doesNotThrow (fn, type, msg)](#apidoc.element.chai.assert.doesNotThrow)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>equal (act, exp, msg)](#apidoc.element.chai.assert.equal)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>extensible (obj, msg)](#apidoc.element.chai.assert.extensible)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>fail (actual, expected, message, operator)](#apidoc.element.chai.assert.fail)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>frozen (obj, msg)](#apidoc.element.chai.assert.frozen)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>ifError (val)](#apidoc.element.chai.assert.ifError)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>include (exp, inc, msg)](#apidoc.element.chai.assert.include)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>includeDeepMembers (superset, subset, msg)](#apidoc.element.chai.assert.includeDeepMembers)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>includeMembers (superset, subset, msg)](#apidoc.element.chai.assert.includeMembers)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>increases (fn, obj, prop)](#apidoc.element.chai.assert.increases)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>instanceOf (val, type, msg)](#apidoc.element.chai.assert.instanceOf)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isAbove (val, abv, msg)](#apidoc.element.chai.assert.isAbove)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isArray (val, msg)](#apidoc.element.chai.assert.isArray)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isAtLeast (val, atlst, msg)](#apidoc.element.chai.assert.isAtLeast)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isAtMost (val, atmst, msg)](#apidoc.element.chai.assert.isAtMost)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isBelow (val, blw, msg)](#apidoc.element.chai.assert.isBelow)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isBoolean (val, msg)](#apidoc.element.chai.assert.isBoolean)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isDefined (val, msg)](#apidoc.element.chai.assert.isDefined)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isExtensible (obj, msg)](#apidoc.element.chai.assert.isExtensible)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isFalse (val, msg)](#apidoc.element.chai.assert.isFalse)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isFrozen (obj, msg)](#apidoc.element.chai.assert.isFrozen)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isFunction (val, msg)](#apidoc.element.chai.assert.isFunction)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNaN (val, msg)](#apidoc.element.chai.assert.isNaN)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotArray (val, msg)](#apidoc.element.chai.assert.isNotArray)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotBoolean (val, msg)](#apidoc.element.chai.assert.isNotBoolean)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotExtensible (obj, msg)](#apidoc.element.chai.assert.isNotExtensible)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotFalse (val, msg)](#apidoc.element.chai.assert.isNotFalse)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotFrozen (obj, msg)](#apidoc.element.chai.assert.isNotFrozen)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotFunction (val, msg)](#apidoc.element.chai.assert.isNotFunction)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotNaN (val, msg)](#apidoc.element.chai.assert.isNotNaN)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotNull (val, msg)](#apidoc.element.chai.assert.isNotNull)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotNumber (val, msg)](#apidoc.element.chai.assert.isNotNumber)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotObject (val, msg)](#apidoc.element.chai.assert.isNotObject)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotOk (val, msg)](#apidoc.element.chai.assert.isNotOk)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotSealed (obj, msg)](#apidoc.element.chai.assert.isNotSealed)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotString (val, msg)](#apidoc.element.chai.assert.isNotString)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNotTrue (val, msg)](#apidoc.element.chai.assert.isNotTrue)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNull (val, msg)](#apidoc.element.chai.assert.isNull)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isNumber (val, msg)](#apidoc.element.chai.assert.isNumber)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isObject (val, msg)](#apidoc.element.chai.assert.isObject)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isOk (val, msg)](#apidoc.element.chai.assert.isOk)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isSealed (obj, msg)](#apidoc.element.chai.assert.isSealed)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isString (val, msg)](#apidoc.element.chai.assert.isString)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isTrue (val, msg)](#apidoc.element.chai.assert.isTrue)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>isUndefined (val, msg)](#apidoc.element.chai.assert.isUndefined)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>lengthOf (exp, len, msg)](#apidoc.element.chai.assert.lengthOf)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>match (exp, re, msg)](#apidoc.element.chai.assert.match)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notDeepEqual (act, exp, msg)](#apidoc.element.chai.assert.notDeepEqual)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notDeepProperty (obj, prop, msg)](#apidoc.element.chai.assert.notDeepProperty)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notEqual (act, exp, msg)](#apidoc.element.chai.assert.notEqual)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notExtensible (obj, msg)](#apidoc.element.chai.assert.notExtensible)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notFrozen (obj, msg)](#apidoc.element.chai.assert.notFrozen)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notInclude (exp, inc, msg)](#apidoc.element.chai.assert.notInclude)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notInstanceOf (val, type, msg)](#apidoc.element.chai.assert.notInstanceOf)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notMatch (exp, re, msg)](#apidoc.element.chai.assert.notMatch)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notOk (val, msg)](#apidoc.element.chai.assert.notOk)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notProperty (obj, prop, msg)](#apidoc.element.chai.assert.notProperty)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notSealed (obj, msg)](#apidoc.element.chai.assert.notSealed)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notStrictEqual (act, exp, msg)](#apidoc.element.chai.assert.notStrictEqual)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>notTypeOf (val, type, msg)](#apidoc.element.chai.assert.notTypeOf)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>ok (val, msg)](#apidoc.element.chai.assert.ok)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>oneOf (inList, list, msg)](#apidoc.element.chai.assert.oneOf)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>operator (val, operator, val2, msg)](#apidoc.element.chai.assert.operator)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>property (obj, prop, msg)](#apidoc.element.chai.assert.property)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>propertyNotVal (obj, prop, val, msg)](#apidoc.element.chai.assert.propertyNotVal)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>propertyVal (obj, prop, val, msg)](#apidoc.element.chai.assert.propertyVal)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>sameDeepMembers (set1, set2, msg)](#apidoc.element.chai.assert.sameDeepMembers)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>sameMembers (set1, set2, msg)](#apidoc.element.chai.assert.sameMembers)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>sealed (obj, msg)](#apidoc.element.chai.assert.sealed)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>strictEqual (act, exp, msg)](#apidoc.element.chai.assert.strictEqual)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>throw (fn, errt, errs, msg)](#apidoc.element.chai.assert.throw)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>throws (fn, errt, errs, msg)](#apidoc.element.chai.assert.throws)
1.  [function <span class="apidocSignatureSpan">chai.assert.</span>typeOf (val, type, msg)](#apidoc.element.chai.assert.typeOf)

#### [module chai.expect](#apidoc.module.chai.expect)
1.  [function <span class="apidocSignatureSpan">chai.</span>expect (val, message)](#apidoc.element.chai.expect.expect)
1.  [function <span class="apidocSignatureSpan">chai.expect.</span>fail (actual, expected, message, operator)](#apidoc.element.chai.expect.fail)

#### [module chai.util](#apidoc.module.chai.util)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>addChainableMethod (ctx, name, method, chainingBehavior)](#apidoc.element.chai.util.addChainableMethod)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>addMethod (ctx, name, method)](#apidoc.element.chai.util.addMethod)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>addProperty (ctx, name, getter)](#apidoc.element.chai.util.addProperty)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>eql (a, b, m)](#apidoc.element.chai.util.eql)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>expectTypes (obj, types)](#apidoc.element.chai.util.expectTypes)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>flag (obj, key, value)](#apidoc.element.chai.util.flag)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>getActual (obj, args)](#apidoc.element.chai.util.getActual)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>getMessage (obj, args)](#apidoc.element.chai.util.getMessage)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>getName (func)](#apidoc.element.chai.util.getName)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>getPathInfo (path, obj)](#apidoc.element.chai.util.getPathInfo)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>getPathValue (path, obj)](#apidoc.element.chai.util.getPathValue)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>hasProperty (name, obj)](#apidoc.element.chai.util.hasProperty)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>inspect (obj, showHidden, depth, colors)](#apidoc.element.chai.util.inspect)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>objDisplay (obj)](#apidoc.element.chai.util.objDisplay)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>overwriteChainableMethod (ctx, name, method, chainingBehavior)](#apidoc.element.chai.util.overwriteChainableMethod)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>overwriteMethod (ctx, name, method)](#apidoc.element.chai.util.overwriteMethod)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>overwriteProperty (ctx, name, getter)](#apidoc.element.chai.util.overwriteProperty)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>test (obj, args)](#apidoc.element.chai.util.test)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>transferFlags (assertion, object, includeAll)](#apidoc.element.chai.util.transferFlags)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>type (obj)](#apidoc.element.chai.util.type)

#### [module chai.util.type](#apidoc.module.chai.util.type)
1.  [function <span class="apidocSignatureSpan">chai.util.</span>type (obj)](#apidoc.element.chai.util.type.type)
1.  [function <span class="apidocSignatureSpan">chai.util.type.</span>Library ()](#apidoc.element.chai.util.type.Library)

#### [module chai.util.type.Library.prototype](#apidoc.module.chai.util.type.Library.prototype)
1.  [function <span class="apidocSignatureSpan">chai.util.type.Library.prototype.</span>define (type, test)](#apidoc.element.chai.util.type.Library.prototype.define)
1.  [function <span class="apidocSignatureSpan">chai.util.type.Library.prototype.</span>of (obj)](#apidoc.element.chai.util.type.Library.prototype.of)
1.  [function <span class="apidocSignatureSpan">chai.util.type.Library.prototype.</span>test (obj, type)](#apidoc.element.chai.util.type.Library.prototype.test)



# <a name="apidoc.module.chai"></a>[module chai](#apidoc.module.chai)

#### <a name="apidoc.element.chai.Assertion"></a>[function <span class="apidocSignatureSpan">chai.</span>Assertion (obj, msg, stack)](#apidoc.element.chai.Assertion)
- description and source-code
```javascript
function Assertion(obj, msg, stack) {
  flag(this, 'ssfi', stack || arguments.callee);
  flag(this, 'object', obj);
  flag(this, 'message', msg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.AssertionError"></a>[function <span class="apidocSignatureSpan">chai.</span>AssertionError (message, _props, ssf)](#apidoc.element.chai.AssertionError)
- description and source-code
```javascript
function AssertionError(message, _props, ssf) {
  var extend = exclude('name', 'message', 'stack', 'constructor', 'toJSON')
    , props = extend(_props || {});

  // default values
  this.message = message || 'Unspecified AssertionError';
  this.showDiff = false;

  // copy from properties
  for (var key in props) {
    this[key] = props[key];
  }

  // capture stack trace
  ssf = ssf || arguments.callee;
  if (ssf && Error.captureStackTrace) {
    Error.captureStackTrace(this, ssf);
  } else {
    try {
      throw new Error();
    } catch(e) {
      this.stack = e.stack;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Should"></a>[function <span class="apidocSignatureSpan">chai.</span>Should ()](#apidoc.element.chai.Should)
- description and source-code
```javascript
function loadShould() {
  // explicitly define this method as function as to have it's name to include as 'ssfi'
  function shouldGetter() {
    if (this instanceof String || this instanceof Number || this instanceof Boolean ) {
      return new Assertion(this.valueOf(), null, shouldGetter);
    }
    return new Assertion(this, null, shouldGetter);
  }
  function shouldSetter(value) {
    // See https://github.com/chaijs/chai/issues/86: this makes
    // 'whatever.should = someValue' actually set 'someValue', which is
    // especially useful for 'global.should = require('chai').should()'.
    //
    // Note that we have to use [[DefineProperty]] instead of [[Put]]
    // since otherwise we would trigger this very setter!
    Object.defineProperty(this, 'should', {
      value: value,
      enumerable: true,
      configurable: true,
      writable: true
    });
  }
  // modify Object.prototype to have 'should'
  Object.defineProperty(Object.prototype, 'should', {
    set: shouldSetter
    , get: shouldGetter
    , configurable: true
  });

  var should = {};

<span class="apidocCodeCommentSpan">  /**
   * ### .fail(actual, expected, [message], [operator])
   *
   * Throw a failure.
   *
   * @name fail
   * @param {Mixed} actual
   * @param {Mixed} expected
   * @param {String} message
   * @param {String} operator
   * @namespace Should
   * @api public
   */
</span>
  should.fail = function (actual, expected, message, operator) {
    message = message || 'should.fail()';
    throw new chai.AssertionError(message, {
        actual: actual
      , expected: expected
      , operator: operator
    }, should.fail);
  };

  /**
   * ### .equal(actual, expected, [message])
   *
   * Asserts non-strict equality ('==') of 'actual' and 'expected'.
   *
   *     should.equal(3, '3', '== coerces values to strings');
   *
   * @name equal
   * @param {Mixed} actual
   * @param {Mixed} expected
   * @param {String} message
   * @namespace Should
   * @api public
   */

  should.equal = function (val1, val2, msg) {
    new Assertion(val1, msg).to.equal(val2);
  };

  /**
   * ### .throw(function, [constructor/string/regexp], [string/regexp], [message])
   *
   * Asserts that 'function' will throw an error that is an instance of
   * 'constructor', or alternately that it will throw an error with message
   * matching 'regexp'.
   *
   *     should.throw(fn, 'function throws a reference error');
   *     should.throw(fn, /function throws a reference error/);
   *     should.throw(fn, ReferenceError);
   *     should.throw(fn, ReferenceError, 'function throws a reference error');
   *     should.throw(fn, ReferenceError, /function throws a reference error/);
   *
   * @name throw
   * @alias Throw
   * @param {Function} function
   * @param {ErrorConstructor} constructor
   * @param {RegExp} regexp
   * @param {String} message
   * @see https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Error#Error_types
   * @namespace Should
   * @api public
   */

  should.Throw = function (fn, errt, errs, msg) {
    new Assertion(fn, msg).to.Throw(errt, errs);
  };

  /**
   * ### .exist
   *
   * Asserts that the target is neither 'null' nor 'undefined'.
   *
   *     var foo = 'hi';
   *
   *     should.exist(foo, 'foo exists');
   *
   * @name exist
   * @namespace Should
   * @api public
   */

  should.exist = function (val, msg) {
    new Assertion(val, msg).to.exist;
  }

  // negation
  should.not = {}

  /**
   * ### .not.equal(actual, expected, [message])
   *
   * Asserts non-strict inequality ('!=') of 'actual' and 'expected'.
   *
   *     should.not.equal(3, 4, 'these numbers are not equal');
   *
   * @name not.equal
   * @param {Mixed} actual
   * @param {Mixed} expected
   * @param {String} message
   * @namespace Should
   * @api public
   */

  should.not.equal = function (val1, val2, msg) {
    new Assertion(val1, msg).to.not.equal(val2);
  };

  /**
   * ### .throw(function, [constructor/regexp], [message])
   *
   * Asserts that 'function' will _not_ throw an error that is an instance of
   * 'constructor', or alternately that it will not throw an er ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert"></a>[function <span class="apidocSignatureSpan">chai.</span>assert (express, errmsg)](#apidoc.element.chai.assert)
- description and source-code
```javascript
assert = function (express, errmsg) {
  var test = new Assertion(null, null, chai.assert);
  test.assert(
      express
    , errmsg
    , '[ negation message unavailable ]'
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.expect"></a>[function <span class="apidocSignatureSpan">chai.</span>expect (val, message)](#apidoc.element.chai.expect)
- description and source-code
```javascript
expect = function (val, message) {
  return new chai.Assertion(val, message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.should"></a>[function <span class="apidocSignatureSpan">chai.</span>should ()](#apidoc.element.chai.should)
- description and source-code
```javascript
function loadShould() {
  // explicitly define this method as function as to have it's name to include as 'ssfi'
  function shouldGetter() {
    if (this instanceof String || this instanceof Number || this instanceof Boolean ) {
      return new Assertion(this.valueOf(), null, shouldGetter);
    }
    return new Assertion(this, null, shouldGetter);
  }
  function shouldSetter(value) {
    // See https://github.com/chaijs/chai/issues/86: this makes
    // 'whatever.should = someValue' actually set 'someValue', which is
    // especially useful for 'global.should = require('chai').should()'.
    //
    // Note that we have to use [[DefineProperty]] instead of [[Put]]
    // since otherwise we would trigger this very setter!
    Object.defineProperty(this, 'should', {
      value: value,
      enumerable: true,
      configurable: true,
      writable: true
    });
  }
  // modify Object.prototype to have 'should'
  Object.defineProperty(Object.prototype, 'should', {
    set: shouldSetter
    , get: shouldGetter
    , configurable: true
  });

  var should = {};

<span class="apidocCodeCommentSpan">  /**
   * ### .fail(actual, expected, [message], [operator])
   *
   * Throw a failure.
   *
   * @name fail
   * @param {Mixed} actual
   * @param {Mixed} expected
   * @param {String} message
   * @param {String} operator
   * @namespace Should
   * @api public
   */
</span>
  should.fail = function (actual, expected, message, operator) {
    message = message || 'should.fail()';
    throw new chai.AssertionError(message, {
        actual: actual
      , expected: expected
      , operator: operator
    }, should.fail);
  };

  /**
   * ### .equal(actual, expected, [message])
   *
   * Asserts non-strict equality ('==') of 'actual' and 'expected'.
   *
   *     should.equal(3, '3', '== coerces values to strings');
   *
   * @name equal
   * @param {Mixed} actual
   * @param {Mixed} expected
   * @param {String} message
   * @namespace Should
   * @api public
   */

  should.equal = function (val1, val2, msg) {
    new Assertion(val1, msg).to.equal(val2);
  };

  /**
   * ### .throw(function, [constructor/string/regexp], [string/regexp], [message])
   *
   * Asserts that 'function' will throw an error that is an instance of
   * 'constructor', or alternately that it will throw an error with message
   * matching 'regexp'.
   *
   *     should.throw(fn, 'function throws a reference error');
   *     should.throw(fn, /function throws a reference error/);
   *     should.throw(fn, ReferenceError);
   *     should.throw(fn, ReferenceError, 'function throws a reference error');
   *     should.throw(fn, ReferenceError, /function throws a reference error/);
   *
   * @name throw
   * @alias Throw
   * @param {Function} function
   * @param {ErrorConstructor} constructor
   * @param {RegExp} regexp
   * @param {String} message
   * @see https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Error#Error_types
   * @namespace Should
   * @api public
   */

  should.Throw = function (fn, errt, errs, msg) {
    new Assertion(fn, msg).to.Throw(errt, errs);
  };

  /**
   * ### .exist
   *
   * Asserts that the target is neither 'null' nor 'undefined'.
   *
   *     var foo = 'hi';
   *
   *     should.exist(foo, 'foo exists');
   *
   * @name exist
   * @namespace Should
   * @api public
   */

  should.exist = function (val, msg) {
    new Assertion(val, msg).to.exist;
  }

  // negation
  should.not = {}

  /**
   * ### .not.equal(actual, expected, [message])
   *
   * Asserts non-strict inequality ('!=') of 'actual' and 'expected'.
   *
   *     should.not.equal(3, 4, 'these numbers are not equal');
   *
   * @name not.equal
   * @param {Mixed} actual
   * @param {Mixed} expected
   * @param {String} message
   * @namespace Should
   * @api public
   */

  should.not.equal = function (val1, val2, msg) {
    new Assertion(val1, msg).to.not.equal(val2);
  };

  /**
   * ### .throw(function, [constructor/regexp], [message])
   *
   * Asserts that 'function' will _not_ throw an error that is an instance of
   * 'constructor', or alternately that it will not throw an er ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.use"></a>[function <span class="apidocSignatureSpan">chai.</span>use (fn)](#apidoc.element.chai.use)
- description and source-code
```javascript
use = function (fn) {
  if (!~used.indexOf(fn)) {
    fn(this, util);
    used.push(fn);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.type"></a>[function <span class="apidocSignatureSpan">chai.</span>util.type (obj)](#apidoc.element.chai.util.type)
- description and source-code
```javascript
function getType(obj) {
  var type = Object.prototype.toString.call(obj).match(objectTypeRegexp)[1].toLowerCase();
  // Let "new String('')" return 'object'
  if (typeof Promise === 'function' && obj instanceof Promise) return 'promise';
  // PhantomJS has type "DOMWindow" for null
  if (obj === null) return 'null';
  // PhantomJS has type "DOMWindow" for undefined
  if (obj === undefined) return 'undefined';
  return type;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.Assertion"></a>[module chai.Assertion](#apidoc.module.chai.Assertion)

#### <a name="apidoc.element.chai.Assertion.Assertion"></a>[function <span class="apidocSignatureSpan">chai.</span>Assertion (obj, msg, stack)](#apidoc.element.chai.Assertion.Assertion)
- description and source-code
```javascript
function Assertion(obj, msg, stack) {
  flag(this, 'ssfi', stack || arguments.callee);
  flag(this, 'object', obj);
  flag(this, 'message', msg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.addChainableMethod"></a>[function <span class="apidocSignatureSpan">chai.Assertion.</span>addChainableMethod (name, fn, chainingBehavior)](#apidoc.element.chai.Assertion.addChainableMethod)
- description and source-code
```javascript
addChainableMethod = function (name, fn, chainingBehavior) {
  util.addChainableMethod(this.prototype, name, fn, chainingBehavior);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.addMethod"></a>[function <span class="apidocSignatureSpan">chai.Assertion.</span>addMethod (name, fn)](#apidoc.element.chai.Assertion.addMethod)
- description and source-code
```javascript
addMethod = function (name, fn) {
  util.addMethod(this.prototype, name, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.addProperty"></a>[function <span class="apidocSignatureSpan">chai.Assertion.</span>addProperty (name, fn)](#apidoc.element.chai.Assertion.addProperty)
- description and source-code
```javascript
addProperty = function (name, fn) {
  util.addProperty(this.prototype, name, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.overwriteChainableMethod"></a>[function <span class="apidocSignatureSpan">chai.Assertion.</span>overwriteChainableMethod (name, fn, chainingBehavior)](#apidoc.element.chai.Assertion.overwriteChainableMethod)
- description and source-code
```javascript
overwriteChainableMethod = function (name, fn, chainingBehavior) {
  util.overwriteChainableMethod(this.prototype, name, fn, chainingBehavior);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.overwriteMethod"></a>[function <span class="apidocSignatureSpan">chai.Assertion.</span>overwriteMethod (name, fn)](#apidoc.element.chai.Assertion.overwriteMethod)
- description and source-code
```javascript
overwriteMethod = function (name, fn) {
  util.overwriteMethod(this.prototype, name, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.overwriteProperty"></a>[function <span class="apidocSignatureSpan">chai.Assertion.</span>overwriteProperty (name, fn)](#apidoc.element.chai.Assertion.overwriteProperty)
- description and source-code
```javascript
overwriteProperty = function (name, fn) {
  util.overwriteProperty(this.prototype, name, fn);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.Assertion.prototype"></a>[module chai.Assertion.prototype](#apidoc.module.chai.Assertion.prototype)

#### <a name="apidoc.element.chai.Assertion.prototype.Throw"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>Throw ()](#apidoc.element.chai.Assertion.prototype.Throw)
- description and source-code
```javascript
Throw = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.above"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>above ()](#apidoc.element.chai.Assertion.prototype.above)
- description and source-code
```javascript
above = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.approximately"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>approximately ()](#apidoc.element.chai.Assertion.prototype.approximately)
- description and source-code
```javascript
approximately = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.assert"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>assert (expr, msg, negateMsg, expected, _actual, showDiff)](#apidoc.element.chai.Assertion.prototype.assert)
- description and source-code
```javascript
assert = function (expr, msg, negateMsg, expected, _actual, showDiff) {
  var ok = util.test(this, arguments);
  if (true !== showDiff) showDiff = false;
  if (true !== config.showDiff) showDiff = false;

  if (!ok) {
    var msg = util.getMessage(this, arguments)
      , actual = util.getActual(this, arguments);
    throw new AssertionError(msg, {
        actual: actual
      , expected: expected
      , showDiff: showDiff
    }, (config.includeStack) ? this.assert : flag(this, 'ssfi'));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.below"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>below ()](#apidoc.element.chai.Assertion.prototype.below)
- description and source-code
```javascript
below = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.closeTo"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>closeTo ()](#apidoc.element.chai.Assertion.prototype.closeTo)
- description and source-code
```javascript
closeTo = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.eq"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>eq ()](#apidoc.element.chai.Assertion.prototype.eq)
- description and source-code
```javascript
eq = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.eql"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>eql ()](#apidoc.element.chai.Assertion.prototype.eql)
- description and source-code
```javascript
eql = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.eqls"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>eqls ()](#apidoc.element.chai.Assertion.prototype.eqls)
- description and source-code
```javascript
eqls = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.equal"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>equal ()](#apidoc.element.chai.Assertion.prototype.equal)
- description and source-code
```javascript
equal = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.equals"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>equals ()](#apidoc.element.chai.Assertion.prototype.equals)
- description and source-code
```javascript
equals = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.greaterThan"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>greaterThan ()](#apidoc.element.chai.Assertion.prototype.greaterThan)
- description and source-code
```javascript
greaterThan = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.gt"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>gt ()](#apidoc.element.chai.Assertion.prototype.gt)
- description and source-code
```javascript
gt = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.gte"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>gte ()](#apidoc.element.chai.Assertion.prototype.gte)
- description and source-code
```javascript
gte = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.haveOwnProperty"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>haveOwnProperty ()](#apidoc.element.chai.Assertion.prototype.haveOwnProperty)
- description and source-code
```javascript
haveOwnProperty = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.haveOwnPropertyDescriptor"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>haveOwnPropertyDescriptor ()](#apidoc.element.chai.Assertion.prototype.haveOwnPropertyDescriptor)
- description and source-code
```javascript
haveOwnPropertyDescriptor = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.instanceOf"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>instanceOf ()](#apidoc.element.chai.Assertion.prototype.instanceOf)
- description and source-code
```javascript
instanceOf = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.instanceof"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>instanceof ()](#apidoc.element.chai.Assertion.prototype.instanceof)
- description and source-code
```javascript
instanceof = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.key"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>key ()](#apidoc.element.chai.Assertion.prototype.key)
- description and source-code
```javascript
key = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.keys"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>keys ()](#apidoc.element.chai.Assertion.prototype.keys)
- description and source-code
```javascript
keys = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.least"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>least ()](#apidoc.element.chai.Assertion.prototype.least)
- description and source-code
```javascript
least = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.lengthOf"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lengthOf ()](#apidoc.element.chai.Assertion.prototype.lengthOf)
- description and source-code
```javascript
lengthOf = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.lessThan"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lessThan ()](#apidoc.element.chai.Assertion.prototype.lessThan)
- description and source-code
```javascript
lessThan = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.lt"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lt ()](#apidoc.element.chai.Assertion.prototype.lt)
- description and source-code
```javascript
lt = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.lte"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>lte ()](#apidoc.element.chai.Assertion.prototype.lte)
- description and source-code
```javascript
lte = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.match"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>match ()](#apidoc.element.chai.Assertion.prototype.match)
- description and source-code
```javascript
match = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.matches"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>matches ()](#apidoc.element.chai.Assertion.prototype.matches)
- description and source-code
```javascript
matches = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.members"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>members ()](#apidoc.element.chai.Assertion.prototype.members)
- description and source-code
```javascript
members = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.most"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>most ()](#apidoc.element.chai.Assertion.prototype.most)
- description and source-code
```javascript
most = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.oneOf"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>oneOf ()](#apidoc.element.chai.Assertion.prototype.oneOf)
- description and source-code
```javascript
oneOf = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.ownProperty"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>ownProperty ()](#apidoc.element.chai.Assertion.prototype.ownProperty)
- description and source-code
```javascript
ownProperty = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.ownPropertyDescriptor"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>ownPropertyDescriptor ()](#apidoc.element.chai.Assertion.prototype.ownPropertyDescriptor)
- description and source-code
```javascript
ownPropertyDescriptor = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.property"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>property ()](#apidoc.element.chai.Assertion.prototype.property)
- description and source-code
```javascript
property = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.respondTo"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>respondTo ()](#apidoc.element.chai.Assertion.prototype.respondTo)
- description and source-code
```javascript
respondTo = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.respondsTo"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>respondsTo ()](#apidoc.element.chai.Assertion.prototype.respondsTo)
- description and source-code
```javascript
respondsTo = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.satisfies"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>satisfies ()](#apidoc.element.chai.Assertion.prototype.satisfies)
- description and source-code
```javascript
satisfies = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.satisfy"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>satisfy ()](#apidoc.element.chai.Assertion.prototype.satisfy)
- description and source-code
```javascript
satisfy = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.string"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>string ()](#apidoc.element.chai.Assertion.prototype.string)
- description and source-code
```javascript
string = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.throw"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>throw ()](#apidoc.element.chai.Assertion.prototype.throw)
- description and source-code
```javascript
throw = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.throws"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>throws ()](#apidoc.element.chai.Assertion.prototype.throws)
- description and source-code
```javascript
throws = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.Assertion.prototype.within"></a>[function <span class="apidocSignatureSpan">chai.Assertion.prototype.</span>within ()](#apidoc.element.chai.Assertion.prototype.within)
- description and source-code
```javascript
within = function () {
  var old_ssfi = flag(this, 'ssfi');
  if (old_ssfi && config.includeStack === false)
    flag(this, 'ssfi', ctx[name]);
  var result = method.apply(this, arguments);
  return result === undefined ? this : result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.AssertionError"></a>[module chai.AssertionError](#apidoc.module.chai.AssertionError)

#### <a name="apidoc.element.chai.AssertionError.AssertionError"></a>[function <span class="apidocSignatureSpan">chai.</span>AssertionError (message, _props, ssf)](#apidoc.element.chai.AssertionError.AssertionError)
- description and source-code
```javascript
function AssertionError(message, _props, ssf) {
  var extend = exclude('name', 'message', 'stack', 'constructor', 'toJSON')
    , props = extend(_props || {});

  // default values
  this.message = message || 'Unspecified AssertionError';
  this.showDiff = false;

  // copy from properties
  for (var key in props) {
    this[key] = props[key];
  }

  // capture stack trace
  ssf = ssf || arguments.callee;
  if (ssf && Error.captureStackTrace) {
    Error.captureStackTrace(this, ssf);
  } else {
    try {
      throw new Error();
    } catch(e) {
      this.stack = e.stack;
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.AssertionError.prototype"></a>[module chai.AssertionError.prototype](#apidoc.module.chai.AssertionError.prototype)

#### <a name="apidoc.element.chai.AssertionError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">chai.AssertionError.prototype.</span>constructor (message, _props, ssf)](#apidoc.element.chai.AssertionError.prototype.constructor)
- description and source-code
```javascript
function AssertionError(message, _props, ssf) {
  var extend = exclude('name', 'message', 'stack', 'constructor', 'toJSON')
    , props = extend(_props || {});

  // default values
  this.message = message || 'Unspecified AssertionError';
  this.showDiff = false;

  // copy from properties
  for (var key in props) {
    this[key] = props[key];
  }

  // capture stack trace
  ssf = ssf || arguments.callee;
  if (ssf && Error.captureStackTrace) {
    Error.captureStackTrace(this, ssf);
  } else {
    try {
      throw new Error();
    } catch(e) {
      this.stack = e.stack;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.AssertionError.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">chai.AssertionError.prototype.</span>toJSON (stack)](#apidoc.element.chai.AssertionError.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (stack) {
  var extend = exclude('constructor', 'toJSON', 'stack')
    , props = extend({ name: this.name }, this);

  // include stack if exists and not turned off
  if (false !== stack && this.stack) {
    props.stack = this.stack;
  }

  return props;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.assert"></a>[module chai.assert](#apidoc.module.chai.assert)

#### <a name="apidoc.element.chai.assert.assert"></a>[function <span class="apidocSignatureSpan">chai.</span>assert (express, errmsg)](#apidoc.element.chai.assert.assert)
- description and source-code
```javascript
assert = function (express, errmsg) {
  var test = new Assertion(null, null, chai.assert);
  test.assert(
      express
    , errmsg
    , '[ negation message unavailable ]'
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.Throw"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>Throw (fn, errt, errs, msg)](#apidoc.element.chai.assert.Throw)
- description and source-code
```javascript
Throw = function (fn, errt, errs, msg) {
  if ('string' === typeof errt || errt instanceof RegExp) {
    errs = errt;
    errt = null;
  }

  var assertErr = new Assertion(fn, msg).to.throw(errt, errs);
  return flag(assertErr, 'object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.approximately"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>approximately (act, exp, delta, msg)](#apidoc.element.chai.assert.approximately)
- description and source-code
```javascript
approximately = function (act, exp, delta, msg) {
  new Assertion(act, msg).to.be.approximately(exp, delta);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.changes"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>changes (fn, obj, prop)](#apidoc.element.chai.assert.changes)
- description and source-code
```javascript
changes = function (fn, obj, prop) {
  new Assertion(fn).to.change(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.closeTo"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>closeTo (act, exp, delta, msg)](#apidoc.element.chai.assert.closeTo)
- description and source-code
```javascript
closeTo = function (act, exp, delta, msg) {
  new Assertion(act, msg).to.be.closeTo(exp, delta);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.decreases"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>decreases (fn, obj, prop)](#apidoc.element.chai.assert.decreases)
- description and source-code
```javascript
decreases = function (fn, obj, prop) {
  new Assertion(fn).to.decrease(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.deepEqual"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>deepEqual (act, exp, msg)](#apidoc.element.chai.assert.deepEqual)
- description and source-code
```javascript
deepEqual = function (act, exp, msg) {
  new Assertion(act, msg).to.eql(exp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.deepProperty"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>deepProperty (obj, prop, msg)](#apidoc.element.chai.assert.deepProperty)
- description and source-code
```javascript
deepProperty = function (obj, prop, msg) {
  new Assertion(obj, msg).to.have.deep.property(prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.deepPropertyNotVal"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>deepPropertyNotVal (obj, prop, val, msg)](#apidoc.element.chai.assert.deepPropertyNotVal)
- description and source-code
```javascript
deepPropertyNotVal = function (obj, prop, val, msg) {
  new Assertion(obj, msg).to.not.have.deep.property(prop, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.deepPropertyVal"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>deepPropertyVal (obj, prop, val, msg)](#apidoc.element.chai.assert.deepPropertyVal)
- description and source-code
```javascript
deepPropertyVal = function (obj, prop, val, msg) {
  new Assertion(obj, msg).to.have.deep.property(prop, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.doesNotChange"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>doesNotChange (fn, obj, prop)](#apidoc.element.chai.assert.doesNotChange)
- description and source-code
```javascript
doesNotChange = function (fn, obj, prop) {
  new Assertion(fn).to.not.change(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.doesNotDecrease"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>doesNotDecrease (fn, obj, prop)](#apidoc.element.chai.assert.doesNotDecrease)
- description and source-code
```javascript
doesNotDecrease = function (fn, obj, prop) {
  new Assertion(fn).to.not.decrease(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.doesNotIncrease"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>doesNotIncrease (fn, obj, prop)](#apidoc.element.chai.assert.doesNotIncrease)
- description and source-code
```javascript
doesNotIncrease = function (fn, obj, prop) {
  new Assertion(fn).to.not.increase(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.doesNotThrow"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>doesNotThrow (fn, type, msg)](#apidoc.element.chai.assert.doesNotThrow)
- description and source-code
```javascript
doesNotThrow = function (fn, type, msg) {
  if ('string' === typeof type) {
    msg = type;
    type = null;
  }

  new Assertion(fn, msg).to.not.Throw(type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.equal"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>equal (act, exp, msg)](#apidoc.element.chai.assert.equal)
- description and source-code
```javascript
equal = function (act, exp, msg) {
  var test = new Assertion(act, msg, assert.equal);

  test.assert(
      exp == flag(test, 'object')
    , 'expected #{this} to equal #{exp}'
    , 'expected #{this} to not equal #{act}'
    , exp
    , act
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.extensible"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>extensible (obj, msg)](#apidoc.element.chai.assert.extensible)
- description and source-code
```javascript
extensible = function (obj, msg) {
  new Assertion(obj, msg).to.be.extensible;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.fail"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>fail (actual, expected, message, operator)](#apidoc.element.chai.assert.fail)
- description and source-code
```javascript
fail = function (actual, expected, message, operator) {
  message = message || 'assert.fail()';
  throw new chai.AssertionError(message, {
      actual: actual
    , expected: expected
    , operator: operator
  }, assert.fail);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.frozen"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>frozen (obj, msg)](#apidoc.element.chai.assert.frozen)
- description and source-code
```javascript
frozen = function (obj, msg) {
  new Assertion(obj, msg).to.be.frozen;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.ifError"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>ifError (val)](#apidoc.element.chai.assert.ifError)
- description and source-code
```javascript
ifError = function (val) {
  if (val) {
    throw(val);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.include"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>include (exp, inc, msg)](#apidoc.element.chai.assert.include)
- description and source-code
```javascript
include = function (exp, inc, msg) {
  new Assertion(exp, msg, assert.include).include(inc);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.includeDeepMembers"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>includeDeepMembers (superset, subset, msg)](#apidoc.element.chai.assert.includeDeepMembers)
- description and source-code
```javascript
includeDeepMembers = function (superset, subset, msg) {
  new Assertion(superset, msg).to.include.deep.members(subset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.includeMembers"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>includeMembers (superset, subset, msg)](#apidoc.element.chai.assert.includeMembers)
- description and source-code
```javascript
includeMembers = function (superset, subset, msg) {
  new Assertion(superset, msg).to.include.members(subset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.increases"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>increases (fn, obj, prop)](#apidoc.element.chai.assert.increases)
- description and source-code
```javascript
increases = function (fn, obj, prop) {
  new Assertion(fn).to.increase(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.instanceOf"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>instanceOf (val, type, msg)](#apidoc.element.chai.assert.instanceOf)
- description and source-code
```javascript
instanceOf = function (val, type, msg) {
  new Assertion(val, msg).to.be.instanceOf(type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isAbove"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isAbove (val, abv, msg)](#apidoc.element.chai.assert.isAbove)
- description and source-code
```javascript
isAbove = function (val, abv, msg) {
  new Assertion(val, msg).to.be.above(abv);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isArray"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isArray (val, msg)](#apidoc.element.chai.assert.isArray)
- description and source-code
```javascript
isArray = function (val, msg) {
  new Assertion(val, msg).to.be.an('array');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isAtLeast"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isAtLeast (val, atlst, msg)](#apidoc.element.chai.assert.isAtLeast)
- description and source-code
```javascript
isAtLeast = function (val, atlst, msg) {
  new Assertion(val, msg).to.be.least(atlst);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isAtMost"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isAtMost (val, atmst, msg)](#apidoc.element.chai.assert.isAtMost)
- description and source-code
```javascript
isAtMost = function (val, atmst, msg) {
  new Assertion(val, msg).to.be.most(atmst);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isBelow"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isBelow (val, blw, msg)](#apidoc.element.chai.assert.isBelow)
- description and source-code
```javascript
isBelow = function (val, blw, msg) {
  new Assertion(val, msg).to.be.below(blw);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isBoolean"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isBoolean (val, msg)](#apidoc.element.chai.assert.isBoolean)
- description and source-code
```javascript
isBoolean = function (val, msg) {
  new Assertion(val, msg).to.be.a('boolean');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isDefined"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isDefined (val, msg)](#apidoc.element.chai.assert.isDefined)
- description and source-code
```javascript
isDefined = function (val, msg) {
  new Assertion(val, msg).to.not.equal(undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isExtensible"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isExtensible (obj, msg)](#apidoc.element.chai.assert.isExtensible)
- description and source-code
```javascript
isExtensible = function (obj, msg) {
  new Assertion(obj, msg).to.be.extensible;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isFalse"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isFalse (val, msg)](#apidoc.element.chai.assert.isFalse)
- description and source-code
```javascript
isFalse = function (val, msg) {
  new Assertion(val, msg).is['false'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isFrozen"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isFrozen (obj, msg)](#apidoc.element.chai.assert.isFrozen)
- description and source-code
```javascript
isFrozen = function (obj, msg) {
  new Assertion(obj, msg).to.be.frozen;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isFunction"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isFunction (val, msg)](#apidoc.element.chai.assert.isFunction)
- description and source-code
```javascript
isFunction = function (val, msg) {
  new Assertion(val, msg).to.be.a('function');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNaN"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNaN (val, msg)](#apidoc.element.chai.assert.isNaN)
- description and source-code
```javascript
isNaN = function (val, msg) {
  new Assertion(val, msg).to.be.NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotArray"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotArray (val, msg)](#apidoc.element.chai.assert.isNotArray)
- description and source-code
```javascript
isNotArray = function (val, msg) {
  new Assertion(val, msg).to.not.be.an('array');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotBoolean"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotBoolean (val, msg)](#apidoc.element.chai.assert.isNotBoolean)
- description and source-code
```javascript
isNotBoolean = function (val, msg) {
  new Assertion(val, msg).to.not.be.a('boolean');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotExtensible"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotExtensible (obj, msg)](#apidoc.element.chai.assert.isNotExtensible)
- description and source-code
```javascript
isNotExtensible = function (obj, msg) {
  new Assertion(obj, msg).to.not.be.extensible;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotFalse"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotFalse (val, msg)](#apidoc.element.chai.assert.isNotFalse)
- description and source-code
```javascript
isNotFalse = function (val, msg) {
  new Assertion(val, msg).to.not.equal(false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotFrozen"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotFrozen (obj, msg)](#apidoc.element.chai.assert.isNotFrozen)
- description and source-code
```javascript
isNotFrozen = function (obj, msg) {
  new Assertion(obj, msg).to.not.be.frozen;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotFunction"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotFunction (val, msg)](#apidoc.element.chai.assert.isNotFunction)
- description and source-code
```javascript
isNotFunction = function (val, msg) {
  new Assertion(val, msg).to.not.be.a('function');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotNaN"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotNaN (val, msg)](#apidoc.element.chai.assert.isNotNaN)
- description and source-code
```javascript
isNotNaN = function (val, msg) {
  new Assertion(val, msg).not.to.be.NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotNull"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotNull (val, msg)](#apidoc.element.chai.assert.isNotNull)
- description and source-code
```javascript
isNotNull = function (val, msg) {
  new Assertion(val, msg).to.not.equal(null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotNumber"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotNumber (val, msg)](#apidoc.element.chai.assert.isNotNumber)
- description and source-code
```javascript
isNotNumber = function (val, msg) {
  new Assertion(val, msg).to.not.be.a('number');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotObject"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotObject (val, msg)](#apidoc.element.chai.assert.isNotObject)
- description and source-code
```javascript
isNotObject = function (val, msg) {
  new Assertion(val, msg).to.not.be.a('object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotOk"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotOk (val, msg)](#apidoc.element.chai.assert.isNotOk)
- description and source-code
```javascript
isNotOk = function (val, msg) {
  new Assertion(val, msg).is.not.ok;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotSealed"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotSealed (obj, msg)](#apidoc.element.chai.assert.isNotSealed)
- description and source-code
```javascript
isNotSealed = function (obj, msg) {
  new Assertion(obj, msg).to.not.be.sealed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotString"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotString (val, msg)](#apidoc.element.chai.assert.isNotString)
- description and source-code
```javascript
isNotString = function (val, msg) {
  new Assertion(val, msg).to.not.be.a('string');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNotTrue"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNotTrue (val, msg)](#apidoc.element.chai.assert.isNotTrue)
- description and source-code
```javascript
isNotTrue = function (val, msg) {
  new Assertion(val, msg).to.not.equal(true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNull"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNull (val, msg)](#apidoc.element.chai.assert.isNull)
- description and source-code
```javascript
isNull = function (val, msg) {
  new Assertion(val, msg).to.equal(null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isNumber"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isNumber (val, msg)](#apidoc.element.chai.assert.isNumber)
- description and source-code
```javascript
isNumber = function (val, msg) {
  new Assertion(val, msg).to.be.a('number');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isObject"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isObject (val, msg)](#apidoc.element.chai.assert.isObject)
- description and source-code
```javascript
isObject = function (val, msg) {
  new Assertion(val, msg).to.be.a('object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isOk"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isOk (val, msg)](#apidoc.element.chai.assert.isOk)
- description and source-code
```javascript
isOk = function (val, msg) {
  new Assertion(val, msg).is.ok;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isSealed"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isSealed (obj, msg)](#apidoc.element.chai.assert.isSealed)
- description and source-code
```javascript
isSealed = function (obj, msg) {
  new Assertion(obj, msg).to.be.sealed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isString"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isString (val, msg)](#apidoc.element.chai.assert.isString)
- description and source-code
```javascript
isString = function (val, msg) {
  new Assertion(val, msg).to.be.a('string');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isTrue"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isTrue (val, msg)](#apidoc.element.chai.assert.isTrue)
- description and source-code
```javascript
isTrue = function (val, msg) {
  new Assertion(val, msg).is['true'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.isUndefined"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>isUndefined (val, msg)](#apidoc.element.chai.assert.isUndefined)
- description and source-code
```javascript
isUndefined = function (val, msg) {
  new Assertion(val, msg).to.equal(undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.lengthOf"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>lengthOf (exp, len, msg)](#apidoc.element.chai.assert.lengthOf)
- description and source-code
```javascript
lengthOf = function (exp, len, msg) {
  new Assertion(exp, msg).to.have.length(len);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.match"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>match (exp, re, msg)](#apidoc.element.chai.assert.match)
- description and source-code
```javascript
match = function (exp, re, msg) {
  new Assertion(exp, msg).to.match(re);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notDeepEqual"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notDeepEqual (act, exp, msg)](#apidoc.element.chai.assert.notDeepEqual)
- description and source-code
```javascript
notDeepEqual = function (act, exp, msg) {
  new Assertion(act, msg).to.not.eql(exp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notDeepProperty"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notDeepProperty (obj, prop, msg)](#apidoc.element.chai.assert.notDeepProperty)
- description and source-code
```javascript
notDeepProperty = function (obj, prop, msg) {
  new Assertion(obj, msg).to.not.have.deep.property(prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notEqual"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notEqual (act, exp, msg)](#apidoc.element.chai.assert.notEqual)
- description and source-code
```javascript
notEqual = function (act, exp, msg) {
  var test = new Assertion(act, msg, assert.notEqual);

  test.assert(
      exp != flag(test, 'object')
    , 'expected #{this} to not equal #{exp}'
    , 'expected #{this} to equal #{act}'
    , exp
    , act
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notExtensible"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notExtensible (obj, msg)](#apidoc.element.chai.assert.notExtensible)
- description and source-code
```javascript
notExtensible = function (obj, msg) {
  new Assertion(obj, msg).to.not.be.extensible;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notFrozen"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notFrozen (obj, msg)](#apidoc.element.chai.assert.notFrozen)
- description and source-code
```javascript
notFrozen = function (obj, msg) {
  new Assertion(obj, msg).to.not.be.frozen;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notInclude"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notInclude (exp, inc, msg)](#apidoc.element.chai.assert.notInclude)
- description and source-code
```javascript
notInclude = function (exp, inc, msg) {
  new Assertion(exp, msg, assert.notInclude).not.include(inc);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notInstanceOf"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notInstanceOf (val, type, msg)](#apidoc.element.chai.assert.notInstanceOf)
- description and source-code
```javascript
notInstanceOf = function (val, type, msg) {
  new Assertion(val, msg).to.not.be.instanceOf(type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notMatch"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notMatch (exp, re, msg)](#apidoc.element.chai.assert.notMatch)
- description and source-code
```javascript
notMatch = function (exp, re, msg) {
  new Assertion(exp, msg).to.not.match(re);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notOk"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notOk (val, msg)](#apidoc.element.chai.assert.notOk)
- description and source-code
```javascript
notOk = function (val, msg) {
  new Assertion(val, msg).is.not.ok;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notProperty"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notProperty (obj, prop, msg)](#apidoc.element.chai.assert.notProperty)
- description and source-code
```javascript
notProperty = function (obj, prop, msg) {
  new Assertion(obj, msg).to.not.have.property(prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notSealed"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notSealed (obj, msg)](#apidoc.element.chai.assert.notSealed)
- description and source-code
```javascript
notSealed = function (obj, msg) {
  new Assertion(obj, msg).to.not.be.sealed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notStrictEqual"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notStrictEqual (act, exp, msg)](#apidoc.element.chai.assert.notStrictEqual)
- description and source-code
```javascript
notStrictEqual = function (act, exp, msg) {
  new Assertion(act, msg).to.not.equal(exp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.notTypeOf"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>notTypeOf (val, type, msg)](#apidoc.element.chai.assert.notTypeOf)
- description and source-code
```javascript
notTypeOf = function (val, type, msg) {
  new Assertion(val, msg).to.not.be.a(type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.ok"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>ok (val, msg)](#apidoc.element.chai.assert.ok)
- description and source-code
```javascript
ok = function (val, msg) {
  new Assertion(val, msg).is.ok;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.oneOf"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>oneOf (inList, list, msg)](#apidoc.element.chai.assert.oneOf)
- description and source-code
```javascript
oneOf = function (inList, list, msg) {
  new Assertion(inList, msg).to.be.oneOf(list);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.operator"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>operator (val, operator, val2, msg)](#apidoc.element.chai.assert.operator)
- description and source-code
```javascript
operator = function (val, operator, val2, msg) {
  var ok;
  switch(operator) {
    case '==':
      ok = val == val2;
      break;
    case '===':
      ok = val === val2;
      break;
    case '>':
      ok = val > val2;
      break;
    case '>=':
      ok = val >= val2;
      break;
    case '<':
      ok = val < val2;
      break;
    case '<=':
      ok = val <= val2;
      break;
    case '!=':
      ok = val != val2;
      break;
    case '!==':
      ok = val !== val2;
      break;
    default:
      throw new Error('Invalid operator "' + operator + '"');
  }
  var test = new Assertion(ok, msg);
  test.assert(
      true === flag(test, 'object')
    , 'expected ' + util.inspect(val) + ' to be ' + operator + ' ' + util.inspect(val2)
    , 'expected ' + util.inspect(val) + ' to not be ' + operator + ' ' + util.inspect(val2) );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.property"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>property (obj, prop, msg)](#apidoc.element.chai.assert.property)
- description and source-code
```javascript
property = function (obj, prop, msg) {
  new Assertion(obj, msg).to.have.property(prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.propertyNotVal"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>propertyNotVal (obj, prop, val, msg)](#apidoc.element.chai.assert.propertyNotVal)
- description and source-code
```javascript
propertyNotVal = function (obj, prop, val, msg) {
  new Assertion(obj, msg).to.not.have.property(prop, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.propertyVal"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>propertyVal (obj, prop, val, msg)](#apidoc.element.chai.assert.propertyVal)
- description and source-code
```javascript
propertyVal = function (obj, prop, val, msg) {
  new Assertion(obj, msg).to.have.property(prop, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.sameDeepMembers"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>sameDeepMembers (set1, set2, msg)](#apidoc.element.chai.assert.sameDeepMembers)
- description and source-code
```javascript
sameDeepMembers = function (set1, set2, msg) {
  new Assertion(set1, msg).to.have.same.deep.members(set2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.sameMembers"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>sameMembers (set1, set2, msg)](#apidoc.element.chai.assert.sameMembers)
- description and source-code
```javascript
sameMembers = function (set1, set2, msg) {
  new Assertion(set1, msg).to.have.same.members(set2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.sealed"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>sealed (obj, msg)](#apidoc.element.chai.assert.sealed)
- description and source-code
```javascript
sealed = function (obj, msg) {
  new Assertion(obj, msg).to.be.sealed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.strictEqual"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>strictEqual (act, exp, msg)](#apidoc.element.chai.assert.strictEqual)
- description and source-code
```javascript
strictEqual = function (act, exp, msg) {
  new Assertion(act, msg).to.equal(exp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.throw"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>throw (fn, errt, errs, msg)](#apidoc.element.chai.assert.throw)
- description and source-code
```javascript
throw = function (fn, errt, errs, msg) {
  if ('string' === typeof errt || errt instanceof RegExp) {
    errs = errt;
    errt = null;
  }

  var assertErr = new Assertion(fn, msg).to.throw(errt, errs);
  return flag(assertErr, 'object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.throws"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>throws (fn, errt, errs, msg)](#apidoc.element.chai.assert.throws)
- description and source-code
```javascript
throws = function (fn, errt, errs, msg) {
  if ('string' === typeof errt || errt instanceof RegExp) {
    errs = errt;
    errt = null;
  }

  var assertErr = new Assertion(fn, msg).to.throw(errt, errs);
  return flag(assertErr, 'object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.assert.typeOf"></a>[function <span class="apidocSignatureSpan">chai.assert.</span>typeOf (val, type, msg)](#apidoc.element.chai.assert.typeOf)
- description and source-code
```javascript
typeOf = function (val, type, msg) {
  new Assertion(val, msg).to.be.a(type);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.expect"></a>[module chai.expect](#apidoc.module.chai.expect)

#### <a name="apidoc.element.chai.expect.expect"></a>[function <span class="apidocSignatureSpan">chai.</span>expect (val, message)](#apidoc.element.chai.expect.expect)
- description and source-code
```javascript
expect = function (val, message) {
  return new chai.Assertion(val, message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.expect.fail"></a>[function <span class="apidocSignatureSpan">chai.expect.</span>fail (actual, expected, message, operator)](#apidoc.element.chai.expect.fail)
- description and source-code
```javascript
fail = function (actual, expected, message, operator) {
  message = message || 'expect.fail()';
  throw new chai.AssertionError(message, {
      actual: actual
    , expected: expected
    , operator: operator
  }, chai.expect.fail);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.util"></a>[module chai.util](#apidoc.module.chai.util)

#### <a name="apidoc.element.chai.util.addChainableMethod"></a>[function <span class="apidocSignatureSpan">chai.util.</span>addChainableMethod (ctx, name, method, chainingBehavior)](#apidoc.element.chai.util.addChainableMethod)
- description and source-code
```javascript
addChainableMethod = function (ctx, name, method, chainingBehavior) {
  if (typeof chainingBehavior !== 'function') {
    chainingBehavior = function () { };
  }

  var chainableBehavior = {
      method: method
    , chainingBehavior: chainingBehavior
  };

  // save the methods so we can overwrite them later, if we need to.
  if (!ctx.__methods) {
    ctx.__methods = {};
  }
  ctx.__methods[name] = chainableBehavior;

  Object.defineProperty(ctx, name,
    { get: function () {
        chainableBehavior.chainingBehavior.call(this);

        var assert = function assert() {
          var old_ssfi = flag(this, 'ssfi');
          if (old_ssfi && config.includeStack === false)
            flag(this, 'ssfi', assert);
          var result = chainableBehavior.method.apply(this, arguments);
          return result === undefined ? this : result;
        };

        // Use '__proto__' if available
        if (hasProtoSupport) {
          // Inherit all properties from the object by replacing the 'Function' prototype
          var prototype = assert.__proto__ = Object.create(this);
          // Restore the 'call' and 'apply' methods from 'Function'
          prototype.call = call;
          prototype.apply = apply;
        }
        // Otherwise, redefine all properties (slow!)
        else {
          var asserterNames = Object.getOwnPropertyNames(ctx);
          asserterNames.forEach(function (asserterName) {
            if (!excludeNames.test(asserterName)) {
              var pd = Object.getOwnPropertyDescriptor(ctx, asserterName);
              Object.defineProperty(assert, asserterName, pd);
            }
          });
        }

        transferFlags(this, assert);
        return assert;
      }
    , configurable: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.addMethod"></a>[function <span class="apidocSignatureSpan">chai.util.</span>addMethod (ctx, name, method)](#apidoc.element.chai.util.addMethod)
- description and source-code
```javascript
addMethod = function (ctx, name, method) {
  ctx[name] = function () {
    var old_ssfi = flag(this, 'ssfi');
    if (old_ssfi && config.includeStack === false)
      flag(this, 'ssfi', ctx[name]);
    var result = method.apply(this, arguments);
    return result === undefined ? this : result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.addProperty"></a>[function <span class="apidocSignatureSpan">chai.util.</span>addProperty (ctx, name, getter)](#apidoc.element.chai.util.addProperty)
- description and source-code
```javascript
addProperty = function (ctx, name, getter) {
  Object.defineProperty(ctx, name,
    { get: function addProperty() {
        var old_ssfi = flag(this, 'ssfi');
        if (old_ssfi && config.includeStack === false)
          flag(this, 'ssfi', addProperty);

        var result = getter.call(this);
        return result === undefined ? this : result;
      }
    , configurable: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.eql"></a>[function <span class="apidocSignatureSpan">chai.util.</span>eql (a, b, m)](#apidoc.element.chai.util.eql)
- description and source-code
```javascript
function deepEqual(a, b, m) {
  if (sameValue(a, b)) {
    return true;
  } else if ('date' === type(a)) {
    return dateEqual(a, b);
  } else if ('regexp' === type(a)) {
    return regexpEqual(a, b);
  } else if (Buffer.isBuffer(a)) {
    return bufferEqual(a, b);
  } else if ('arguments' === type(a)) {
    return argumentsEqual(a, b, m);
  } else if (!typeEqual(a, b)) {
    return false;
  } else if (('object' !== type(a) && 'object' !== type(b))
  && ('array' !== type(a) && 'array' !== type(b))) {
    return sameValue(a, b);
  } else {
    return objectEqual(a, b, m);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.expectTypes"></a>[function <span class="apidocSignatureSpan">chai.util.</span>expectTypes (obj, types)](#apidoc.element.chai.util.expectTypes)
- description and source-code
```javascript
expectTypes = function (obj, types) {
  var obj = flag(obj, 'object');
  types = types.map(function (t) { return t.toLowerCase(); });
  types.sort();

  // Transforms ['lorem', 'ipsum'] into 'a lirum, or an ipsum'
  var str = types.map(function (t, index) {
    var art = ~[ 'a', 'e', 'i', 'o', 'u' ].indexOf(t.charAt(0)) ? 'an' : 'a';
    var or = types.length > 1 && index === types.length - 1 ? 'or ' : '';
    return or + art + ' ' + t;
  }).join(', ');

  if (!types.some(function (expected) { return type(obj) === expected; })) {
    throw new AssertionError(
      'object tested must be ' + str + ', but ' + type(obj) + ' given'
    );
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.flag"></a>[function <span class="apidocSignatureSpan">chai.util.</span>flag (obj, key, value)](#apidoc.element.chai.util.flag)
- description and source-code
```javascript
flag = function (obj, key, value) {
  var flags = obj.__flags || (obj.__flags = Object.create(null));
  if (arguments.length === 3) {
    flags[key] = value;
  } else {
    return flags[key];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.getActual"></a>[function <span class="apidocSignatureSpan">chai.util.</span>getActual (obj, args)](#apidoc.element.chai.util.getActual)
- description and source-code
```javascript
getActual = function (obj, args) {
  return args.length > 4 ? args[4] : obj._obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.getMessage"></a>[function <span class="apidocSignatureSpan">chai.util.</span>getMessage (obj, args)](#apidoc.element.chai.util.getMessage)
- description and source-code
```javascript
getMessage = function (obj, args) {
  var negate = flag(obj, 'negate')
    , val = flag(obj, 'object')
    , expected = args[3]
    , actual = getActual(obj, args)
    , msg = negate ? args[2] : args[1]
    , flagMsg = flag(obj, 'message');

  if(typeof msg === "function") msg = msg();
  msg = msg || '';
  msg = msg
    .replace(/#\{this\}/g, function () { return objDisplay(val); })
    .replace(/#\{act\}/g, function () { return objDisplay(actual); })
    .replace(/#\{exp\}/g, function () { return objDisplay(expected); });

  return flagMsg ? flagMsg + ': ' + msg : msg;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.getName"></a>[function <span class="apidocSignatureSpan">chai.util.</span>getName (func)](#apidoc.element.chai.util.getName)
- description and source-code
```javascript
getName = function (func) {
  if (func.name) return func.name;

  var match = /^\s?function ([^(]*)\(/.exec(func);
  return match && match[1] ? match[1] : "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.getPathInfo"></a>[function <span class="apidocSignatureSpan">chai.util.</span>getPathInfo (path, obj)](#apidoc.element.chai.util.getPathInfo)
- description and source-code
```javascript
function getPathInfo(path, obj) {
  var parsed = parsePath(path),
      last = parsed[parsed.length - 1];

  var info = {
    parent: parsed.length > 1 ? _getPathValue(parsed, obj, parsed.length - 1) : obj,
    name: last.p || last.i,
    value: _getPathValue(parsed, obj)
  };
  info.exists = hasProperty(info.name, info.parent);

  return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.getPathValue"></a>[function <span class="apidocSignatureSpan">chai.util.</span>getPathValue (path, obj)](#apidoc.element.chai.util.getPathValue)
- description and source-code
```javascript
getPathValue = function (path, obj) {
  var info = getPathInfo(path, obj);
  return info.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.hasProperty"></a>[function <span class="apidocSignatureSpan">chai.util.</span>hasProperty (name, obj)](#apidoc.element.chai.util.hasProperty)
- description and source-code
```javascript
function hasProperty(name, obj) {
  var ot = type(obj);

  // Bad Object, obviously no props at all
  if(ot === 'null' || ot === 'undefined')
    return false;

  // The 'in' operator does not work with certain literals
  // box these before the check
  if(literals[ot] && typeof obj !== 'object')
    obj = new literals[ot](obj);

  return name in obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.inspect"></a>[function <span class="apidocSignatureSpan">chai.util.</span>inspect (obj, showHidden, depth, colors)](#apidoc.element.chai.util.inspect)
- description and source-code
```javascript
function inspect(obj, showHidden, depth, colors) {
  var ctx = {
    showHidden: showHidden,
    seen: [],
    stylize: function (str) { return str; }
  };
  return formatValue(ctx, obj, (typeof depth === 'undefined' ? 2 : depth));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.objDisplay"></a>[function <span class="apidocSignatureSpan">chai.util.</span>objDisplay (obj)](#apidoc.element.chai.util.objDisplay)
- description and source-code
```javascript
objDisplay = function (obj) {
  var str = inspect(obj)
    , type = Object.prototype.toString.call(obj);

  if (config.truncateThreshold && str.length >= config.truncateThreshold) {
    if (type === '[object Function]') {
      return !obj.name || obj.name === ''
        ? '[Function]'
        : '[Function: ' + obj.name + ']';
    } else if (type === '[object Array]') {
      return '[ Array(' + obj.length + ') ]';
    } else if (type === '[object Object]') {
      var keys = Object.keys(obj)
        , kstr = keys.length > 2
          ? keys.splice(0, 2).join(', ') + ', ...'
          : keys.join(', ');
      return '{ Object (' + kstr + ') }';
    } else {
      return str;
    }
  } else {
    return str;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.overwriteChainableMethod"></a>[function <span class="apidocSignatureSpan">chai.util.</span>overwriteChainableMethod (ctx, name, method, chainingBehavior)](#apidoc.element.chai.util.overwriteChainableMethod)
- description and source-code
```javascript
overwriteChainableMethod = function (ctx, name, method, chainingBehavior) {
  var chainableBehavior = ctx.__methods[name];

  var _chainingBehavior = chainableBehavior.chainingBehavior;
  chainableBehavior.chainingBehavior = function () {
    var result = chainingBehavior(_chainingBehavior).call(this);
    return result === undefined ? this : result;
  };

  var _method = chainableBehavior.method;
  chainableBehavior.method = function () {
    var result = method(_method).apply(this, arguments);
    return result === undefined ? this : result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.overwriteMethod"></a>[function <span class="apidocSignatureSpan">chai.util.</span>overwriteMethod (ctx, name, method)](#apidoc.element.chai.util.overwriteMethod)
- description and source-code
```javascript
overwriteMethod = function (ctx, name, method) {
  var _method = ctx[name]
    , _super = function () { return this; };

  if (_method && 'function' === typeof _method)
    _super = _method;

  ctx[name] = function () {
    var result = method(_super).apply(this, arguments);
    return result === undefined ? this : result;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.overwriteProperty"></a>[function <span class="apidocSignatureSpan">chai.util.</span>overwriteProperty (ctx, name, getter)](#apidoc.element.chai.util.overwriteProperty)
- description and source-code
```javascript
overwriteProperty = function (ctx, name, getter) {
  var _get = Object.getOwnPropertyDescriptor(ctx, name)
    , _super = function () {};

  if (_get && 'function' === typeof _get.get)
    _super = _get.get

  Object.defineProperty(ctx, name,
    { get: function () {
        var result = getter(_super).call(this);
        return result === undefined ? this : result;
      }
    , configurable: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.test"></a>[function <span class="apidocSignatureSpan">chai.util.</span>test (obj, args)](#apidoc.element.chai.util.test)
- description and source-code
```javascript
test = function (obj, args) {
  var negate = flag(obj, 'negate')
    , expr = args[0];
  return negate ? !expr : expr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.transferFlags"></a>[function <span class="apidocSignatureSpan">chai.util.</span>transferFlags (assertion, object, includeAll)](#apidoc.element.chai.util.transferFlags)
- description and source-code
```javascript
transferFlags = function (assertion, object, includeAll) {
  var flags = assertion.__flags || (assertion.__flags = Object.create(null));

  if (!object.__flags) {
    object.__flags = Object.create(null);
  }

  includeAll = arguments.length === 3 ? includeAll : true;

  for (var flag in flags) {
    if (includeAll ||
        (flag !== 'object' && flag !== 'ssfi' && flag != 'message')) {
      object.__flags[flag] = flags[flag];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.type"></a>[function <span class="apidocSignatureSpan">chai.util.</span>type (obj)](#apidoc.element.chai.util.type)
- description and source-code
```javascript
function getType(obj) {
  var type = Object.prototype.toString.call(obj).match(objectTypeRegexp)[1].toLowerCase();
  // Let "new String('')" return 'object'
  if (typeof Promise === 'function' && obj instanceof Promise) return 'promise';
  // PhantomJS has type "DOMWindow" for null
  if (obj === null) return 'null';
  // PhantomJS has type "DOMWindow" for undefined
  if (obj === undefined) return 'undefined';
  return type;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.util.type"></a>[module chai.util.type](#apidoc.module.chai.util.type)

#### <a name="apidoc.element.chai.util.type.type"></a>[function <span class="apidocSignatureSpan">chai.util.</span>type (obj)](#apidoc.element.chai.util.type.type)
- description and source-code
```javascript
function getType(obj) {
  var type = Object.prototype.toString.call(obj).match(objectTypeRegexp)[1].toLowerCase();
  // Let "new String('')" return 'object'
  if (typeof Promise === 'function' && obj instanceof Promise) return 'promise';
  // PhantomJS has type "DOMWindow" for null
  if (obj === null) return 'null';
  // PhantomJS has type "DOMWindow" for undefined
  if (obj === undefined) return 'undefined';
  return type;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.type.Library"></a>[function <span class="apidocSignatureSpan">chai.util.type.</span>Library ()](#apidoc.element.chai.util.type.Library)
- description and source-code
```javascript
function Library() {
  if (!(this instanceof Library)) return new Library();
  this.tests = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chai.util.type.Library.prototype"></a>[module chai.util.type.Library.prototype](#apidoc.module.chai.util.type.Library.prototype)

#### <a name="apidoc.element.chai.util.type.Library.prototype.define"></a>[function <span class="apidocSignatureSpan">chai.util.type.Library.prototype.</span>define (type, test)](#apidoc.element.chai.util.type.Library.prototype.define)
- description and source-code
```javascript
define = function (type, test) {
  if (arguments.length === 1) return this.tests[type];
  this.tests[type] = test;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.type.Library.prototype.of"></a>[function <span class="apidocSignatureSpan">chai.util.type.Library.prototype.</span>of (obj)](#apidoc.element.chai.util.type.Library.prototype.of)
- description and source-code
```javascript
function getType(obj) {
  var type = Object.prototype.toString.call(obj).match(objectTypeRegexp)[1].toLowerCase();
  // Let "new String('')" return 'object'
  if (typeof Promise === 'function' && obj instanceof Promise) return 'promise';
  // PhantomJS has type "DOMWindow" for null
  if (obj === null) return 'null';
  // PhantomJS has type "DOMWindow" for undefined
  if (obj === undefined) return 'undefined';
  return type;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chai.util.type.Library.prototype.test"></a>[function <span class="apidocSignatureSpan">chai.util.type.Library.prototype.</span>test (obj, type)](#apidoc.element.chai.util.type.Library.prototype.test)
- description and source-code
```javascript
test = function (obj, type) {
  if (type === getType(obj)) return true;
  var test = this.tests[type];

  if (test && 'regexp' === getType(test)) {
    return test.test(obj);
  } else if (test && 'function' === getType(test)) {
    return test(obj);
  } else {
    throw new ReferenceError('Type test "' + type + '" not defined or invalid.');
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
