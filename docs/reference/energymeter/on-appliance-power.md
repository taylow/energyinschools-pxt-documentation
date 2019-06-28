# On Appliance Power

Start an [event handler](/makecode-blockeditor/reference/event-handler) (part of the program that will run when something happens, like when the appliance power turns on). 
This handler works when the appliance that the @boardname@ is connected to changes from on to off, or off to on.

To use the @boardname@ to check the appliance power you must first calibrate the position of the @boardname@ on the cable. After connecting a @boardname@ to an appliance power cable you can run the calibration block to correctly position the @boardname@.

```sig
energymeter.onPowerHandler(ApplianceState.on, () => {})
```

## How does it work?
This works by using the @boardname@'s compas (magnetometer) to sense the changes in the magnetic field produced by current flowing through a cable. When an appliance is turned on, the magnetic force is strong and will trigger the `on` event. When an appliance is turned off, the magnetic force wont be being produced by the cable and will trigger the `off` event.

Learn about the magnetic field of a wire in this video:

https://www.youtube.com/watch?v=nfSJ62mzKyY

## Example

This program uses `on appliance power` and `show icon` to display a tick or a cross when the appliance is turned on or off.

```blocks
energymeter.onPowerHandler(ApplianceState.on, () => {
    basic.showIcon(IconNames.Yes)
})
energymeter.onPowerHandler(ApplianceState.off, () => {
    basic.showIcon(IconNames.No)
})
```

Note: The @boardname@ needs to be calibrated correctly for the readings to be accurate.

## See also

[calibrate energy meter](/makecode-blockeditor/reference/energymeter/calibrate), [event handler](/makecode-blockeditor/reference/event-handler)
