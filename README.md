# async-collection [![stability][0]][1]
[![npm version][2]][3] [![build status][4]][5]
[![downloads][8]][9] [![js-standard-style][10]][11]

Collection of async functions

## Usage
```js
// require the whole module
var async = require('async-collection')

// require an invidiual method
var parallel = require('async-collection/parallel')
```

## API
### `async.waterfall(arr, cb)`
Run an array of functions in series, each passing its results to the next
function. Uses [run-waterfall](https://github.com/feross/run-waterfall).

### `async.series(arr, cb)`
Run an array of functions in series. Uses
[run-series](https://github.com/feross/run-series).

### `async.parallel(arr, cb)`
Run an array of functions in parallel. Uses
[run-parallel](https://github.com/feross/run-parallel).

### `async.parallelLimit(arr, cb)`
Run an array of functions in parallel, but limit the number of tasks executing
at the same time. Uses
[parallel-limit](https://github.com/feross/run-parallel-limit).

### `async.mapLimit(arr, limit, iterator, cb)`
Map over an array of data and call them, but limit the number of tasks
executing at the same time. Uses
[map-limit](https://github.com/hughsk/map-limit).

## License
[MIT](https://tldrlegal.com/license/mit-license)

[0]: https://img.shields.io/badge/stability-experimental-orange.svg?style=flat-square
[1]: https://nodejs.org/api/documentation.html#documentation_stability_index
[2]: https://img.shields.io/npm/v/async-collection.svg?style=flat-square
[3]: https://npmjs.org/package/async-collection
[4]: https://img.shields.io/travis/yoshuawuyts/async-collection/master.svg?style=flat-square
[5]: https://travis-ci.org/yoshuawuyts/async-collection
[6]: https://img.shields.io/codecov/c/github/yoshuawuyts/async-collection/master.svg?style=flat-square
[7]: https://codecov.io/github/yoshuawuyts/async-collection
[8]: http://img.shields.io/npm/dm/async-collection.svg?style=flat-square
[9]: https://npmjs.org/package/async-collection
[10]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square
[11]: https://github.com/feross/standard
