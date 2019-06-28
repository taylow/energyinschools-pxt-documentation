# Get sensor state

Returns current state of sensor 

```sig
samsungiot.getSensorState("Motion sensor");
```

## Parameters

* `name` is a [String](/types/string). Sensor device name.

## Examples:

To check state of sensor, named "Motion sensor":

```blocks
let state = samsungiot.getSensorState("Motion sensor")
if (state) {
    basic.showString("Motion detected!")
} else {
    basic.showString("No motion!")
}
```
