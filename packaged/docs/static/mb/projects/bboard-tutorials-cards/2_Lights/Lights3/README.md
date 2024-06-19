# Lights:  MAKE IT LIGHT UP different COLORS using a button !

![Mkt_Light-Up_Diff_Color_Button-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/2_Lights/Lights3/Mkt_Light-Up_Diff_Color_Button-EN.png?raw=true "Mkt_Light-Up_Diff_Color_Button-EN!")

![Mkt_Light-Up_Diff_Color_Button-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/2_Lights/Lights3/Mkt_Light-Up_Diff_Color_Button-EN?raw=true "Mkt_Light-Up_Diff_Color_Button-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

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