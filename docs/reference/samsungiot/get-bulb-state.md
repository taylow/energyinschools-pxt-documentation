# Get bulb state

Returns current state of bulb 

```sig
samsungiot.getBulbState("Sengled bulb");
```

## Parameters

* `name` is a [String](/types/string). Bulb device name.

## Examples:

To check state of bulb, named "Sengled bulb":

```blocks
let state = samsungiot.getBulbState("Sengled bulb")
if (state) {
    basic.showString("Bulb is on!")
} else {
    basic.showString("Bulb is off!")
}
```
