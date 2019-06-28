# Get bulb brightness level

Returns current brightness level of bulb

```sig
samsungiot.getBulbLevel("Sengled bulb");
```

## Parameters

* `name` is a [String](/types/string). Bulb device name.

## Examples:

To get brightness level of bulb, named "Sengled bulb":

```blocks
let level = samsungiot.getBulbLevel("Sengled bulb")
basic.showNumber(level)
```
