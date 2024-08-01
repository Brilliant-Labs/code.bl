# Control:  PUMP UP AND DEFLATE A BALLON

![Pump_a_balloon-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/6_Control/Control2/Pump_a_balloon-EN.png?raw=true "Pump_a_balloon-EN")

## Code Example

Example PUMP UP AND DEFLATE A BALLON using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorLeftTimed(50, 1000)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorRightTimed(50, 1000)
})

```