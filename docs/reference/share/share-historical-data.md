# Share historical data

Send historical data collected by microbit into cloud storage. Together with name and namespace it will form historical dataset
```sig
share.shareHistoricalData("15", "temperature near window", "class 5-B", "celsius");
```

## Parameters

* `data` is a [String](/types/string). Data, that would be send to storage 
* `name` is a [String](/types/string). Dataset name 
* `space` is a [String](/types/string). Dataset namespace
* `unit` is a [String](/types/string). Dataset unit. Can be 'celsius', 'watt', etc.

## Examples:

To share temperature data from sensor, that is located near window:

```blocks
let temperature = samsungiot.getSensorTemp("Motion sensor")
let temperatureText = share.numberToText(temperature);
share.shareHistoricalData(temperatureText, "temperature near window", "class 5-B", "celsius");
```
