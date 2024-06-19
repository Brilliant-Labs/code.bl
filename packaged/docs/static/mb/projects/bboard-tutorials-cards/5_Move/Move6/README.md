# Move:  MAKE IT TURN!

![Mkt_Turn_Servo-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/5_Move/Move6/Mkt_Turn_Servo-EN.png?raw=true "Mkt_Turn_Servo-EN")

![Adding_motors-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/5_Move/Move6/Mkt_Turn_Servo-EN.png?raw=true "Mkt_Turn_Servo-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example
 
ExampleMAKE IT TURN! using the b.Board

```blocks

let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
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