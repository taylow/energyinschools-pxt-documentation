# write Value To Serial

Write the data received by radio to serial in JSON format.

```sig
radio.writeValueToSerial();
```

## ~ hint

**Deprecated**

This API has been deprecated! Use [write received packet to serial](/makecode-blockeditor/reference/radio/write-received-packet-to-serial) instead.

## ~

## Data received format

The format for received data printed to serial is as follows:

- [send number](/makecode-blockeditor/reference/radio/send-number): ```{v:ValueSent,t:MicrobitTimeAlive,s:SerialNumber}```
- [send value](/makecode-blockeditor/reference/radio/send-value): ```{v:ValueSent,t:MicrobitTimeAlive,s:SerialNumber,n:"Name"}```
- [send string](/makecode-blockeditor/reference/radio/send-string): ```{t:MicrobitTimeAlive,s:SerialNumber,n:"Text"}```

## Examples

When ```radio``` data is received (after pressing the ``A`` button on
the second @boardname@), this program sends temperature data to
serial.

```blocks
input.onButtonPressed(Button.A, () => {
    radio.sendNumber(input.temperature());
});
radio.onDataReceived(() => {
    radio.writeValueToSerial();
});
```
Sample output to serial when ``A`` button pressed:

```Text
{v:27,t:323,s:0}
```

## See also

[send number](/makecode-blockeditor/reference/radio/send-number),
[send value](/makecode-blockeditor/reference/radio/send-value),
[send string](/makecode-blockeditor/reference/radio/send-string),
[on data packet received](/makecode-blockeditor/reference/radio/on-data-packet-received)

```package
radio
```