# Get My School Energy Usage For Months

Get selected energy type total usage for my school for selected duration in months

```sig
energy.querySchoolEnergyMonth(EnergyType.electricity, MonthType.last_month);
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `monthType` is choice value. Duration in months.

## Examples:

To get total electricity usage in my school for last month:

```blocks
let energyUsage = energy.querySchoolEnergyMonth(EnergyType.electricity, MonthType.last_month);
basic.showNumber(energyUsage);
```
