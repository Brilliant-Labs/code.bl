# LED:  MAKE YOUR LIGHTS ROTATE

![Mk_Your_Lights_Rotate-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/3_LED/LED3/Mk_Your_Lights_Rotate-EN.png?raw=true "Mk_Your_Lights_Rotate-EN")

![Mk_Your_Lights_Rotate-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/3_LED/LED3/Mk_Your_Lights_Rotate-EN?raw=true "Mk_Your_Lights_Rotate-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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