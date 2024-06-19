# Control:  USE A,B AND AB BUTTONS

![Use_A-B_buttons-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/6_Control/Control1/Use_A-B_buttons-EN.png?raw=true "Use_A-B_buttons-EN")

![Use_A-B_buttons-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/6_Control/Control1/Use_A-B_buttons-EN.png?raw=true "Use_A-B_buttons-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example USE A,B AND AB BUTTONS using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
basic.showIcon(IconNames.Heart)
})
input.onButtonPressed(Button.B, function () {
basic.showIcon(IconNames.Yes)
})

```