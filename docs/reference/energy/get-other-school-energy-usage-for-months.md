# Get Other School Energy Usage For Months

Get selected energy type total usage for other school for selected duration in months

```sig
energy.queryEnergyMonth(EnergyType.electricity, WeekType.last_month, "AB123");
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `monthType` is choice value. Duration in months.
* `schoolId` is a [String](/types/string). It is other school ID

## Examples:

To get total electricity usage in other school for last 2 months:

```blocks
let energyUsage = energy.queryEnergyMonth(EnergyType.electricity, MonthType._2_months_ago, "AB123");
basic.showNumber(energyUsage);
```
