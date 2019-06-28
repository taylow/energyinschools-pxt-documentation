# Share data

Send data collected by microbit into cloud storage. Data can be private, or shared with other schools
```sig
share.shareData("15", "temperature in room", ShareLevel.all);
```

## Parameters

* `data` is a [String](/types/string). Data, that would be send to storage 
* `name` is a [String](/types/string). Data identifier 
* `level` is a choice value. Can be own school or all

## Examples:

To share data from sensor with own school only:

```blocks
let temperature = samsungiot.getSensorTemp("Motion sensor")
let temperatureText = share.numberToText(temperature);
share.shareData(temperatureText, "motion sensor temperature", ShareLevel.school);
```
