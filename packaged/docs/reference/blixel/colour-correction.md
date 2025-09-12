# BLiXel Colour Correction

Some BLiXel LEDs on certain b.Board devices have their colours mixed up by the manufacturer.  
This block fixes the issue so that **red, green, and blue** display correctly.

## How to use

1. Drag the **BLiXel colour correction** block into your program.
2. Place it inside `on start` so that the fix is applied as soon as your program begins.
3. After that, all BLiXel colours will display correctly.

## Example

```blocks
input.onButtonPressed(Button.A, function () {
    BLiXel.showColour(0xff0000)
})
BLiXel.blixelColourCorrection()
basic.forever(function () {
	
})
```