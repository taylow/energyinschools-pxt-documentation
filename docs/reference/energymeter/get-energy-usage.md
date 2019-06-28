# Get Energy Consumption

After connecting a @boardname@ to an appliance power cable and calibrating, the @boardname@ can sense and report how much power in Watts the appliance is using right now.

```sig
energymeter.getEnergyUsage()
```

## Returns
* a [number](/types/number) that is the power draw of the appliance in Watts.

## How does it work?
This works by using the @boardname@'s compas (magnetometer) to sense the changes in the magnetic field produced by current flowing through a cable. With some fancy maths, the strength of this magnetic field can be converted to Watts.

Learn about the magnetic field of a wire in this video:

https://www.youtube.com/watch?v=nfSJ62mzKyY

## Example

This program uses `get energy consumption` and `show number` to show the power consumption of an appliance. 

```blocks
basic.forever(() => {
    basic.showNumber(energymeter.getEnergyUsage())
})
```

Note: The @boardname@ needs to be calibrated correctly for the readings to be accurate.

## See also

[on appliance power](/makecode-blockeditor/reference/energymeter/on-appliance-power), [calibrate energy meter](/makecode-blockeditor/reference/energymeter/calibrate), [forever](/makecode-blockeditor/reference/basic/forever)
