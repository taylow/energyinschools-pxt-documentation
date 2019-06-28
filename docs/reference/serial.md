# Serial

Read and write data over a serial connection.

```cards
serial.writeLine("");
serial.writeNumber(0);
serial.writeValue("x", 0);
serial.writeString("");
serial.writeNumbers([0]);
serial.readUntil(",");
serial.readLine();
serial.readString();
serial.onDataReceived(",", () => {})
```

## Advanced

```cards
serial.redirect(SerialPin.P0, SerialPin.P0, BaudRate.BaudRate115200);
serial.redirectToUSB();
serial.writeBuffer(pins.createBuffer(0));
serial.readBuffer(64);
```

## See Also

[writeLine](/makecode-blockeditor/reference/serial/write-line), [writeNumber](/makecode-blockeditor/reference/serial/write-number), [writeValue](/makecode-blockeditor/reference/serial/write-value),
[writeString](/makecode-blockeditor/reference/serial/write-string), 
[writeNumbers](/makecode-blockeditor/reference/serial/write-numbers), [readUntil](/makecode-blockeditor/reference/serial/read-until), [readLine](/makecode-blockeditor/reference/serial/read-line),
[readString](/makecode-blockeditor/reference/serial/read-string), [onDataReceived](/makecode-blockeditor/reference/serial/on-data-received),
[redirect](/makecode-blockeditor/reference/serial/redirect), [writeBuffer](/makecode-blockeditor/reference/serial/write-buffer), [readBuffer](/makecode-blockeditor/reference/serial/read-buffer),
[redirectToUSB](/makecode-blockeditor/reference/serial/redirect-to-usb)
