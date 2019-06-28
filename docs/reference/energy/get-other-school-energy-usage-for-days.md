# Get Other School Energy Usage For Days

Get selected energy type total usage for other school for selected duration in days

```sig
energy.queryEnergyDay(EnergyType.electricity, DayType.yesterday, "AB123");
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `dayType` is choice value. Duration in days.
* `schoolId` is a [String](/types/string). It is other school ID

## Examples:

To get total electricity usage in other school for last 3 days:

```blocks
let energyUsage = energy.queryEnergyDay(EnergyType.electricity, DayType._3_days_ago, "AB123");
basic.showNumber(energyUsage);
```
