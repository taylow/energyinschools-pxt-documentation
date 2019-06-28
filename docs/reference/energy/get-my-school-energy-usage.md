# Get My School Energy Usage

Get selected energy type current usage for my school 

```sig
energy.querySchoolEnergy(EnergyType.electricity);
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.

## Examples:

To get current electricity usage in my school:

```blocks
let energyUsage = energy.querySchoolEnergy(EnergyType.electricity);
basic.showNumber(energyUsage);
```
