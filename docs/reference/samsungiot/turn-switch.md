# Turn switch state to on/off

Change current state of switch 

```sig
samsungiot.turnSwitch("Room switch", SwitchState.on);
```

## Parameters

* `name` is a [String](/types/string). Switch device name.
* `state` is a choice value. Target state value (on/off).

## Examples:

To change state of switch, named "Room switch", to "Off":

```blocks
samsungiot.turnSwitch("Room switch", SwitchState.off)
```
