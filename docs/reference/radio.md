# Radio

Send and receive data using radio packets.

```cards
radio.sendNumber(0);
radio.sendValue("name", 0);
radio.sendString("");
radio.onReceivedNumber(function (receivedNumber) { });
radio.onReceivedValue(function (name, value) { });
radio.onReceivedString(function (receivedString) { });
radio.receivedPacket(RadioPacketProperty.SignalStrength)
radio.setGroup(0);
```

## Advanced

```cards
radio.writeReceivedPacketToSerial();
radio.setTransmitPower(7);
radio.setTransmitSerialNumber(false);
radio.raiseEvent(0, 0);
```

```package
radio
```

## See Also

[send number](/makecode-blockeditor/reference/radio/send-number),
[send value](/makecode-blockeditor/reference/radio/send-value),
[send string](/makecode-blockeditor/reference/radio/send-string),
[on received number](/makecode-blockeditor/reference/radio/on-received-number),
[on received value](/makecode-blockeditor/reference/radio/on-received-value),
[on received string](/makecode-blockeditor/reference/radio/on-received-string),
[received packet](/makecode-blockeditor/reference/radio/received-packet),
[set group](/makecode-blockeditor/reference/radio/set-group),
[set transmit power](/makecode-blockeditor/reference/radio/set-transmit-power),
[set transmit serial number](/makecode-blockeditor/reference/radio/set-transmit-serial-number),
[write received packet to serial](/makecode-blockeditor/reference/radio/write-received-packet-to-serial),
[raise event](/makecode-blockeditor/reference/radio/raise-event)
