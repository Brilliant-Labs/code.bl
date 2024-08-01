# Move:  MAKE IT TURN!

![Mkt_Turn_Servo-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/5_Move/Move6/Mkt_Turn_Servo-EN.png?raw=true "Mkt_Turn_Servo-EN")

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