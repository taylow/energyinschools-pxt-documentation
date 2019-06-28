# Clear Screen

Turn off all the LED lights on the [LED screen](/device/screen).

```sig
basic.clearScreen()
```

## Example: Vanishing heart

The following code shows a heart on the screen and then turns off all the LED lights.

```blocks
basic.showLeds(`
. # . # . 
# # # # # 
# # # # # 
. # # # . 
. . # . . 
`)
basic.clearScreen()
```

## See also

[set brightness](/makecode-blockeditor/reference/led/set-brightness), [unplot](/makecode-blockeditor/reference/led/unplot), [plot](/makecode-blockeditor/reference/led/plot), [Image](/makecode-blockeditor/reference/images/image)

