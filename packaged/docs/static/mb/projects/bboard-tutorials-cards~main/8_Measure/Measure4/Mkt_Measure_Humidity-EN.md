# Measure:  MAKE IT MEASURE HUMIDITY

![Mkt_Measure_Humidity-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/8_Measure/Measure4/Mkt_Measure_Humidity-EN.png?raw=true "Mkt_Measure_Humidity-EN")

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