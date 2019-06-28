# Get Temperature

Get current temperature for city or by location postcode

```sig
weather.getTemperature(WeatherLocationType.city, "London,UK");
```

## Parameters

* `weatherLocationType` is choice value. It can be city or postcode.
* `location` is a [String](/types/string). It is city name or location postcode, followed by country code separated by a comma. 

## Examples:

To get current temperature in London:

```blocks
let temperature = weather.getTemperature(WeatherLocationType.city, "London,UK")
basic.showString(temperature)
```

To show what temperature is by Big Ben postcode (SW1A):

```blocks
let temperature = weather.getTemperature(WeatherLocationType.postcode, "SW1A,UK")
basic.showString(temperature)
```
