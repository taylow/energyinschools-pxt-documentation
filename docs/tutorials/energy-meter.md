# Micro:bit Energy Meter

## Introduction @unplugged

You can program a micro:bit to sense and collect the amount of watts an electric appliance is consuming. You can use it to monitor a computer, a kettle or any appliances that you want to find out the energy consumption of.

**Think!**
When you know how much energy a device uses, what actions can you take to reduce energy consumption?

| Learning Objectives | Success Criteria |
|-|-|
| Code the micro:bit to collect and display the amount of energy used from a device | All Pupils should be able to use button events |
| Use the micro:bit as a energy monitor | Display current energy use on the micro:bit |

## Step 1 @fullscreen

The micro:bit needs to be placed in a very specific location on the power cable of an appliance in order to accurately sense the magnetic force produced by current (electricity) flowing through a conductor (the wire).

To do this, we can use the ``||energymeter:calibrate||`` block found in the ``||energymeter:Energy Metering||`` section.

First, we must place an ``||input:on button A||`` event block down in the editor.

![An animation that shows how to drag an on button A block](/static/eis/tutorials/energy-meter/add-button-event.gif)

## Step 2 @fullscreen

Next, place the ``||energymeter:calibrate||`` block found in the ``||energymeter:Energy Metering||`` section into the body of the ``||input:on button A||`` event block.

![An animation that shows how to drag an on button A block](/static/eis/tutorials/energy-meter/add-calibrate.gif)

## Step 3 @fullscreen

Place another ``||input:on button A||`` event block down, and change the button to ``||input:button B||``.
              
![An animation that shows how to drag an on button A block and change the button](/static/eis/tutorials/energy-meter/add-button-B.gif)

## Step 4 @fullscreen

Next we need to display the value of the energy use in watts on the micro:bit's display.

To do this, add a ``||basic:show number||`` block inside of the ``||input:on button B||`` block. This will display a number once ``||input:button B||`` is pressed.

![An animation that shows how to drag a show number block](/static/eis/tutorials/energy-meter/add-show-number.gif)

## Step 5 @fullscreen

To display the amount of power being used in Watts, drag a ``||energymeter:get energy consumption (watts)||`` block into the ``||basic:show number||`` block.

![An animation that shows how to drag a get energy consumption (watts) block](/static/eis/tutorials/energy-meter/add-watts.gif)

## Step 6 @fullscreen

The complete code should look something like this.

```blocks
input.onButtonPressed(Button.A, function () {
    energymeter.calibrateEnergyMeter()
})
input.onButtonPressed(Button.B, function () {
    basic.showNumber(energymeter.getEnergyUsage())
})
```

## Step 7 @fullscreen

If you have a @boardname@ connected, click ``|Download|`` to transfer your code.

## Step 8 @unplugged

Attach the wire onto a cable using a hair bobble and run the calibration process by pressing ``||input:button A||``.

**NOTE: It is important that the device is turned on and working while you calibrate your micro:bit as it is using the electromagnetic force coming from the wire to calculate where the best place for the micro:bit to sit is.**

Slowly rotate the micro:bit around the cable once, then again until the line on the micro:bit's display is at the highest point you can get it to go (sometimes its VERY hard to get it to the top, but the higher the line is, the more accurate the reading will be!)

Lock in the calibration by pressing ``||input:button A + B||`` at the same time.

Here's a quick guide on how to do this:
https://vimeo.com/306384257

## Step 9 @unplugged

You should now be able to press ``||input:button B||`` for a reading of the energy consumption to be displayed on the micro:bit's display.