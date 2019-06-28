# Get My School Energy Usage For Hours

Get selected energy type total usage for my school for selected duration in hours

```sig
energy.querySchoolEnergyHour(EnergyType.electricity, HourType._1_hour_ago);
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `hourType` is choice value. Duration in hours.

## Examples:

To get total electricity usage in my school for last 5 hours:

```blocks
let energyUsage = energy.querySchoolEnergyHour(EnergyType.electricity, HourType._5_hours_ago);
basic.showNumber(energyUsage);
```
