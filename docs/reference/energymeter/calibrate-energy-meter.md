# Calibrate Energy Meter

To use the @boardname@ as an energy meter you must first calibrate the position of the @boardname@ on the cable. After connecting a @boardname@ to an appliance power cable you can run the calibration block to correctly position the @boardname@.

```sig
energymeter.calibrateEnergyMeter()
```

## How does it work?
This works by using the @boardname@'s compas (magnetometer) to sense the changes in the magnetic field produced by current flowing through a cable. This field has stronger and weaker points which are recorded as the high and low values. 
Start by slowly turning the @boardname@ around the cable at least once.
Once the @boardname@ has had a chance to sense around the cable, it will know where the strong points are and will show you how strong the magnetic force is by drawing a line on the display. If the line is high, the strength is high.
After you begin to see a line moving around, try to position the @boardname@ so that the line is as high as you can get it (the higher the better!). Once you are happy with the calibration, press in button `A` and button `B` together to complete the calibration.

Learn about the magnetic field of a wire in this video:

https://www.youtube.com/watch?v=nfSJ62mzKyY

## Example

This program uses `on button bressed` and `calibrate energy meter` to start the calibration process needed to position the @boardname@ on the appliance power cable correctly.

```blocks
input.onButtonPressed(Button.A, () => {
    energymeter.calibrateEnergyMeter()
})
```

Note: The @boardname@ needs to be calibrated correctly for the readings to be accurate.

## See also

[on button pressed](/makecode-blockeditor/reference/input/on-button-pressed)
