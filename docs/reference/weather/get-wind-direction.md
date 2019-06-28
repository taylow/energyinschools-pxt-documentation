# Get Wind Direction

Get current wind direction for city or by location postcode

```sig
weather.getWindDirection(WeatherLocationType.city, "London, UK");
```

## Parameters

* `weatherLocationType` is choice value. It can be city or postcode.
* `location` is a [String](/types/string). It is city name or location postcode, followed by country code separated by a comma. 

## Examples:

To get current wind direction in London:

```blocks
let windDirection = weather.getWindDirection(WeatherLocationType.city, "London,UK")
basic.showString(windDirection)
```

To show what wind direction is by Big Ben postcode (SW1A):

```blocks
let windDirection = weather.getWindDirection(WeatherLocationType.postcode, "SW1A,UK")
basic.showString(windDirection)
```
