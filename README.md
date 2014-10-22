loop-grid-suppressor
===

Transform for suppressing selected loops on [loop-grid](https://github.com/mmckegg/loop-grid).

## API

```js
var Suppressor = require('loop-grid-suppressor')
```

### `var suppressor = Suppressor(transform, shape[, stride])`

Pass `loopGrid.transform` to this constructor.

Returns an extended [observ](https://github.com/raynos/observ) instance containing instances of [array-grid](https://github.com/mmckegg/array-grid) with `true` values at coords where currently suppressed.

### `suppressor.start(indexes, done)`

Calls `transform` with a function that suppresses all `indexes` specified.

### `suppressor.stop()`

Release suppression `transform`.