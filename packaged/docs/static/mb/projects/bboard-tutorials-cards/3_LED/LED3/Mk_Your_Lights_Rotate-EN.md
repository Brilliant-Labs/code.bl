# LED:  MAKE YOUR LIGHTS ROTATE

![Mk_Your_Lights_Rotate-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/3_LED/LED3/Mk_Rotate_Your_Lights-EN.png?raw=true "Mk_Your_Lights_Rotate-EN")

## Code Example

Example MAKE YOUR LIGHTS ROTATE using the b.Board

```blocks

let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
strip.showRainbow(1, 360)
basic.forever(function () {
strip.rotate(1)
strip.show()
})

```