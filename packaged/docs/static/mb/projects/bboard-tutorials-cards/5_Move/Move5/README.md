# Move:  MAKE IT ROLL FOR LIMITED AMOUNTS OF TIME!

![Mkt_Roll-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/5_Move/Move5/Mkt_Roll-EN.png?raw=true "Mkt_Roll-EN")

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