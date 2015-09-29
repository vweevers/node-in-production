# in-production

**Two simple variants of NODE_ENV === production. Exports a boolean or a function, which turns into a noop when browserified. Best combined with [uglifyify](https://github.com/hughsk/uglifyify) as a transform to remove dead code.**

[![npm status](http://img.shields.io/npm/v/in-production.svg?style=flat-square)](https://www.npmjs.org/package/in-production) 

## example

As a boolean, using a cached `process.env.NODE_ENV`

```js
var inProduction = require('in-production')

if (inProduction) //..
```

As a function, using an uncached `process.env.NODE_ENV`

```js
var inProduction = require('in-production/function')

if (inProduction()) // ..
```

## install

With [npm](https://npmjs.org) do:

```
npm install in-production
```

## license

[MIT](http://opensource.org/licenses/MIT) © [Vincent Weevers](http://vincentweevers.nl/)
