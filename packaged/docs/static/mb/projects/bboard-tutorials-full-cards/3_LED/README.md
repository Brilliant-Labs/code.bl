# 📒 b.Board Tutorial Cards / 📒 Cartes de tutoriel b.Board:

# `LEDS`

| English | French |
| ------------------------------- | ------------------------------- | 
| [Make it Light Addressable Rainbow](#make-it-light-addressable-rainbow) | [Faites le allumer des lumieres adressables arcenciel](#faites-le-allumer-des-lumieres-adressables-arcenciel) | 
| [Make it Light Addressable One Color](#make-it-light-addressable-one-color) | [Faites le allumer des lumieres adressables d une couleur](#faites-le-allumer-des-lumieres-adressables-d-une-couleur) |
| [Make it Light Your Lights Rotate](#make-your-lights-rotate) | [Faites tourner vos lumieres](#faites-tourner-vos-lumieres) | 
| [Make it Blink](#make-it-blink)  | [Faites les clignoter](#faites-les-clignoter)  |
| [Make it Control Lights Sound](#make-it-control-lights-sound) | [Faites controler les lumieres avec le son](#faites-controler-les-lumieres-avec-le-son) |
---
---
# `🇬🇧 ENGLISH`
---
## Make it Light Addressable Rainbow
![Mkt_Light_Addressable_Rainbow-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED1/Mkt_Light_Addressable_Rainbow-EN.png?raw=true "Mkt_Light_Addressable_Rainbow-EN")
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
---











# `🇫🇷 FRENCH`
---
## Faites le allumer des lumieres adressables arcenciel
<!-- ![Mkt_Light_Addressable_Rainbow-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED1/Mkt_Light_Addressable_Rainbow-EN.png?raw=true "Mkt_Light_Addressable_Rainbow-EN")-->
![Mkt_Light_Addressable_Rainbow-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED1/Mkt_Light_Addressable_Rainbow-FR.png?raw=true "Mkt_Light_Addressable_Rainbow-FR")

### Exemple de code
Exemple FAIS BRILLER DES LUMIÈRES ARC-EN-CIEL ADRESSABLES avec la b.Board
```blocks
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})
```
---
##### [🔙 Menu Retour](#leds) 
---
## Faites le allumer des lumieres adressables d une couleur
![Mkt_Light_Addressable_One_Color-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED2/Mkt_Light_Addressable_One_Color-FR.png?raw=true "Mkt_Light_Addressable_One_Color-FR")
### Exemple de code
Exemple FAIS BRILLER DES LUMIÈRES ADRESSABLES D’UNE SEULE COULEUR avec la b.Board
```blocks
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
basic.forever(function () {
strip.showColor(neopixel.colors(NeoPixelColors.Red))
})
```
---
##### [🔙 Menu Retour](#leds) 
---
## Faites tourner vos lumieres
![Mk_Your_Lights_Rotate-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED3/Mk_Rotate_Your_Lights-FR.png?raw=true "Mk_Your_Lights_Rotate-FR")
### Exemple de code
Exemple FAIS TOURNER TES LUMIÈRES avec la b.Board
```blocks
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
strip.showRainbow(1, 360)
basic.forever(function () {
strip.rotate(1)
strip.show()
})
```
---
##### [🔙 Menu Retour](#leds) 
---
## Faites les clignoter
![Mkt_Blink-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED4/Mkt_Blink-FR.png?raw=true "Mkt_Blink-FR")
### Exemple de code
Exemple FAIS-LA CLIGNOTER avec la b.Board
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
##### [🔙 Menu Retour](#leds) 
---
## Faites controler les lumieres avec le son
![Mkt_Control_Lights_Sound-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/3_LED/LED5/Mkt_Control_Lights_Sound-FR.png?raw=true "Mkt_Control_Lights_Sound-FR")
---
##### [🔙 Menu Retour](#leds) 

