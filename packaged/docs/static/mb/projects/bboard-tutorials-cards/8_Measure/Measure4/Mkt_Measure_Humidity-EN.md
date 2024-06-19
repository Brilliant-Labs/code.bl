# Measure:  MAKE IT MEASURE HUMIDITY

![Mkt_Measure_Humidity-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/8_Measure/Measure4/Mkt_Measure_Humidity-EN.png?raw=true "Mkt_Measure_Humidity-EN")

![Mkt_Measure_Humidity-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/8_Measure/Measure4/Mkt_Measure_Humidity-EN.png?raw=true "Mkt_Measure_Humidity-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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