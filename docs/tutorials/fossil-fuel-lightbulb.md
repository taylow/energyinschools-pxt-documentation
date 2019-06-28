# Fossil Fuel Light Bulb Controller

## Introduction @unplugged

You can code a @boardname@ to change a light bulb's colour based on the level of fossil fuels currently being used to generate electricity. You can make the light bulb turn red when using fossil fuels and turn green when using wind or solar power.

![IoT bulbs changing colour](/static/eis/tutorials/fossil-fuel-lightbulb/bulbs-changing-colour.gif)

| Learning Objectives | Success Criteria |
|-|-|
| To explore how you can code the @boardname@ to read if the carbon index level is high | All pupils should be able to use an IF…THEN…ELSE statement |
| Use the @boardname@ as a controller for an IoT device | Change the colour of the light bulb on pressing button A based on the IF…THEN…ELSE statement |

## Step 1 @fullscreen

Place an ``||input:on button A||`` event block down in the editor.

![An animation that shows how to drag an on button A block](/static/eis/tutorials/fossil-fuel-lightbulb/add-button-event.gif)

## Step 2 @fullscreen

Place an ``||logic:if then else||`` block inside of the ``||input:on button A||``. This will eventually allow you to run two separate pieces of code depending on the condition.

![An animation that shows how to drag an if block](/static/eis/tutorials/fossil-fuel-lightbulb/add-if-logic.gif)

## Step 3 @fullscreen

Place a ``||logic:comparison||`` block in the condition section of the ``||logic:if then else||`` block and select the `equal to` ( = ) comparison. This will allow you to compare two values against each other and will become true if they are the same.

![An animation that shows how to drag a comparison block](/static/eis/tutorials/fossil-fuel-lightbulb/add-condition.gif)

## Step 4 @fullscreen

In the comparison block, add a ``||carbon:get carbon index level||`` block to the left hand side of the condition check.

![An animation that shows how to drag a carbon block](/static/eis/tutorials/fossil-fuel-lightbulb/add-carbon-index.gif)

## Step 5 @fullscreen

In the right hand side of the comparison block, add a ``||carbon:carbon index level||`` block and change the value to `high`.

![An animation that shows how to drag a carbon block](/static/eis/tutorials/fossil-fuel-lightbulb/add-carbon-level-high.gif)

This will now compare the current carbon index level (from https://carbonintensity.org.uk/) with a "high" value. When the carbon index is considered high, the logic is true and the first section of the ``||logic:if||`` block will run.

## Step 6 @fullscreen

Now we have the IF THEN ELSE logic set up to run the first section of code when the carbon index level is `high`, and the second section of code when the carbon index is not high, we can now add the code that runs for each.

In the first section, add a ``||samsungiot:turn bulb to colour||`` block and set the smart bulb's colour to `red`.

![An animation that shows how to drag an IoT block](/static/eis/tutorials/fossil-fuel-lightbulb/add-iot-bulb.gif)

## Step 7 @fullscreen

The bulb name should be set to the name of one of the smart bulbs found on the Energy in Schools Device Management page.

![An animation that shows how to drag an IoT block](/static/eis/tutorials/fossil-fuel-lightbulb/device-management.png)

**Note: If the bulb is not working, make sure the device has been allowed for use**

## Step 8 @fullscreen

Repeat the previous steps and add another ``||samsungiot:turn bulb to colour||`` block to the second part of the ``||logic:if||`` block. This time, set the colour to green!

```blocks
input.onButtonPressed(Button.A, function () {
    if (carbon.queryCarbonIndex() == carbon.setCarbonIndexValueType(CarbonIndex.high)) {
        samsungiot.setBulbColour("bulb", BulbColour.red)
    } else {
        samsungiot.setBulbColour("bulb", BulbColour.green)
    }
})
```

## Step 9 @fullscreen

If you have a @boardname@ connected, click ``|Download|`` to transfer your code. Press button A and watch the smart bulb light up and change colour.

Note: Visit https://carbonintensity.org.uk/ to see the current energy information used to control this bulb!

Extension: You could also set button B to display the ``||carbon:get carbon index level||`` to see what the current value is!