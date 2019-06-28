# Door Magnet Sensor

## Introduction @unplugged

The door open and close sensor was built by using a @boardname@ to sense the magnetic force of a magnet on the door. The pupils learn about magnetic force and how to program a @boardname@ to show a happy face when the door is closed and keeping heat in and a sad face when the door is open letting the air out.

![A smiling micro:bit attached to a door](/static/eis/tutorials/door-open-close/door-smile.jpg)

|Learning Objectives|Success Criteria|
|-|-|
|Use magnetic input though micro:bit sensors to change micro:bit LED display|All Pupils should be able to Use an IF…THEN…ELSE statement|
|Use magnetic input though micro:bit sensors to change micro:bit LED display|Display patterns on LED which change based on the IF…THEN…ELSE statement|

## Step 1 @fullscreen

Place the ``||logic:if||`` block in the ``||basic:forever||``.

![An animation that shows how to drag an if block](/static/eis/tutorials/door-open-close/add-if.gif)

## Step 2 @fullscreen

Place a ``||logic:comparison||`` block in the condition section of the ``||logic:if||`` block and select the greater than (>) comparison. This will allow you to compare two numbers against each other.

![An animation that shows how to drag a comparison block](/static/eis/tutorials/door-open-close/add-comparison.gif)

## Step 3 @fullscreen

In the comparison block, add a ``||input:magnetic force||`` block to the left hand side and set its type to ``Force``.

In the right hand side, enter the value ``50``.

![An animation that shows how to drag a magnetic force block](/static/eis/tutorials/door-open-close/add-force.gif)


This will now compare the strength of the magnetic field around the micro:bit against the number 50. When it is greater than 50 (when the door is closed and the @boardname@ is close to the magnet) the logic is true and the first section of the ``||logic:if||`` block will run.

## Step 4 @fullscreen

Add ``||basic:show icon||`` blocks to both parts of the ``||logic:if||`` block, setting the top one to a smiley face and the bottom one to a sad face.

```blocks
basic.forever(() => {
    if (input.magneticForce(Dimension.Strength) > 50) {
        basic.showIcon(IconNames.Happy)
    } else {
        basic.showIcon(IconNames.Sad)
    }
})
```

## Step 5 @fullscreen

If you have a @boardname@ connected, click ``|Download|`` to transfer your code. Hold a magnet close to the @boardname@ and watch the face change from sad to happy!
