# Move:  MAKE IT ROLL USING A TILT REMOTE - remote code

![Mkt_Roll_Tilt_Remote_Code-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/5_Move/Move2/Mkt_Roll_Tilt_Remote_Code-EN.png?raw=true "Mkt_Roll_Tilt_Remote_Code-EN")

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