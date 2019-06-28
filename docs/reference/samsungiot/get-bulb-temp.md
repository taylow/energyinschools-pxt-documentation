# Get bulb colour temperature level

Returns current colour temperature level of bulb

```sig
samsungiot.getBulbTemp("Sengled bulb");
```

## Parameters

* `name` is a [String](/types/string). Bulb device name.

## Examples:

To get temperature level of bulb, named "Sengled bulb":

```blocks
let temperature = samsungiot.getBulbTemp("Sengled bulb")
basic.showNumber(temperature)
```
