# 📒 b.Board Tutorial Clickboards:

# `MOTION`

- [Reed](#reed) 
- [Motion Click](#motion-click) 
- [Proximity](#proximity) 
---
## Reed
![REED SENSOR](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/reed-sensor/reedswitch.png?raw=true "Reed Sensor")

## Description

Magnets always seem like magic.
Become a magician with a Reed
Sensor. 

![Reed Sensor Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/reed-sensor/reedgif1.gif?raw=true "Reed Sensor Click")

This switch has magnetic
contacts that remain separated
until a magnet is applied. With a
little logic, the reverse could also
be true.

![Reed Sensor Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/reed-sensor/reed-click.jpg?raw=true "Reed Sensor Click")

## Code Example

This example has the Reed Sensor Click plugged into to MikroBus #1 on the b.Board. 

We will place the Reed Sensor Click's value in an "IF / ELSE Statement" which we've nested inside a "Forever Loop". If the reed sensor picks up magnetism and is activated then we will evaluate that input then activate an output. This output could be lights, sounds, motors, servos, on even the micro:bit's onboard LEDs.   

```blocks
basic.forever(function () {
    if (Reed.isActivated(clickBoardID.one)) {
        basic.showIcon(IconNames.Yes)
    } else {
        basic.showIcon(IconNames.No)
    }
})
```

## Project Idea

SECRET SWITCH

Keep your precious
items safe by hiding a
Reed Sensor inside a
cabinet to trigger a
servo to lock and unlock
your treasure chest with
a magnet.


![Reed Sensor](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/reed-sensor/reedswitchgif.gif?raw=true "Let's Keep Things Safe")
---
##### [🔙 Back Menu](#motion) 
---
## Motion Click
![Motion Detection](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motion/motionSensor.jpg?raw=true "Motion Detection")

## Description

This sensor can detect motion up
to 1.7 metres away. There are two
sensors on board: a PIR as well as
a light dependent resistor. Finally,
should you need to change the
sensitivity of your sensor, simply
use your b.Board screwdriver
until you hit that sweet spot

![Motion Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motion/motion-click.jpg?raw=true "Motion Click")

## Code Example

This example has the Motion Click plugged into to MikroBus #1 on the b.Board. 

We will place the motion click value in an "IF Statement" which we've nested inside a "Forever Loop".  

```blocks
let Motion2 = Motion.createMotion(BoardID.zero, ClickID.A)

basic.forever(function () {
    if (Motion2.isDetected()) {
        basic.showIcon(IconNames.Yes)
        basic.showString("We have motion!")
    } else {
        basic.showIcon(IconNames.No)
        basic.showString("No Movement")
    }
})


```

## Project Idea

SOUND THE ALARM!

Use this motion detecting
sensor to secure your space.
Keep this sensor in a
bedroom or study space and
code it to alert you to the
presence of intruders


![Line Following](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motion/motion_gif.gif?raw=true "Let's Keep things centered")
---
##### [🔙 Back Menu](#motion) 
---
## Proximity
![Proximity Detection](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/proximity-2/proximity2.jpg?raw=true "Proximity Detection")

## Description

This sensor combines ambient
light and distance to an obstacle
to allow you to integrate
proximity awareness into your
project.  You can use on or the other, or both!

![Proximity-2 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/proximity-2/proximity-2-click.jpg?raw=true "Proximity-2 Click")

## Code Example

This example has the Proximity 2 Click plugged into to MikroBus #1 on the b.Board. 

We will place the proximity 2 click's value in an "IF / ELSE Statement" which we've nested inside a "Forever Loop".  We will compare this value then scroll a message on the Micro:Bit's onboard LEDs depending on if the proximity value is lesser than 10cm.

```blocks
let Proximity_22 = Proximity_2.createProximity_2(BoardID.zero, ClickID.A)
basic.forever(function () {
    if (Proximity_22.proximity_2_Read_Proximity() < 10) {
        basic.showString("This object is close!")
    } else {
        basic.showString("Not so close")
    }
})
```

## Project Idea

HANDS OFF!

Use this click for hands off
control. By simply raising
and lowering your hand over
the sensor, control the
volume, speed, or servo
angles of your project.


![Proximity 2](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/proximity-2/proximity2gif.gif?raw=true "Hands Off!")
---
##### [🔙 Back Menu](#motion) 
---