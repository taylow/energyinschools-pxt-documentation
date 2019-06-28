# Query carbon generation mix

Returns carbon generation mix for specific type

```sig
carbon.queryCarbonGenerationMix(GenerationMixType.coal);
```

## Parameters

* `mixType` is choice value. Carbon generation mix type.

## Examples:

To get carbon generation mix for coal type:

```blocks
let carbonGenerationMix = carbon.queryCarbonGenerationMix(GenerationMixType.coal)
basic.showNumber(carbonGenerationMix)
```
