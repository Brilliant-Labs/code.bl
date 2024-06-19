# Lights:  LIGHT UP WHEN ITS DARK

![Light_Up_Dark-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/2_Lights/Lights7/Light_Up_Dark-EN.png?raw=true "Light_Up_Dark-EN")

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