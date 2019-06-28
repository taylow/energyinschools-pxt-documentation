# Set bulb colour temperature value

Change current colour temperature level of bulb 

```sig
samsungiot.setBulbTemp("Sengled bulb", BulbTemp.soft_1);
```

## Parameters

* `name` is a [String](/types/string). Bulb device name.
* `colour` is a choice value. Colour temperature values.

## Examples:

To set colour temperature level of bulb, named "Sengled bulb", to soft:

```blocks
samsungiot.setBulbTemp("Sengled bulb", BulbTemp.soft_1)
```
