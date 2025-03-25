# 📒 b.Board Tutorial Clickboards:

# `CONTROL`

- [Button G](#button-g) 
- [Keylock](#keylock) 
- [Relay](#relay) 
- [Servo](#servo)
- [Motor](#motor)
- [Mini LCD](#mini-lcd)
---
## Button G
# Neopixels + Button_G
# ACTIVATE YOUR DANCE ON

![alt text](\docs\static\mb\projects\bboard-tutorials-full\2_Control\button-g\button_A.gif "For more info: www.brilliantlabs.ca")

Do you have this great, ultra luminous, neopixel project but no way of intiating your code? Look no further than the Button G ClickBoardTM. The Button G can be extended with our Expasion board from your bBoard to really get the light show started. Not only does the Button G have a very satisfying push, it also has an onboard LED to lure your party goers to push that button that is just waiting to be pushed. Happy Coding!

## STEP 1
**Plan your install.** Neopixels are really brilliant, but they do require some thought. Since each neopixel is indvidually addressable, which colour do you want, where does it appear on the strip, and how long will it be illuminated? Other questions to consider may include: 

 - How many neopixels do you require? 
 - Neopixel brightness? 
 - Does the light need to be diffused? 
 - Should I use a neopixel strip, ring, bare, breadboard, or some other variant? 
 - Will this installation need to last a while? Should you use the b.Board Gator Grabbers, the b.Board terminal blocks or maybe solder to the b.Board itself for a more permanent installation? 
 - How far will the Button G need to be from your b.Board? 
 - Any other ideas...

## STEP 2
**What is your project's < HELLO WORLD / > ?** 
When prototyping your code, it is great to start off with something that you know will work. The final version of your code will likely be extraordinarly complex - so don't stress yourself out - get motivated by starting with a simple set of blocks to get your project up and going. 

## Initialize your Neopixels
As brilliant as you belive your micro:bit and b.Board are, regrettably they are not. Should you just hook your neopixles to the Gator Grabbers and apply power to your b.Board and expect the neopixels to illuminate, you will be sadly mistaken. You must tell your micro:bit and b.Board where those neopiels are, how many are attached in sequence and their type. 
To do this, follow these steps: 

 1. Click the ``||Neopixel||`` category to reveal all your neopixel options. The following photo depicts an example strip setup. 
 ![enter image description here](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/button-g/neopixel_start_basic.png?raw=true)

 2. Choose a simple light pattern to send to your neopixel strip to discover if you have indeed initialized your strip correctly. Your sample code may resemble these blocks: 

```blocks
let strip = neopixel.create(DigitalPin.P0, 24, NeoPixelMode.RGB)
strip.setBrightness(100)
basic.forever(function () {
if (input.buttonIsPressed(Button.A)) {
strip.showColor(neopixel.colors(NeoPixelColors.Purple))
} else {
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
}
})
```

 2. If coded correctly, the blocks above should illuminate the strip blue, but when the ``||Button A: Is Pressed||``the strip should turn purple. **NOTE:** If you are running your b.Board off of a battery pack, you will want to reduce your ``||neopixel:more:brightness||``so that you don't need to replace your batteries every hour. Look at that brilliant purple! 
 
 ![alt text](\docs\static\mb\projects\bboard-tutorials-full\2_Control\button-g\button_A.gif "For more info: www.brilliantlabs.ca")

## STEP 3
**Click your way to a Button G** Ok, we know that pushing ``||Button A||`` on the micro:bit is pretty neat, but you know what is ~~neater~~ better? Using the following ClickBoardTM. Meet the glorious Button G. 

![alt text](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/button-g/glowy.gif?raw=true "For more info: www.brilliantlabs.ca")

This button can be setup similar to the code you created for the ``||Button A||``. You may want to consider how far you would like your button to be away from your b.Board. For this you will want to use either our (soon to be released) expansion board, or a [Shuttle Click](https://www.mikroe.com/shuttle-click). 

Use the following code to get your started: 
```blocks
let ButtonG2 = ButtonG.createButtonG(BoardID.zero, ClickID.A)
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
strip.setBrightness(100)
basic.forever(function () {
    if (ButtonG2.getSwitch() == 1) {
        strip.showColor(neopixel.colors(NeoPixelColors.Purple))
    } else {
        strip.showColor(neopixel.colors(NeoPixelColors.Blue))
    }
})
```
## Some reminders when using the blocks for Button G: 

 1. The depress/press of the button follows the common state of 0/1.
 2. Use the ``||Logic||``category to find the equality function. 
 3. Remember to look at the ClickBoard position you have used on your b.Board. 
 4. Try using the glowing commands to make your install extra glowy. 

![alt text](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/button-g/button_g_click.png?raw=true "For more info: www.brilliantlabs.ca")

## HAPPY MAKING. 
Remember to tweet your progress @brilliant_labs and hashtag #makeSomethingBrilliant.

---
##### [🔙 Back Menu](#control) 
---
## Keylock

![Keylock Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/keylock/keylock.jpg?raw=true "Keylock Click")

## Description

This locking mechanism Keylock Click BoardTM has an
integrated lock that can be used
as an input switch. It comes with
two keys which can become your
own, unique access point for your
code. Use our extension port to
place your keylock anywhere you
need. Also, this input sensor has
3 key positions: 0-2.

![Keylock Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/keylock/keylock-click.jpg?raw=true "Keylcok Click")

## Code Example

This example has the Keylock Click plugged into to MikroBus #1 on the b.Board.

The keylock has 3 positions available!

Locate the Keylock in Clickboards Buttons & switches group

```blocks
let Keylock2 = Keylock.createkeylock(BoardID.zero, ClickID.A)
basic.forever(function () {
    if (Keylock2.getLockPosition() == 0) {
        basic.showIcon(IconNames.No)
    } else if (Keylock2.getLockPosition() == 1) {
        basic.showIcon(IconNames.Yes)
    } else if (Keylock2.getLockPosition() == 2) {
        basic.showIcon(IconNames.Heart)
    }
})
```

## Project Idea

PROJECT PROTECTION

Be the only one who can run
your experiment, turn on
your robot or even enter your
mad scientist laboratory with this Keylock Click.


![Keylock](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/keylock/keylock-gif.gif?raw=true "Let's Keep things locked")
---
##### [🔙 Back Menu](#control) 
---
## Relay

![Relay](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/relay/relay.png?raw=true "Relay")

## Description

Controls a wide range of higher
powered devices. Have a battery
powered toy that you want to turn
into a smart device? This board
will allow that to happen.

PLEASE EXERCISE CAUTION
WHEN DEALING WITH HIGH
VOLTAGES. THIS SHOULD BE
USED UNDER STRICT ADULT
SUPERVISION.

![Relay](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/relay/relay-click.jpg?raw=true "Relay Click")

## Code Example

This example has the Relay Click plugged into to MikroBus #1 on the b.Board.

Locate the ``|| Relay ||`` blocks


```blocks
input.onButtonPressed(Button.A, function () {
    Relay2.relayOnOff(Relay.onOff.On, Relay.relay.Relay1)
})
input.onButtonPressed(Button.B, function () {
    Relay2.relayOnOff(Relay.onOff.Off, Relay.relay.Relay1)
})
let Relay2: Relay.Relay = null
Relay2 = Relay.createRelay(BoardID.zero, ClickID.A)
```

## Project Idea

HACK YOUR TOY

Complete or break any
circuit with the Relay Click
BoardTM. This nifty board acts
as an on/off switch for all
your circuitry needs.
Combine it with a WiFi BLE
Click BoardTM to offer remote
control wherever you have
internet access.


![Relay](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/relay/relayclick-gif.gif?raw=true "Let's Keep things nifty")
---
##### [🔙 Back Menu](#control) 
---
## Servo
![Servo Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servoinside.jpg?raw=true "Servo Click")

## Description

Have you noticed that your
b.Board has 6 on-board 5V servo
connectors but only 3 are
available to use at one time?
Does your project require even
more servos? All of your
questions are answered with this
board that offers 16 servo
connectors. 

![Servo Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servoarm.jpg?raw=true "Servo Click")

Just make sure you have your bBoard powered with a wall adapter.  Daisy chain up to 30 more Servo Clicks using the b.Board's expansion port to control more than 500 servo motors!

![Servo Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servo-click.jpg?raw=true "Servo Click")

## Code Example

This example has the Servo Click plugged into to MikroBus #1 on the b.Board. 

You can place the Servo Click's blocks to move your servo motors any way you like! 

```blocks

let Servo2 = Servo.createServo(BoardID.zero, ClickID.A)

input.onButtonPressed(Button.A, function () {
    Servo2.setServoAngle(1, 120)
    Servo2.setServoAngle(8, 90)
    Servo2.setServoAngle(16, 180)
    basic.pause(1000)
    Servo2.setServoAngle(1, 40)
    Servo2.setServoAngle(8, 120)
    Servo2.setServoAngle(16, 0)
})

```

## Project Idea

Interactive Art!

Keep your world, and your art, moving with the
ultimate servo click! This click
board can handle 16 servo
motors. Options are endless, and
collaborative servo projects are
encouraged! Try creating a moving
work of art friends.  Prefer Robots?  The servo click is your perfect companion to use 16 servos simultaneously!


![Servo](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servogif.gif?raw=true "Let's Keep things moving")
---
##### [🔙 Back Menu](#control) 
---
## Motor
![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/dcmotor.jpg?raw=true "Motor Click 3")

## Description

This motor driver will allow you to
pick up any DC motor you may
have hiding in your makerspace
and make it turn. Motors can be
larger than those yellow motors
that come with small robots. 

![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/gearmotor.jpg?raw=true "Motor Click 3")

With output capabilities of 3.5 A with 30V, you can make use of some very large motors.  


![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/dcpower.png?raw=true "Motor Click 3")

Just be sure to take a jumper cable and take 5V from the b.Board's servo rail or an other power source.

![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/motor-3-click.jpg?raw=true "Motor Click 3")

## Code Example

This example has the Motor 3 Click plugged into to MikroBus #1 on the b.Board. 

We will place the Motor Click 3's blocks wherever and however you want to make a DC motor move.  It could be from a button input, a condition of an IF / ELSE statement, or other input which actuates the Motor 3 click. 

```blocks
input.onButtonPressed(Button.A, function () {
    DC_Motor3.motorSpeedDirection(100, DC_Motor3.MotorDirection.Forward, clickBoardID.one)
    basic.pause(2000)
    DC_Motor3.motorSpeedDirection(0, DC_Motor3.MotorDirection.Reverse, clickBoardID.one)
})

```

## Project Idea

It's warm in here! Can you use the microbit's temperature sensor or the temp log 2 click to trigger a fan with the Motor 3 Click. Or make a gear motor move a car? 


![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/fangif.gif?raw=true "Let's Keep things spinning")
---
##### [🔙 Back Menu](#control) 
---
## Mini LCD
![NFC](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/lcd-mini/simplestLCD.jpg?raw=true "LCD MINI")

## Description

This two lined, mini LCD display
will let you display up to 16
characters on 2 different lines. Use this to add additional, text-based feedback to your project.

![LCD MINI](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/lcd-mini/lcd-mini-click.jpg?raw=true "LCD MINI Click")

## Code Example

This example has the LCD MINI Click plugged into to MikroBus #1 on the b.Board.

Just sent your text, strings, and input values to your LCD MINI with the the LCD Mini blocks or convert values or any responses you want listed on the LCD Mini's screen.

The screen currently has 2 lines to choose from and will display up to 16 characters each. 

The LCD MINI can help you display data and words to an LCD Screen. 

Locate the LCD_MINI blocks

```blocks
let LCDSettings = LCD_Mini.createLCDSettings(BoardID.zero, ClickID.A)
basic.forever(function () {
    LCDSettings.lcd_writeString("Hello", LCD_Mini.lineNumber.one)
    LCDSettings.lcd_writeString("World", LCD_Mini.lineNumber.two)
    basic.pause(1000)
    LCDSettings.lcd_clearDisplay()
})
```

## Project Idea

INTERACTIVE HAIKU

The format of a Haiku poem is
already perfect for this mini LCD
display. Construct a project
using multiple Click Boards to
allow you to interact and change
the tone of your Haiku based on
an external factor. Brilliant!


![Noise](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/lcd-mini/lcdgif.gif?raw=true "Let's Keep things noisy")
---
##### [🔙 Back Menu](#control) 
---