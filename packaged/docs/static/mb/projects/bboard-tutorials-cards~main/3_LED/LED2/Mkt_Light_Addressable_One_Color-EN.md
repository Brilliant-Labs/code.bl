# LED:  MAKE IT LIGHT UP ADDRESSABLE LIGHTS ONE COLOR

![Mkt_Light_Addressable_One_Color-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/3_LED/LED2/Mkt_Light_Addressable_One_Color-EN.png?raw=true "Mkt_Light_Addressable_One_Color-EN")

## Code Example

Example MAKE IT LIGHT UP ADDRESSABLE LIGHTS ONE COLOR using the b.Board

```blocks

let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})

```