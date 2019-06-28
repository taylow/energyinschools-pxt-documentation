# Get Other School Energy Usage For Weeks

Get selected energy type total usage for other school for selected duration in weeks

```sig
energy.queryEnergyWeek(EnergyType.electricity, WeekType.last_week, "AB123");
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `weekType` is choice value. Duration in weeks.
* `schoolId` is a [String](/types/string). It is other school ID

## Examples:

To get total electricity usage in other school for last 2 weeks:

```blocks
let energyUsage = energy.queryEnergyWeek(EnergyType.electricity, WeekType._2_weeks_ago, "AB123");
basic.showNumber(energyUsage);
```
