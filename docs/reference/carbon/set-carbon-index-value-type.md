# Set carbon index value type

Returns carbon index value type

```sig
carbon.setCarbonIndexValueType(CarbonIndex.moderate);
```

## Parameters

* `index` is choice value. Carbon index that should be returned.

## Examples:

To return moderate carbon index value:

```blocks
let carbonIndex = carbon.setCarbonIndexValueType(CarbonIndex.moderate)
basic.showNumber(carbonIndex)
```
