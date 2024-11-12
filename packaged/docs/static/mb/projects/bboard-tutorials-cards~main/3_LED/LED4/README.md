# LED:  MAKE IT BLINK

![Mkt_Blink-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/3_LED/LED4/Mkt_Blink-EN.png?raw=true "Mkt_Blink-EN")

## Code Example

Example MAKE IT BLINK using the b.Board

```blocks

let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
basic.pause(500)
strip.showColor(neopixel.colors(NeoPixelColors.Black))
basic.pause(500)
})

```