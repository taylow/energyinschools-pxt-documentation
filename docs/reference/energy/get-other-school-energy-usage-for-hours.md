# Get Other School Energy Usage For Hours

Get selected energy type total usage for other school for selected duration in hours

```sig
energy.queryEnergyHour(EnergyType.electricity, HourType._1_hour_ago, "AB123");
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `hourType` is choice value. Duration in hours.
* `schoolId` is a [String](/types/string). It is other school ID

## Examples:

To get total electricity usage in other school for last 5 hours:

```blocks
let energyUsage = energy.queryEnergyHour(EnergyType.electricity, HourType._5_hours_ago, "AB123");
basic.showNumber(energyUsage);
```
