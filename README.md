# eslint-config-simple

<a name="overview"></a>

### Overview

A simple, shareable ESLint configuration meant to be used with [prettier](https://github.com/prettier/prettier). Look at the [config](/configs/eslint.config.js) file as it is pretty small.

<a name="install"></a>

### Install

First install `eslint-config-simple`:

```shell
$ yarn install eslint-config-simple --dev
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
