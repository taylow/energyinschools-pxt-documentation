# Clear

The clear function for images.

Turn off all the pixels in an [Image](/makecode-blockeditor/reference/images/image).

## JavaScript

```sig
export function clear(img: micro_bit.Image)
```

## Parameters

* none

## Example

The following example turns off the pixels of `img` when the A input button is pressed:

```blocks
let img = images.createImage(`
. . . . .
. # # # .
. # # # .
. # # # .
. . . . .
`)
img.showImage(0)
input.onButtonPressed(Button.A, () => {
    img.clear()
    img.showImage(0)
})
```

## See also

[Image](/makecode-blockeditor/reference/images/image), [show animation](/makecode-blockeditor/reference/basic/show-animation), [show image](/makecode-blockeditor/reference/images/show-image), [scroll image](/makecode-blockeditor/reference/images/scroll-image), [create image](/makecode-blockeditor/reference/images/create-image)

