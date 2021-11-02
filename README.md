# Weird `meta http-equiv="refresh"` behavior with `window.close()`

* `index.html` has a `meta http-equiv="refresh"` with a `url` attribute.
* `closeme/index.html` has a `window.close()`

By messing with the `content="0;` we can see different behaviors.

## Getting started

1. `npm install`
2. `npm start`

## Scenarios

### `content` set to `0;`

In Edge, `window.close()` will work.

In Safari, `window.close()` will not work and throw `Can't close the window since it was not opened by JavaScript`.

### `content` set to `5;`

In Edge & Safari, `window.close()` will not work and throw `Can't close the window since it was not opened by JavaScript`.
