# eslint-config-simple

<a name="overview"></a>

### Overview

A simple, shareable ESLint configuration meant to be used with [prettier](https://github.com/prettier/prettier). View the [config](/configs/eslint.config.js) file, (it is pretty small), to see how ESLint is made to work with prettier.

<a name="install"></a>

### Install

```shell
# npm
npm install eslint-config-simple --save-dev

# yarn
yarn add eslint-config-simple --dev
```

Then add to the `extends` array in your eslint config file:

```json5
{
  extends: ["simple"]
}
```

### Overriding

Since it exports an object it can also be used in the following manner:

```js
// eslint.config.js

"use strict";

// Import simple eslint config.
const config = require("eslint-config-simple");

// Override/add anything to config object:

// Add settings key, for example.
config.settings = {
  react: {
    version: "16.6.3"
  }
};

// Export config.
module.exports = config;
```

<a name="license"></a>

### License

This project uses the [MIT License](/LICENSE.txt).
