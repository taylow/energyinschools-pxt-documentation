# Get switch state

Returns current state of switch 

```sig
samsungiot.getSwitchState("Room switch");
```

## Parameters

* `name` is a [String](/types/string). Switch device name.

## Examples:

To check state of switch, named "Room switch":

```blocks
let state = samsungiot.getSwitchState("Room switch")
if (state) {
    basic.showString("Switch is on!")
} else {
    basic.showString("Switch is off!")
}
```
