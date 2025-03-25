# 📒 b.Board Tutorial Clickboards:

# `OPTICAL`

- [IR Distance](#ir-distance) 
- [IR Thermo](#ir-thermo) 
- [Line Follower](#line-follower) 
- [UV 3](#uv-3) 
---
## IR Distance
![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Description

Using a combination of IR LEDs
and signal processing, this
distance sensor is great for
measuring objects or obstacles at 
distances between 10 and 150 cm!

![IR Distance Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/ir-distance-click.jpg?raw=true "IR DISTANCE Click")

## Code Example

This example has the IR Distance Click plugged into to MikroBus #1 on the b.Board

```blocks
let IR_Distance2 = IR_Distance.createIR_Distance(BoardID.zero, ClickID.A)
basic.forever(function () {
    if (IR_Distance2.getDistance() < 30) {
        basic.showString("Near")
    } else {
        basic.showString("Far")
    }
    basic.pause(1000)
})
```

## Project Idea

THE MAGICIAN'S ASSISTANT

This sensor detects the presence of any object that is between 10 and 150 cm from its sensor. Create your own illusions by activating and deactivating a magic trick of your own design. Pull an object out of a hat and place it near the sensor to act as your own magical assistant! 

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/magicianGif.gif?raw=true "A magician's assistant")
---
##### [🔙 Back Menu](#optical) 
---
## IR Thermo
![IR Thermo](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-thermo-3/howIRthermoWorks.png?raw=true "IR Thermo")

## Description

Using thermal imaging, this
sensor, once pointed at the object
in question, will provide a
contactless temperature reading which can be displayed, evaluated, or sent to the cloud for further analysis. 

![IR THERMO 3 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-thermo-3/ir-thermo-3-click.jpg?raw=true "IR THERMO 3 Click")

## Code Example

This example has the IR THERMO 3 Click plugged into to MikroBus #1 on the b.Board and if the temperature is higher than 20 degrees Celcius we are activating a fan with the DC motor click on MidroBus #2 onk the b.Board.  You can substitue the DC Motor click with anything you like including displaying something on the Micro:Bit's LEDs, turning on Neopixels, servos, etc... 

```blocks
let IrThermo_32 = IrThermo_3.createIrThermo(BoardID.zero, ClickID.A)
basic.forever(function () {
    if (IrThermo_32.getObjectTemp(IrThermo_3.TempUnits.C) < 20) {
        basic.showString("It's cold!")
    } else {
        basic.showString("It's warm! Turn on the fan :)")
        bBoard_Motor.motorLeftTimed(100, 5000)
    }
})


```

## Project Idea

A WATCHED POT NEVER BOILS

Have you ever heard the saying "A
watched pot never boils?" Keep tabs
on your stovetop or kettle from afar
with the IrThermo 3 sensor. This
sensor does not have to be in
contact with the object it is
measuring. It can also be used to
safely measure anything in hard to
reach places or hot things from a safe place!

![Boiling Pot](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-thermo-3/boilingGIF.gif?raw=true "Too hot? Stay safe!")
---
##### [🔙 Back Menu](#optical) 
---
## Line Follower
![Line Follower](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/line-follower/linefollowing.jpeg?raw=true "Line Follower")

## Description

If you are interested in becoming
an autonomous car engineer,
then you want to make sure your
vehicle stays on course. This line
follower has an array of 5
reflective sensors that sense the
difference in surface contrast

![Line Follower Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/line-follower/line-follower-click.jpg?raw=true "Line Follower Click")

## Code Example

This example has the LINE FOLLOWER Click plugged into to MikroBus #1 on the b.Board. This example also has the forward and backwards movement of the robot controlled by a DC motor plugged into DC Motor on the b.Board.  We are using a servo motor to control the stearing which is plugged into P0 on the b.Board's servo rail. 

We first set the robot in a forward motion at a speed of 50.  Let's be careful not to go too fast or we may affect the line follower values.  Please note that we are following a black line in this example.

We've set a variable named "Correction" where we will store the value of the Line Follower then adjust the steering of the robot according to the Line Follower values. 

```blocks
let Line_Follower2 = Line_Follower.createLineFollower(BoardID.zero, ClickID.A)
bBoard_Motor.motorRightDuty(50)
bBoard_Motor.motorLeftDuty(50)
basic.forever(function () {
    if (Line_Follower2.getDirectionEnum(Line_Follower.lineDetection.soft_right_turn)) {
        pins.servoWritePin(AnalogPin.P0, 75)
        if (Line_Follower2.getDirectionEnum(Line_Follower.lineDetection.soft_left_turn)) {
            pins.servoWritePin(AnalogPin.P0, 105)
        }
        if (Line_Follower2.getDirectionEnum(Line_Follower.lineDetection.no_correction)) {
            pins.servoWritePin(AnalogPin.P0, 90)
        }
    }
})


```

## Project Idea

A LONG AND WINDING ROAD

Attach this sensor to
any robotic design for
line following
capabilities. Forge your
own path by making
roads and mazes for
your robot to follow.

![Line Following](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/line-follower/robot_moving.gif?raw=true "Let's Keep things centered")
---
##### [🔙 Back Menu](#optical) 
---
## UV 3
![UV 3 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/uv3/ice.jpg?raw=true "UV 3 click")

## Description

This board is an advanced ultraviolet (UV) light sensor.  It can be used for UV measurement, sun exposure protection devices, display backlighting control based on received ambient or UV light

![UV 3 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/uv3/uv3-click.jpg?raw=true "UV 3 Click")

## Code Example

This example has the UV 3 Click plugged into to MikroBus #1 on the b.Board. 

We will place the UV 3 click value in a "ButtonPressed" event.  As soon as A button is pressed, we trigger the UV3 reading and display it as a message.

```blocks
input.onButtonPressed(Button.A, function () {
    basic.clearScreen()
    basic.showString("" + (UV_32.UVSteps()))
})
let UV_32: UV_3.UV_3 = null
UV_32 = UV_3.createUV_3(BoardID.zero, ClickID.A)
```

## Project Idea

SUN UV 3 AUTOMATIC ALERT

Protection from high UV 3 levels!, Let this sensor stay
outside and pair it with a Wifi Click to
inform you of the UV level while you
enjoy inside. The Wifi click
can be coded to turn on a lamp on your
chest of drawers to indicate that it is
high UV 3 level, and remind you to use 
enough SUN screen before you leave.


![Cold Gif](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/uv3/cold.gif?raw=true "It's Cold!")
---
##### [🔙 Back Menu](#optical) 
---