# LED:  MAKE IT BLINK

![Mkt_Blink-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/3_LED/LED5/Mkt_Blink-EN.png?raw=true "Mkt_Blink-EN")

![Mkt_Blink-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/3_LED/LED5/Mkt_Blink-EN?raw=true "Mkt_Blink-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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