ESLint environments for bem-xjst
================================

[![NPM Status][npm-img]][npm]
[![Travis Status][test-img]][travis]

[npm]:          https://www.npmjs.org/package/eslint-plugin-bem-xjst
[npm-img]:      https://img.shields.io/npm/v/eslint-plugin-bem-xjst.svg

[travis]:       https://travis-ci.org/bem/eslint-plugin-bem-xjst
[test-img]:     https://img.shields.io/travis/blond/eslint-plugin-bem-xjst.svg?label=tests

This plugin includes two ESLint environments:

* `bem-xjst/bemhtml` - for [BEMHTML](https://en.bem.info/technology/bemhtml/v2/rationale/) templates
* `bem-xjst/bemtree` - for [BEMTREE](https://en.bem.info/technology/bemtree/v2/bemtree/) templates

Install
-------

You'll first need to install `ESLint`:

```
$ npm install eslint --save-dev
```

**Note**: You may install ESLint globally using the `-g` flag.

Next, install `eslint-plugin-bem-xjst`:

```
$ npm install eslint-plugin-bem-xjst --save-dev
```

**Note**: If you installed ESLint globally (using the `-g` flag) then you must also install `eslint-plugin-bem-xjst` globally.

A globally-installed instance of ESLint can only use globally-installed ESLint plugins. A locally-installed ESLint can make use of both locally- and globally- installed ESLint plugins.

Usage
-----

Add `bem-xjst` to the plugins section of your `.eslintrc` configuration file.

```json
{
    "plugins": [
        "bem-xjst"
    ]
}
```

**Note**: We omitted the `eslint-plugin-` prefix since it is automatically assumed by ESLint.

For BEMHTML templates add the `bem-xjst/bemhtml` environment to `.eslintrc`:

```json
{
    "env": {
        "bem-xjst/bemhtml": true
    }
}
```

For BEMTREE templates add the `bem-xjst/bemtree` environment to `.eslintrc`:

```json
{
    "env": {
        "bem-xjst/bemtree": true
    }
}
```

License
-------

MIT © [Andrew Abramov](https://github.com/blond)
