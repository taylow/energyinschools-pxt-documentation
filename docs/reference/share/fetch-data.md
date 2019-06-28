# Fetch data

Get data from other school cloud storage
```sig
share.fetchData("temperature in room", "AB123");
```

## Parameters

* `name` is a [String](/types/string). Data identifier 
* `targetSchool` is a [String](/types/string). Target school ID 

## Examples:

To get value, previously saved in storage as "temperature in room" in school with ID AB123:

```blocks
let temperature = share.fetchData("temperature in room", "AB123");
basic.showString(temperature)
```
