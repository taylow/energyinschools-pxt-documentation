# Set colour temperature value

Returns temperature colour value

```sig
samsungiot.setTempColour(BulbTemp.level_5);
```

## Parameters

* `colourTemp` is choice value. It can any available colour temperature.

## Examples:

To return soft colour temperature:

```blocks
let temperature = samsungiot.setTempColour(BulbTemp.soft_1)
basic.showNumber(temperature)
```
