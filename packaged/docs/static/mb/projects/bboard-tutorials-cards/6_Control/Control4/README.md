# Control:  MAKE IT PUMP WATER

![Mkt_Pump_Water-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/6_Control/Control4/Mkt_Pump_Water-EN.png?raw=true "Mkt_Pump_Water-EN")

## Code Example

Example MAKE IT PUMP WATER using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorDuty(100)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorDuty(0)
})

```