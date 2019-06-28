# Devices

Control a phone with the @boardname@ via Bluetooth.

## ~ hint

**App required** You must use one of the [micro:bit apps](https://microbit.org/guide/mobile/) to use this functionality.

## ~

```cards
devices.tellCameraTo(MesCameraEvent.TakePhoto);
devices.tellRemoteControlTo(MesRemoteControlEvent.play);
devices.raiseAlertTo(MesAlertEvent.DisplayToast);
devices.onNotified(MesDeviceInfo.IncomingCall, () => {
    
});
devices.onGamepadButton(MesDpadButtonInfo.ADown, () => {
    
});
devices.signalStrength();
devices.onSignalStrengthChanged(() => {
    
});
```

```package
devices
```

## See Also

[tellCameraTo](/makecode-blockeditor/reference/devices/tell-camera-to), [tellRemoteControlTo](/makecode-blockeditor/reference/devices/tell-remote-control-to), [raiseAlertTo](/makecode-blockeditor/reference/devices/raise-alert-to), [onNotified](/makecode-blockeditor/reference/devices/on-notified), [onGamepadButton](/makecode-blockeditor/reference/devices/on-gamepad-button), [signalStrength](/makecode-blockeditor/reference/devices/signal-strength), [onSignalStrengthChanged](/makecode-blockeditor/reference/devices/on-signal-strength-changed)
