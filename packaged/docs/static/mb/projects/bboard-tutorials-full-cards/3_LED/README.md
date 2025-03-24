# 📒 b.Board Tutorial Cards:

# `LEDS`

- [Make it Light Addressable Rainbow](#make-it-light-addressable-rainbow) 
- [Make it Light Addressable One Color](#make-it-light-addressable-one-color) 
- [Make it Light Your Lights Rotate](#make-it-your-lights-rotate) 
- [Make it Blink](#make-it-blink) 
- [Make it Control Lights Sound](#make-it-control-lights-sound)

---
## Make it Light Addressable Rainbow
![Mkt_Light_Addressable_Rainbow-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED1/Mkt_Light_Addressable_Rainbow-EN.png?raw=true "Mkt_Light_Addressable_Rainbow-EN")
### Code Example
Example MAKE IT LIGHT UP ADDRESSABLE RAINBOW LIGHTS using the b.Board
```blocks
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})
```
---
##### [🔙 Back Menu](#leds) 
---
## Make it Light Addressable One Color
![Mkt_Light_Addressable_One_Color-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED2/Mkt_Light_Addressable_One_Color-EN.png?raw=true "Mkt_Light_Addressable_One_Color-EN")
### Code Example
Example MAKE IT LIGHT UP ADDRESSABLE LIGHTS ONE COLOR using the b.Board
```blocks
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})
```
---
##### [🔙 Back Menu](#leds) 
---
## Make Your Lights Rotate
![Mk_Your_Lights_Rotate-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED3/Mk_Rotate_Your_Lights-EN.png?raw=true "Mk_Your_Lights_Rotate-EN")
### Code Example
Example MAKE YOUR LIGHTS ROTATE using the b.Board
```blocks
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
strip.showRainbow(1, 360)
basic.forever(function () {
strip.rotate(1)
strip.show()
})
```
---
##### [🔙 Back Menu](#leds) 
---
## Make it Blink
![Mkt_Blink-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED4/Mkt_Blink-EN.png?raw=true "Mkt_Blink-EN")
### Code Example
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
---
##### [🔙 Back Menu](#leds) 
---
## Make it Control Lights Sound
![Mkt_Control_Lights_Sound-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED5/Mkt_Control_Lights_Sound-EN.png?raw=true "Mkt_Control_Lights_Sound-EN")
---
##### [🔙 Back Menu](#leds) 
---
