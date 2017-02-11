# babel-plugin-transform-flow-strip-types

> Strip all [flow](http://flowtype.org) type annotations and declarations from your output code.

## Example

**In**

```javascript
function foo(one: any, two: number, three?): string {}
```

**Out**

```javascript
function foo(one, two, three) {}
```

## Installation

```sh
npm install --save-dev babel-plugin-transform-flow-strip-types
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["transform-flow-strip-types"]
}
```

### Via CLI

```sh
babel --plugins transform-flow-strip-types script.js
```

### Via Node API

```javascript
require("@babel/core").transform("code", {
  plugins: ["transform-flow-strip-types"]
});
```
