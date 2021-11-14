# Pocket Style Guide

Pocket's style guide package: eslint, prettier & commitlint.

## Usage

1. Add `@grande-armee/pocket-style-guide` to *devDependencies* in *package.json*

```bash
npm install --save-dev @grande-armee/pocket-style-guide
```

```json
{
  "devDependencies": {
    "@grande-armee/pocket-style-guide": "^2.0.0"
  }
}
```

2. Install peer dependencies

```bash
npm install --save-dev eslint prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-prettier eslint-import-resolver-typescript eslint-plugin-import eslint-plugin-unicorn eslint-plugin-jest eslint-plugin-prettier @commitlint/cli @commitlint/config-conventional
```

3. Import config files

`.eslintrc.js`:

```js
const { createConfig } = require('@grande-armee/pocket-style-guide/eslint');

module.exports = createConfig([]);
```

`.prettierrc.js`:

```js
const { createConfig } = require('@grande-armee/pocket-style-guide/prettier');

module.exports = createConfig();
```

`commitlint.config.js`:

```js
const { createConfig } = require('@grande-armee/pocket-style-guide/commitlint');

module.exports = createConfig();
```
