mochify-istanbul
=====================

Add istanbul coverage to the [mochify.js](https://github.com/mantoni/mochify.js) pipeline.
**NOTE:** This will work with >= mochify.js@2.0.0, in the mean time it depends on a fork that already returns the browserify bundle

## Install

```
$ npm install mochify mochify-istanbul
```

## Usage

```javascript
va b = mochify('path/to/your/file', mochifyOpts)
  .plugin(istanbul({
    reporter: { reports: ['text', 'cobertura', 'json'] }
  }))
  .bundle();
```

## Compatibility
 - Node >= 0.10
 - v0.x
    - Mochify 2.x
        - Browserify 6.x
        - Mocha 2.x


## Run tests
Clone the repo and run ```npm install && npm test```
