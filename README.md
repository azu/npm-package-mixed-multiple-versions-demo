# npm-package-mixed-multiple-versions-demo

Demo project for mixing multiple version of the same npm package in a project.

## Installation

    npm install
    
## Usage


1. Create local package `lodash3` and `lodash4`
    - These wrap of `lodash@3` and `lodash@4`
2. Install as local dependencies(`file:`)
    - `npm i -S packages/lodash3 packages/lodash4`
3. Use it!

```js
"use strict";
var assert = require("assert");
var lodash3 = require("lodash3");
var lodash4 = require("lodash4");

assert(lodash3.VERSION.includes("3"));
assert(lodash4.VERSION.includes("4"));
```

## Real UseCase

- [Add support for ESLint v2 by Daniel15 · Pull Request #107 · fkling/astexplorer](https://github.com/fkling/astexplorer/pull/107/files#diff-b9cfc7f2cdf78a7f4b91a753d10865a2R52 "Add support for ESLint v2 by Daniel15 · Pull Request #107 · fkling/astexplorer")

## Tests

    npm test

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

MIT