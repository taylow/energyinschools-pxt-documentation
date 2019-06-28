# Bluetooth

Support for additional Bluetooth services.

## ~hint
![](/static/bluetooth/Bluetooth_SIG.png)

For another device like a smartphone to use any of the Bluetooth "services" which the @boardname@ has, it must first be [paired with the @boardname@](/makecode-blockeditor/reference/bluetooth/bluetooth-pairing). Once paired, the other device may connect to the @boardname@ and exchange data relating to many of the @boardname@'s features.

## ~


```cards
bluetooth.startAccelerometerService();
bluetooth.startButtonService();
bluetooth.startIOPinService();
bluetooth.startLEDService();
bluetooth.startMagnetometerService();
bluetooth.startTemperatureService();
bluetooth.onBluetoothConnected(() => {});
bluetooth.onBluetoothDisconnected(() => {});
bluetooth.setTransmitPower(7);
```

## UART 

```cards
bluetooth.startUartService();
bluetooth.uartReadUntil("");
bluetooth.uartWriteLine("");
bluetooth.uartWriteString("");
bluetooth.uartWriteNumber(0);
bluetooth.uartWriteValue("", 0);
bluetooth.onUartDataReceived(",", () => {})
```

## Eddystone

```cards
bluetooth.advertiseUid(42, 1, 7, true);
bluetooth.advertiseUrl("https://makecode.microbit.org/", 7, true);
bluetooth.stopAdvertising();
```

## Advanced
 
For more advanced information on the @boardname@ Bluetooth UART service including information on using a smartphone, see the [Lancaster University @boardname@ runtime technical documentation](http://lancaster-university.github.io/microbit-docs/ble/uart-service/)

## See Also

[startAccelerometerService](/makecode-blockeditor/reference/bluetooth/start-accelerometer-service), [startButtonService](/makecode-blockeditor/reference/bluetooth/start-button-service), [startIOPinService](/makecode-blockeditor/reference/bluetooth/start-io-pin-service), [startLEDService](/makecode-blockeditor/reference/bluetooth/start-led-service), [startMagnetometerService](/makecode-blockeditor/reference/bluetooth/start-magnetometer-service), [startTemperatureService](/makecode-blockeditor/reference/bluetooth/start-temperature-service), 
[startUartService](/makecode-blockeditor/reference/bluetooth/start-uart-service),
[uartReadUntil](/makecode-blockeditor/reference/bluetooth/uart-read-until), 
[uartWriteLine](/makecode-blockeditor/reference/bluetooth/uart-write-line), 
[uartWriteString](/makecode-blockeditor/reference/bluetooth/uart-write-string), 
[uartWriteNumber](/makecode-blockeditor/reference/bluetooth/uart-write-number), 
[uartWriteValue](/makecode-blockeditor/reference/bluetooth/uart-write-value), 
[onBluetoothConnected](/makecode-blockeditor/reference/bluetooth/on-bluetooth-connected), 
[onBluetoothDisconnected](/makecode-blockeditor/reference/bluetooth/on-bluetooth-disconnected),
[advertiseUrl](/makecode-blockeditor/reference/bluetooth/advertise-url),
[stopAdvertising](/makecode-blockeditor/reference/bluetooth/stop-advertising)

```package
bluetooth
```
