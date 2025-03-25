# 📒 b.Board Tutorial Cards:

# `MOVE`

- [Adding Motors](#adding-motors) 
- [Make it Roll Tilt Remote Code](#make-it-roll-tilt-remote-code) 
- [Make it Roll Vehicule Code](#make-it-roll-vehicule-code) 
- [Make it Button RC](#make-it-button-rc) 
- [Make it Roll](#make-it-roll)
- [Make it Turn Servo](#make-it-turn-servo) 
- [Make it Intruder Alert](#make-it-intruder-alert) 
- [Make it React Movement](#make-it-react-movement)
---
## Adding Motors
![Adding_motors-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move1/Adding_motors-EN.png?raw=true "Adding_motors-EN")

---
##### 🔙 [Back Menu](#move) 
---
---
## Make it Roll Tilt Remote Code
![Mkt_Roll_Tilt_Remote_Code-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move2/Mkt_Roll_Tilt_Remote_Code-EN.png?raw=true "Mkt_Roll_Tilt_Remote_Code-EN")

## Code Example

Example MAKE IT ROLL USING A TILT REMOTE - remote code using the b.Board

```blocks

input.onGesture(Gesture.LogoUp, function () {
radio.sendNumber(1)
})
input.onGesture(Gesture.TiltLeft, function () {
radio.sendNumber(3)
})
input.onGesture(Gesture.TiltRight, function () {
radio.sendNumber(4)
})
input.onGesture(Gesture.LogoDown, function () {
radio.sendNumber(2)
})
radio.setGroup(1)

```
---
##### 🔙 [Back Menu](#move) 
---
---
## Make it Roll Vehicule Code
![Mkt_Roll_Vehicule_Code-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move3/Mkt_Roll_Vehicule_Code-EN.png?raw=true "AMkt_Roll_Vehicule_Code-EN")

## Code Example

Example MAKE IT ROLL USING A REMOTE vehicule code using the b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
if (receivedNumber == 1) {
bBoard_Motor.motorLeftDuty(50)
bBoard_Motor.motorRightDuty(100)
} else if (receivedNumber == 2) {
bBoard_Motor.motorLeftDuty(100)
bBoard_Motor.motorRightDuty(50)
} else if (receivedNumber == 3) {
bBoard_Motor.motorDuty(100)
} else if (receivedNumber == 4) {
bBoard_Motor.motorDuty(-100)
} else {

}
})
radio.setGroup(1)

```
---
##### 🔙 [Back Menu](#move) 
---
---
## Make it Button RC
![Mkt_Button_RC-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move4/Mkt_Button_RC-EN.png?raw=true "Mkt_Button_RC-EN")

## Code Example

Example MAKE IT ROLL USING A BUTTON REMOTE CONTROL remote code using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendNumber(1)
})
input.onButtonPressed(Button.AB, function () {
radio.sendNumber(2)
})
input.onButtonPressed(Button.B, function () {
radio.sendNumber(3)
})
radio.setGroup(1)

```
---
##### 🔙 [Back Menu](#move) 
---
---
## Make it Roll
![Mkt_Roll-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move5/Mkt_Roll-EN.png?raw=true "Mkt_Roll-EN")

## Code Example

Example MAKE IT ROLL FOR LIMITED AMOUNTS OF TIME! using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorLeftTimed(100, 5000)
})
input.onButtonPressed(Button.AB, function () {
bBoard_Motor.motorTimed(100, 5000)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorRightTimed(100, 5000)
})

```
---
##### 🔙 [Back Menu](#move) 
---
---
## Make it Turn Servo
![Mkt_Turn_Servo-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move6/Mkt_Turn_Servo-EN.png?raw=true "Mkt_Turn_Servo-EN")

## Code Example
 
ExampleMAKE IT TURN! using the b.Board

```blocks

basic.forever(function () {
for (let index = 0; index < 4; index++) {
pins.servoWritePin(AnalogPin.P0, 0)
basic.pause(1000)
pins.servoWritePin(AnalogPin.P0, 45)
basic.pause(1000)
pins.servoWritePin(AnalogPin.P0, 0)
basic.pause(1000)
}
})

```
---
##### 🔙 [Back Menu](#move) 
---
---
## Make it Intruder Alert
![Mk_Intruder_Alert-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move7/Mk_Intruder_Alert-EN.png?raw=true "Mk_Intruder_Alert-EN")

## Code Example

Example MAKE AN INTRUDER ALERT using the b.Board

```blocks

let Motion2 = Motion.createMotion(BoardID.zero, ClickID.A)
Motion2.onMotionDetected(function () {
for (let index = 0; index < 4; index++) {
music.playTone(262, music.beat(BeatFraction.Whole))
BLiXel.showColour(0xff0000)
}
})

```
---
##### 🔙 [Back Menu](#move) 
---
---
## Make it React Movement
![Mkt_React_Movement-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move8/Mkt_React_Movement-EN.png?raw=true "Mkt_React_Movement-EN")

## Code Example

Example MAKE IT REACT TO MOVEMENT using the b.Board

```blocks

input.onGesture(Gesture.Shake, function () {
for (let index = 0; index < 4; index++) {
BLiXel.showColour(0xff0000)
basic.pause(500)
BLiXel.showColour(0x000000)
basic.pause(500)
}
})

```
---
##### 🔙 [Back Menu](#move) 
---
