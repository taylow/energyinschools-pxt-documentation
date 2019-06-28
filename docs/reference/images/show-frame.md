# Show Frame

The show frame function.

Display an [Image](/makecode-blockeditor/reference/images/image) on the @boardname@'s [LED screen](/device/screen)

## JavaScript

```sig
export function showFrame(img: micro_bit.Image, frame: number)
```

## Parameters

* index - [Number](/types/number); which frame of the image to display

## Difference from `plot frame`

The `show frame` function is the same as [plot frame](/makecode-blockeditor/reference/images/plot-frame), but contains a built-in delay after the LED screen has been updated (whereas `plot frame` has no built-in delay)

## Example

```blocks
let img = images.createImage(`
# . . . # # . . . #
. # . # . . # # # .
. . # . . . # # # .
. # . # . . # # # .
# . . . # # . . . #
`)
img.showFrame(1)
```

## See also

[create image](/makecode-blockeditor/reference/images/create-image), [show animation](/makecode-blockeditor/reference/basic/show-animation), [image](/makecode-blockeditor/reference/images/image), [show image](/makecode-blockeditor/reference/images/show-image), [scroll image](/makecode-blockeditor/reference/images/scroll-image)

