# Get bulb colour value

Returns current colour of bulb

```sig
samsungiot.getBulbColour("Sengled bulb");
```

## Parameters

* `name` is a [String](/types/string). Bulb device name.

## Examples:

To get current colour of bulb, named "Sengled bulb":

```blocks
let colour = samsungiot.getBulbColour("Sengled bulb")
basic.showNumber(colour)
```
