# Get My School Energy Usage For Weeks

Get selected energy type total usage for my school for selected duration in weeks

```sig
energy.querySchoolEnergyWeek(EnergyType.electricity, WeekType.last_week);
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `weekType` is choice value. Duration in weeks.

## Examples:

To get total electricity usage in my school for last 3 weeks:

```blocks
let energyUsage = energy.querySchoolEnergyWeek(EnergyType.electricity, WeekType._3_weeks_ago);
basic.showNumber(energyUsage);
```
