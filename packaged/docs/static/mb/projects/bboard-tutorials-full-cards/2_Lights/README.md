# 📒 b.Board Tutorial Cards:

# `LIGHTS`

- [Make it Light Up](#make-it-light-up) 
- [Make it Light Different Colors](#make-it-light-different-colors) 
- [Make it Light Up Different Colors Using a Button](#make-it-light-up-different-colors-using-a-button) 
- [Add Your Name Screen](#add-your-name-screen) 
- [Make it Light a LED](#make-it-light-a-led)
- [Make a Night Light ](#make-a-night-light)
- [Light Up Dark](#light-up-dark)
---
## Make it Light Up
![Mkt_Light_UP-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights1/Mkt_Light_UP-EN.png?raw=true "MAKE IT LIGHT UP!")
### Code Example
Example MAKE IT LIGHT UP! using the b.Board
```blocks
basic.forever(function () {
BLiXel.showColour(0xff9da5)
})
```
---
##### [🔙 Back Menu](#lights) 
---
## Make it Light Different Colors
![Mkt_Light-Up_Diff_Color-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights2/Mkt_Light-Up_Diff_Color-EN.png?raw=true "Mkt_Light-Up_Diff_Color-EN!")
### Code Example
Example MAKE IT LIGHT UP different COLORS ! using the b.Board
```blocks
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.one), 0xffff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.two), 0x00ff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.three), 0xffffff)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.four), 0xff0000)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.five), 0x007fff)
```
---
##### [🔙 Back Menu](#lights) 
---
## Make it Light Up Different Colors Using a Button

![Mkt_Light-Up_Diff_Color_Button-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights3/Mkt_Light-Up_Diff_Color_Button-EN.png?raw=true "Mkt_Light-Up_Diff_Color_Button-EN!")
### Code Example
Example MAKE IT LIGHT UP different COLORS using a button ! using the b.Board
```blocks
input.onButtonPressed(Button.A, function () {
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.one), 0xffff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.two), 0x00ff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.three), 0xffffff)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.four), 0xff0000)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.five), 0x007fff)
})
```
---
##### [🔙 Back Menu](#lights) 
---
## Add Your Name Screen
![Add_Your_Name_Screen-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights4/Add_Your_Name_Screen-EN.png?raw=true "Add_Your_Name_Screen-EN!")
### Code Example
Example ADD YOUR NAME TO THE LED SCREEN! using the b.Board
```blocks
basic.forever(function () {
basic.showString("Bob")
})
```
---
##### [🔙 Back Menu](#lights) 
---
## Make it light a LED
![Mkt_Light_Led-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights5/Mkt_Light_Led-EN.png?raw=true "Mkt_Light_Led-EN!")
### Code Example
Example Make it light a LED using the b.Board
```blocks
input.onButtonPressed(Button.A, function () {
pins.digitalWritePin(DigitalPin.P0, 1)
})
input.onButtonPressed(Button.B, function () {
pins.digitalWritePin(DigitalPin.P0, 0)
})
```
---
##### [🔙 Back Menu](#lights) 
---
## Make a Night Light 
![Mkt_Night_Light-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights6/Mkt_Night_Light-EN.png?raw=true "Mkt_Night_Light-EN")
---
##### [🔙 Back Menu](#lights) 
---
## Light Up Dark
![Light_Up_Dark-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights7/Light_Up_Dark-EN.png?raw=true "Light_Up_Dark-EN")
## Code Example
Example   LIGHT UP WHEN ITS DARK using the b.Board
```blocks
basic.forever(function () {
BLiXel.showColour(0x000000)
while (input.lightLevel() < 50) {
BLiXel.showColour(0xffffff)
}
})
```
---
##### [🔙 Back Menu](#lights) 
---
