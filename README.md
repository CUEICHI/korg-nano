# Korg Nano #

A simple module for getting data events from a Korg Nano Kontrol.

## Example ##

```js

var Korg = require('korg-nano')

korg = new Korg()

korg.on('*', function(event, value) {
  console.log(event)
  // event will be something like one of the following
  // "knob:1", "slider:9", "button:16", "button:prev"
  console.log(value)
  // value will be a number between 0 and 1
  // buttons will either be 0 or 1
})

```

## License ##

MIT
