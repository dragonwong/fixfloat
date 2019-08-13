# fixfloat

[![npm](https://img.shields.io/npm/v/fixfloat.svg?maxAge=60)](https://www.npmjs.com/package/fixfloat)
[![npm](https://img.shields.io/npm/dt/fixfloat.svg?maxAge=60)](https://www.npmjs.com/package/fixfloat)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/dragonwong/fixfloat/master/LICENSE)

You can use it to fix the float-number bug in javascript.

```js
const fixfloat = require('fixfloat');

const floatNumber = 0.1 + 0.2; // 0.30000000000000004

fixfloat(floatNumber); // 0.3
```

You can also use it to round your number.

```js
const fixfloat = require('fixfloat');

const floatNumber = 3456.3456;

fixfloat(floatNumber); // 3456.3
fixfloat(floatNumber, 2); // 3456.35
fixfloat(floatNumber, 1); // 3456.3
fixfloat(floatNumber, 0); // 3456
fixfloat(floatNumber, -1); // 3460
fixfloat(floatNumber, -3); // 3000
```

## Install

```bash
npm install fixfloat --save
```
