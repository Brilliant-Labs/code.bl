# LED:  MAKE IT LIGHT UP ADDRESSABLE RAINBOW LIGHTS

![Mkt_Light_Addressable_Rainbow-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/3_LED/LED1/Mkt_Light_Addressable_Rainbow-EN.png?raw=true "Mkt_Light_Addressable_Rainbow-EN")

![Add_Your_Name_Screen-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/3_LED/LED1/Mkt_Light_Addressable_Rainbow-EN.png?raw=true "Mkt_Light_Addressable_Rainbow-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example AMAKE IT LIGHT UP ADDRESSABLE RAINBOW LIGHTS using the b.Board

```blocks

let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})

```