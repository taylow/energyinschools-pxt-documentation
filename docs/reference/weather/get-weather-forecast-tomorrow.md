# Get Tomorrows Weather Forecast 

Get tomorrows weather forecast for city or by location postcode

```sig
weather.getWeatherForecastTomorrow(WeatherLocationType.city, "London, UK");
```

## Parameters

* `weatherLocationType` is choice value. It can be city or postcode.
* `location` is a [String](/types/string). It is city name or location postcode, followed by country code separated by a comma. 

## Examples:

To get tomorrows weather forecast in London:

```blocks
let forecast = weather.getWeatherForecastTomorrow(WeatherLocationType.city, "London,UK")
basic.showString(forecast)
```

To show tomorrows weather forecast by Big Ben postcode (SW1A):

```blocks
let forecast = weather.getWeatherForecastTomorrow(WeatherLocationType.postcode, "SW1A,UK")
basic.showString(forecast)
```
