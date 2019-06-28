# Send Power Level

After connecting a @boardname@ to an appliance power cable and calibrating, the @boardname@ can sense and report how much power in Watts the appliance is using right now.
This data will be sent directly to the Energy in Schools portal along with the appliance type and a name.

```sig
energymeter.sendEnergyMeterReading(ApplianceType.other, "")
```

## How does it work?
This works by using the @boardname@'s compas (magnetometer) to sense the changes in the magnetic field produced by current flowing through a cable. With some fancy maths, the strength of this magnetic field can be converted to Watts.

Learn about the magnetic field of a wire in this video:

https://www.youtube.com/watch?v=nfSJ62mzKyY

## Example

This program uses `on button A` and `send power level (watts)` to report the power consumption of an appliance to the Energy in Schools portal.

```blocks
input.onButtonPressed(Button.A, () => {
    energymeter.sendEnergyMeterReading(ApplianceType.other, "")
})
```

Note: The @boardname@ needs to be calibrated correctly for the readings to be accurate.

## See also

[on button pressed](/makecode-blockeditor/reference/input/on-button-pressed), [forever](/makecode-blockeditor/reference/basic/forever)
