# Control:  USE A,B AND AB BUTTONS

![Use_A-B_buttons-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/6_Control/Control1/Use_A-B_buttons-EN.png?raw=true "Use_A-B_buttons-EN")

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