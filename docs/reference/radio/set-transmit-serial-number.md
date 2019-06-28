# set Transmit Serial Number

Make the radio packet embed the board serial number with each packet of data.

```sig
radio.setTransmitSerialNumber(true);
```

## Parameters

* **transmit**: a [boolean](/types/boolean) that, when ``true``, means that the board serial number is included in each transmitted packet. If ``false``, the serial number value is set to `0`.

## Example

This program makes the ``radio`` send the serial number in each packet.

```blocks
radio.setTransmitSerialNumber(true);
```

## See also

[received packet property](/makecode-blockeditor/reference/radio/received-packet),
[send number](/makecode-blockeditor/reference/radio/send-number),
[send value](/makecode-blockeditor/reference/radio/send-value),
[send string](/makecode-blockeditor/reference/radio/send-string)

```package
radio
```