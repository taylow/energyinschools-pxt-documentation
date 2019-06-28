# Electrical Power Status

After connecting a @boardname@ to an appliance power cable and calibrating, the @boardname@ can tell you if that device is currently turned on or off right now.

```sig
energymeter.getElectricalPowerStatus();
```

## Returns
* a [boolean](/blocks/logic/boolean) value that is `true` if the electrical device the @boardname@ is attached to if on, `false` if it is off.

## Example

This program uses an [``||logic:if||``](/blocks/logic/if) to run 
one part of the program if the applicance if on, and 
another part if it is off.

```blocks
basic.forever(() => {
    let on = energymeter.getElectricalPowerStatus()
    if (on) {
        // this part runs if the appliance is on
        basic.showNumber(1)
    } else {
        // this part runs if the appliance is off
        basic.showNumber(0)
    }
})
```

Note: The @boardname@ needs to be calibrated correctly for the readings to be accurate.

## See also

[on appliance power](/makecode-blockeditor/reference/energymeter/on-appliance-power), [calibrate energy meter](/makecode-blockeditor/reference/energymeter/calibrate), [if](/blocks/logic/if), [forever](/makecode-blockeditor/reference/basic/forever)
