# Lights:  LIGHT UP WHEN ITS DARK

![Light_Up_Dark-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/2_Lights/Lights7/Light_Up_Dark-EN.png?raw=true "Light_Up_Dark-EN")

![Light_Up_Dark-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/2_Lights/Lights7/Light_Up_Dark-EN.png?raw=true "Light_Up_Dark-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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