# Set bulb state

Change current state of bulb 

```sig
samsungiot.setBulbState("Sengled bulb", SwitchState.on);
```

## Parameters

* `name` is a [String](/types/string). Bulb device name.
* `state` is a choice value. Target state value (on/off).

## Examples:

To set state of bulb, named "Sengled bulb", to "On":

```blocks
samsungiot.setBulbState("Sengled bulb", SwitchState.on)
```
