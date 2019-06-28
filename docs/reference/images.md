# Images

Create, show, and scroll images on the LED display.

```cards
images.createImage(`
. . . . .
. . . . .
. . # . .
. . . . .
. . . . .
`);
images.createBigImage(`
. . . . .
. . . . .
. . # . .
. . . . .
. . . . .
`);
images.createImage(``).showImage(0);
images.createImage(``).scrollImage(0,0);
images.arrowImage(ArrowNames.North)
images.iconImage(IconNames.Heart)
images.arrowNumber(ArrowNames.North)
```

## See Also

[createImage](/makecode-blockeditor/reference/images/create-image), [createBigImage](/makecode-blockeditor/reference/images/create-big-image),
[showImage](/makecode-blockeditor/reference/images/show-image), [scrollImage](/makecode-blockeditor/reference/images/scroll-image),
[arrowImage](/makecode-blockeditor/reference/images/arrow-image), [iconImage](/makecode-blockeditor/reference/images/icon-image), [arrowNumber](/makecode-blockeditor/reference/images/arrow-number), 
[pixel](/makecode-blockeditor/reference/images/pixel), [set-pixel](/makecode-blockeditor/reference/images/set-pixel)
