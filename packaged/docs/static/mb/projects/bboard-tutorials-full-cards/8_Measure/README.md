# 📒 b.Board Tutorial Cards:

# `MEASURE`

- [Make it Measure Temp](#make-it-measure-temp) 
- [Make it Sense Distance](#make-it-sense-distance) 
- [Make it Measure Magnetic Field](#make-it-measure-magnetic-field)
- [Make it Measure Humidity](#make-it-measure-humidity) 
- [Make it Measure UV](#make-it-measure-uv) 
- [Make it Measure CO2](#make-it-measure-co2) 
- [Make it Measure Light](#make-it-measure-light) 
- [Make it Compass](#make-it-compass) 
---
## Make it Measure Temp
![Mkt_Measure_Temp-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure1/Mkt_Measure_Temp-EN.png?raw=true "Mkt_Measure_Temp-EN")

## Code Example

Example MAKE IT MEASURE TEMPERATURE using the b.Board

```blocks

basic.forever(function () {
basic.showNumber(input.temperature())
})

```
---
##### 🔙 [Back Menu](#measure) 
---
## Make it Sense Distance
![Mkt_Sense_Distance-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure2/Mkt_Sense_Distance-EN.png?raw=true "Mkt_Sense_Distance-EN")

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
---
##### 🔙 [Back Menu](#measure) 
---
## Make it Measure Magnetic Field
![Mkt_Measure_Magnetic_Field-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure3/Mkt_Measure_Magnetic_Field-EN.png?raw=true "Mkt_Measure_Magnetic_Field-EN")

## Code Example

Example MAKE IT MEASURE MAGNETIC FIELD using the b.Board

```blocks

basic.forever(function () {
BLiXel.showBarGraph(input.magneticForce(Dimension.Strength), 1000)
})

```
---
##### 🔙 [Back Menu](#measure) 
---
## Make it Measure Humidity
![Mkt_Measure_Humidity-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure4/Mkt_Measure_Humidity-EN.png?raw=true "Mkt_Measure_Humidity-EN")

## Code Example

Example MAKE IT MEASURE HUMIDITY using the b.Board

```blocks

input.onButtonPressed(Button.B, function () {
basic.clearScreen()
basic.showNumber(Weather2.humidity())
})
let Weather2: Weather.Weather = null
Weather2 = Weather.createWeather(BoardID.zero, ClickID.A)

```
---
##### 🔙 [Back Menu](#measure) 
---
## Make it Measure UV
![Mkt_Measure_UV-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure5/Mkt_Measure_UV-EN.png?raw=true "Mkt_Measure_UV-EN")
---
##### 🔙 [Back Menu](#measure) 
---
## Make it Measure CO2
![Mkt_Measure_CO2-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure6/Mkt_Measure_CO2-EN.png?raw=true "Mkt_Measure_CO2-EN")
---
##### 🔙 [Back Menu](#measure) 
---
## Make it Measure Light
![Measure_Light-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure7/Measure_Light-EN.png?raw=true "Measure_Light-EN")
---
##### 🔙 [Back Menu](#measure) 
---
## Make it Compass
![Mkt_Compass-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure8/Mkt_Compass-EN.png?raw=true "Mkt_Compass-EN")
---
##### 🔙 [Back Menu](#measure) 
---