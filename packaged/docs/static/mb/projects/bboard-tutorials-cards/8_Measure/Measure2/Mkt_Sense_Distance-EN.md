# Measure:  MAKE IT SENSE DISTANCE

![Mkt_Sense_Distance-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/8_Measure/Measure2/Mkt_Sense_Distance-EN.png?raw=true "Mkt_Sense_Distance-EN")

![Mkt_Sense_Distance-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/8_Measure/Measure2/Mkt_Sense_Distance-EN.png?raw=true "Mkt_Sense_Distance-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT SENSE DISTANCE using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
basic.showNumber(Ultrasonic_Sensor2.getDistance(Ultrasonic_Sensor.DistUnits.cm))
})
let Ultrasonic_Sensor2: Ultrasonic_Sensor.Ultrasonic_Sensor = null
Ultrasonic_Sensor2 = Ultrasonic_Sensor.createUltrasonic_Sensor(DigitalPin.P0, DigitalPin.P1)
basic.forever(function () {
if (Ultrasonic_Sensor2.getDistance(Ultrasonic_Sensor.DistUnits.cm) < 10) {
basic.showIcon(IconNames.No)
music.playMelody("C5 B A G F E D C ", 120)
}
})

```