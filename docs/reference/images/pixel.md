# Pixel

Get the state of a pixel in an [Image](/makecode-blockeditor/reference/images/image).


## JavaScript

```sig
let item: Image = null;
item.pixel(0, 0)
```
## Parameters

* x - [Number](/types/number); the *x coordinate* or horizontal position of a pixel in an [image](/makecode-blockeditor/reference/images/image)
* y - [Number](/types/number); the *y coordinate* or vertical position of a pixel in an [image](/makecode-blockeditor/reference/images/image)

## x, y coordinates?

To figure out the ``x``, ``y`` coordinates, see [LED screen](/device/screen).

## Returns

* [Boolean](/blocks/logic/boolean) - `true` for on and `false` for off

## Example

This example gets the state of pixel `0, 0` in the `img` variable:

```blocks
let img = images.createImage(`
. . # . . . . . . .
. # . # . . . # . .
. . # . . . . . . .
. # . # . . . # . .. . # . . . . . . .
`)
let state = img.pixel(0, 0)
```

## See also

[set pixel](/makecode-blockeditor/reference/images/set-pixel), [show image](/makecode-blockeditor/reference/images/show-image), [image](/makecode-blockeditor/reference/images/image), [create image](/makecode-blockeditor/reference/images/create-image), [scroll image](/makecode-blockeditor/reference/images/scroll-image)