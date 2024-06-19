# Move:  MAKE IT ROLL FOR LIMITED AMOUNTS OF TIME!

![Mkt_Roll-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/5_Move/Move5/Mkt_Roll-EN.png?raw=true "Mkt_Roll-EN")

![Mkt_Roll-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/5_Move/Move5/Mkt_Roll-EN.png?raw=true "Mkt_Roll-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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