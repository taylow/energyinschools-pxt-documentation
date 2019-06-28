# Get Other School Energy Usage

Get selected energy type current usage for other school 

```sig
energy.queryEnergy(EnergyType.electricity, "AB123");
```

## Parameters

* `energyType` is choice value. It can be electricity or gas.
* `schoolId` is a [String](/types/string). It is other school ID

## Examples:

To get current electricity usage in school "AB123":

```blocks
let energyUsage = energy.queryEnergy(EnergyType.electricity, "AB123");
basic.showNumber(energyUsage);
```
