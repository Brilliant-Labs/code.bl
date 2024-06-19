# LED:  MAKE IT LIGHT UP ADDRESSABLE RAINBOW LIGHTS

![Mkt_Light_Addressable_Rainbow-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/3_LED/LED1/Mkt_Light_Addressable_Rainbow-EN.png?raw=true "Mkt_Light_Addressable_Rainbow-EN")

## Code Example

Example AMAKE IT LIGHT UP ADDRESSABLE RAINBOW LIGHTS using the b.Board

```blocks

let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})

```