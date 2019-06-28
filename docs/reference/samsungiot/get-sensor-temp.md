# Get sensor temperature level

Returns current temperature level of sensor

```sig
samsungiot.getSensorTemp("Motion sensor");
```

## Parameters

* `name` is a [String](/types/string). Sensor device name.

## Examples:

To get temperature level of sensor, named "Motion sensor":

```blocks
let temperature = samsungiot.getSensorTemp("Motion sensor")
basic.showNumber(temperature)
```
