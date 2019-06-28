# Get My School Energy Usage For Days

Get selected energy type total usage for my school for selected duration in days

```sig
energy.querySchoolEnergyDay(EnergyType.electricity, DayType.yesterday);
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `dayType` is choice value. Duration in days.

## Examples:

To get total electricity usage in my school for last 2 days:

```blocks
let energyUsage = energy.querySchoolEnergyDay(EnergyType.electricity, DayType._2_days_ago);
basic.showNumber(energyUsage);
```
