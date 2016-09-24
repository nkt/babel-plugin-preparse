# babel-plugin-preparse

Optimize code for faster initial execution and parsing, by wrapping all immediately-invoked functions or likely-to-be-invoked functions in parentheses.

[Original project](https://github.com/nolanlawson/optimize-js).

## Installation

```sh
$ npm install babel-plugin-preparse
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["preparse"]
}
```

### Via CLI

```sh
$ babel --plugins preparse script.js
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  plugins: ["preparse"]
});
```
