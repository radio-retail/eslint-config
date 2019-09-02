# @radio-retail/eslint-config

[![make a pull request](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![radio-retail-code-style](https://img.shields.io/badge/style-radio%20retail-379CC1.svg?style=flat-square)](https://github.com/radio-retail/eslint-config)

> ESLint config for [Radio Retail](http://www.zapop.com/service/radioretail/)

## Table of Contents

- [About](#about)
- [Usage](#usage)
- [Configuration](#configuration)
- [Other](#other)
- [Contribute](#contribute)
- [License](#license)

## About

Shareable configs are designed to work with the `extends` feature of `eslint` files.
You can learn more about
[shareable configs](http://eslint.org/docs/developer-guide/shareable-configs) on the
official ESLint website.

## Usage

This package has several peer dependencies. Run `npm info "@radio-retail/eslint-config@latest" peerDependencies` to list them all.

Install all the dependencies:

```bash
npm install --save-dev @radio-retail/eslint-config eslint babel-eslint prettier eslint-config-prettier eslint-plugin-promise eslint-plugin-import

# or

yarn add --dev @radio-retail/eslint-config eslint babel-eslint prettier eslint-config-prettier eslint-plugin-promise eslint-plugin-import
```


Then, add this to your `.eslintrc` file:

```json
{
  "extends": "@radio-retail",
  "env": {
    "browser": true,
  }
}
```

_Note: The `eslint-config-` prefix  has been omitted since it is automatically assumed by ESLint._

You can override settings from the shareable config by adding them directly into your
`.eslintrc` file.

### Using with prettier

Follow instructions for [prettier-eslint-cli](https://github.com/prettier/prettier-eslint-cli) installation and add script:

```
"format": "prettier-eslint --write --eslint-ignore"
```

### Add a badge [![radio-retail-code-style](https://img.shields.io/badge/style-radio%20retail-379CC1.svg?style=flat-square)](https://github.com/radio-retail/eslint-config)

```
[![radio-retail-code-style](https://img.shields.io/badge/style-radio%20retail-379CC1.svg?style=flat-square)](https://github.com/radio-retail/eslint-config)
```

## Configurations

## React

Includes the [default configuration](./index.js) as well as [React](https://reactjs.org/) specific environment specification and rules via:

- [`eslint-plugin-react`](https://github.com/yannickcr/eslint-plugin-react)
- [`eslint-plugin-react-hooks`](https://github.com/facebook/react/tree/master/packages/eslint-plugin-react-hooks)
- [`eslint-plugin-jsx-a11y`](https://github.com/evcohen/eslint-plugin-jsx-a11y)

Setup:

```bash
$ npm install --save-dev @radio-retail/eslint-config eslint babel-eslint prettier eslint-config-prettier eslint-plugin-promise eslint-plugin-import eslint-plugin-react eslint-plugin-jsx-a11y eslint-plugin-react-hooks

# or

yarn add --dev @radio-retail/eslint-config eslint babel-eslint prettier eslint-config-prettier eslint-plugin-promise eslint-plugin-import eslint-plugin-react eslint-plugin-jsx-a11y eslint-plugin-react-hooks

```

In your `.eslintrc`:

```json
{
  "extends": "@radio-retail/eslint-config/react"
}
```

## Contribute

1. Fork it and create your feature branch: `git checkout -b my-new-feature`
2. Commit your changes: `git commit -am 'Add some feature'`
3. Push to the branch: `git push origin my-new-feature`
4. Submit a pull request

## License

MIT

