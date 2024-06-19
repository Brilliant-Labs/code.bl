# LED:  MAKE IT LIGHT UP ADDRESSABLE LIGHTS ONE COLOR

![Mkt_Light_Addressable_One_Color-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/3_LED/LED2/Mkt_Light_Addressable_One_Color-EN.png?raw=true "Mkt_Light_Addressable_One_Color-EN")

![Mkt_Light_Addressable_One_Color-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/3_LED/LED2/Mkt_Light_Addressable_One_Color-EN.png?raw=true "Mkt_Light_Addressable_One_Color-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT LIGHT UP ADDRESSABLE LIGHTS ONE COLOR using the b.Board

```blocks

let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})

```