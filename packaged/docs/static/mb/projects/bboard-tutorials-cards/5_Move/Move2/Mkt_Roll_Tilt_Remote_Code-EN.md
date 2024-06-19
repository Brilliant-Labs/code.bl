# Move:  MAKE IT ROLL USING A TILT REMOTE - remote code

![Mkt_Roll_Tilt_Remote_Code-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/5_Move/Move2/Mkt_Roll_Tilt_Remote_Code-EN.png?raw=true "Mkt_Roll_Tilt_Remote_Code-EN")

![Mkt_Roll_Tilt_Remote_Code-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/5_Move/Move2/Mkt_Roll_Tilt_Remote_Code-EN.png?raw=true "Adding_motors-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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