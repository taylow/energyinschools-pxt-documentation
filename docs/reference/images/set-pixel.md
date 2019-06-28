# Set Pixel

Set the on/off state of pixel in an [Image](/makecode-blockeditor/reference/images/image).

## JavaScript

```sig
let item: Image = null;
item.setPixel(0, 0, true)
```

## Parameters

* x - [Number](/types/number); the *x coordinate* or horizontal position of a pixel in an [image](/makecode-blockeditor/reference/images/image)
* y - [Number](/types/number); the *y coordinate* or vertical position of a pixel in an [image](/makecode-blockeditor/reference/images/image)
* value -[Boolean](/blocks/logic/boolean); the on/off state of a pixel; `true` for on, `false` for off

## x, y coordinates?

To figure out the ``x``, ``y`` coordinates, see [LED screen](/device/screen).

## Example

The following example creates an image and stores it in the `img` variable. The `set pixel` function sets the center pixel off, before `img` is shown using `show image`.

```blocks
let img = images.createImage(`
. . # . .
. # . # .
. . # . .
. # . # .
. . # . .
`)
img.setPixel(2, 2, false)
img.showImage(0)
```
 ## See also

 [pixel](/makecode-blockeditor/reference/images/pixel), [show image](/makecode-blockeditor/reference/images/show-image), [image](/makecode-blockeditor/reference/images/image), [create image](/makecode-blockeditor/reference/images/create-image), [scroll image](/makecode-blockeditor/reference/images/scroll-image)