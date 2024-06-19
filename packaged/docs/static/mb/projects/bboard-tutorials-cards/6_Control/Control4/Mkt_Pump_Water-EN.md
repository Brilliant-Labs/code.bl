# Control:  MAKE IT PUMP WATER

![Mkt_Pump_Water-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/6_Control/Control4/Mkt_Pump_Water-EN.png?raw=true "Mkt_Pump_Water-EN")

![Mkt_Pump_Water-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/6_Control/Control4/Mkt_Pump_Water-EN.png?raw=true "Mkt_Pump_Water-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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