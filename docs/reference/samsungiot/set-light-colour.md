# Set colour value

Returns light colour value

```sig
samsungiot.setLightColour(BulbColour.blue);
```

## Parameters

* `lightColour` is choice value. It can any available light colour.

## Examples:

To return blue light colour:

```blocks
let colour = samsungiot.setLightColour(BulbColour.blue)
basic.showNumber(colour)
```
