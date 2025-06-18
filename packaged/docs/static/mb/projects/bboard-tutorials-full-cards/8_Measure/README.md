# 📒 b.Board Tutorial Cards / 📒 Cartes de tutoriel b.Board:

# `MEASURE-MESURER`

| English | French |
| ------------------------------- | ------------------------------- | 
| [Make it Measure Temp](#make-it-measure-temp) | [Fais le mesurer la temperature](#fais-le-mesurer-la-temperature) | 
| [Make it Sense Distance](#make-it-sense-distance) | [Fais le detecter la distance](#fais-le-detecter-la-distance) |
| [Make it Measure Magnetic Field](#make-it-measure-magnetic-field) | [Fais le mesurer le champ magnetique](#fais-le-mesurer-le-champ-magnetique) |
| [Make it Measure Humidity](#make-it-measure-humidity) | [Fais le mesurer l humidite](#fais-le-mesurer-l-humidite) | 
| [Make it Measure UV](#make-it-measure-uv) | [Fais le mesurer les uv](#fais-le-mesurer-les-uv) |
| [Make it Measure CO2](#make-it-measure-co2) | [Fais le mesurer le co2](#fais-le-mesurer-le-co2) |
| [Make it Measure Light](#make-it-measure-light) | [Fais le mesurer la lumiere](#fais-le-mesurer-la-lumiere) | 
| [Make it Compass](#make-it-compass) | [Fais le boussole](#fais-le-boussole) |

---
---
# `🇬🇧 ENGLISH`
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
##### 🔙 [Back Menu](#measure-mesurer) 
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
##### 🔙 [Back Menu](#measure-mesurer) 
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
##### 🔙 [Back Menu](#measure-mesurer) 
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
##### 🔙 [Back Menu](#measure-mesurer) 
---
## Make it Measure UV
![Mkt_Measure_UV-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure5/Mkt_Measure_UV-EN.png?raw=true "Mkt_Measure_UV-EN")
---
##### 🔙 [Back Menu](#measure-mesurer) 
---
## Make it Measure CO2
![Mkt_Measure_CO2-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure6/Mkt_Measure_CO2-EN.png?raw=true "Mkt_Measure_CO2-EN")
---
##### 🔙 [Back Menu](#measure-mesurer) 
---
## Make it Measure Light
![Measure_Light-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure7/Measure_Light-EN.png?raw=true "Measure_Light-EN")
---
##### 🔙 [Back Menu](#measure-mesurer) 
---
## Make it Compass
![Mkt_Compass-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure8/Mkt_Compass-EN.png?raw=true "Mkt_Compass-EN")
---
##### 🔙 [Back Menu](#measure-mesurer) 
---
---








# `🇫🇷 FRENCH`
---
---
## Fais le mesurer la temperature
![Mkt_Measure_Temp-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure1/Mkt_Measure_Temp-FR.png?raw=true "Mkt_Measure_Temp-FR")

## Exemple de code

Exemple FAIS-LE MESURER LA TEMPÉRATURE avec la b.Board

```blocks

basic.forever(function () {
basic.showNumber(input.temperature())
})

```
---
##### 🔙 [Menu Retour](#measure-mesurer) 
---
## Fais le detecter la distance
![Mkt_Sense_Distance-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure2/Mkt_Sense_Distance-FR.png?raw=true "Mkt_Sense_Distance-FR")

## Exemple de code

Exemple FAIS-LE DÉTECTER LA DISTANCE avec la b.Board

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
##### 🔙 [Menu Retour](#measure-mesurer) 
---
## Fais le mesurer le champ magnetique
![Mkt_Measure_Magnetic_Field-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure3/Mkt_Measure_Magnetic_Field-FR.png?raw=true "Mkt_Measure_Magnetic_Field-FR")

## Exemple de code

Exemple FAIS-LE MESURER LE CHAMP MAGNÉTIQUE avec la b.Board

```blocks

basic.forever(function () {
BLiXel.showBarGraph(input.magneticForce(Dimension.Strength), 1000)
})

```
---
##### 🔙 [Menu Retour](#measure-mesurer) 
---
## Fais le mesurer l humidite
![Mkt_Measure_Humidity-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure4/Mkt_Measure_Humidity-FR.png?raw=true "Mkt_Measure_Humidity-FR")

## Exemple de code

Exemple FAIS-LE MESURER L’HUMIDITÉ avec la b.Board

```blocks

input.onButtonPressed(Button.B, function () {
basic.clearScreen()
basic.showNumber(Weather2.humidity())
})
let Weather2: Weather.Weather = null
Weather2 = Weather.createWeather(BoardID.zero, ClickID.A)

```
---
##### 🔙 [Menu Retour](#measure-mesurer) 
---
## Fais le mesurer les UV
![Mkt_Measure_UV-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure5/Mkt_Measure_UV-FR.png?raw=true "Mkt_Measure_UV-FR")
---
##### 🔙 [Menu Retour](#measure-mesurer) 
---
## Fais le mesurer le CO2
![Mkt_Measure_CO2-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure6/Mkt_Measure_CO2-FR.png?raw=true "Mkt_Measure_CO2-FR")
---
##### 🔙 [Menu Retour](#measure-mesurer) 
---
## Fais le mesurer la lumiere
![Measure_Light-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure7/Measure_Light-FR.png?raw=true "Measure_Light-FR")
---
##### 🔙 [Menu Retour](#measure-mesurer) 
---
## Fais le boussole
![Mkt_Compass-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/8_Measure/Measure8/Mkt_Compass-FR.png?raw=true "Mkt_Compass-FR")
---
##### 🔙 [Menu Retour](#measure-mesurer) 