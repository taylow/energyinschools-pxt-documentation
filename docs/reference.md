# Reference

## @description List of API categories available in the editors

```namespaces
basic.showNumber(0);
input.onButtonPressed(Button.A, () => {
    
});
music.playTone(0, 0);
led.plot(0, 0);
radio.sendNumber(0);
carbon.setCarbonIndexValueType(CarbonIndex.moderate);
energy.querySchoolEnergy(EnergyType.electricity);
samsungiot.setTempColour(BulbTemp.level_5)
share.shareHistoricalData("15", "temperature near window", "class 5-B", "celsius")
weather.getWeatherForecastTomorrow(WeatherLocationType.city, "London")
energymeter.sendEnergyMeterReading(ApplianceType.printer, "printer")
```
## Advanced

```namespaces
game.addScore(1);
images.createImage(`
. . . . .
. . . . .
. . # . .
. . . . .
. . . . .
`);
pins.digitalReadPin(DigitalPin.P0);
serial.writeNumber(0);
control.inBackground(() => {
    
});
```

## Bluetooth

```namespaces
bluetooth.onBluetoothConnected(() => {});
devices.tellCameraTo(MesCameraEvent.TakePhoto);
```
  
```package
radio
devices
bluetooth
```

## See Also

[basic](/makecode-blockeditor/reference/basic), [input](/makecode-blockeditor/reference/input), [music](/makecode-blockeditor/reference/music), [led](/makecode-blockeditor/reference/led), [Math (blocks)](/blocks/math), [String](/types/string), [game](/makecode-blockeditor/reference/game), [images](/makecode-blockeditor/reference/images), [pins](/makecode-blockeditor/reference/pins), [serial](/makecode-blockeditor/reference/serial), [control](/makecode-blockeditor/reference/control), [radio](/makecode-blockeditor/reference/radio), [devices](/makecode-blockeditor/reference/devices), [bluetooth](/makecode-blockeditor/reference/bluetooth)
