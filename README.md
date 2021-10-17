# Pocket Style Guide

Pocket's style guide package: eslint, prettier & commitlint.

## Usage

1. Add `@grande-armee/pocket-style-guide` to *devDependencies* in *package.json*

```json
{
  "devDependencies": {
    "@grande-armee/pocket-style-guide": "^1.0.0"
  }
}
```

2. Install peer dependencies

```bash
npm i -D eslint prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-prettier eslint-plugin-import eslint-plugin-prettier @commitlint/cli @commitlint/config-conventional
```

1. Import config files

`.eslintrc.js`:

```js
module.exports = {
  ...require('@grande-armee/pocket-style-guide/eslint'),
};
```

`.prettierrc.js`:

```js
module.exports = {
  ...require('@grande-armee/pocket-style-guide/prettier'),
};
```

`commitlint.config.js`:

```js
module.exports = {
  ...require('@grande-armee/pocket-style-guide/commitlint'),
};
```
