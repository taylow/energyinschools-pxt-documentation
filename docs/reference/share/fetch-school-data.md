# Fetch school data

Get data from own school cloud storage
```sig
share.fetchSchoolData("temperature in room");
```

## Parameters

* `name` is a [String](/types/string). Data identifier 

## Examples:

To get value, previously saved in storage as "temperature in room":

```blocks
let temperature = share.fetchSchoolData("temperature in room");
basic.showString(temperature)
```
