# Move:  MAKE IT ROLL USING A BUTTON REMOTE CONTROL remote code

![Mkt_Button_RC-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/5_Move/Move4/Mkt_Button_RC-EN.png?raw=true "Mkt_Button_RC-EN")

## Code Example

Example MAKE IT ROLL USING A BUTTON REMOTE CONTROL remote code using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendNumber(1)
})
input.onButtonPressed(Button.AB, function () {
radio.sendNumber(2)
})
input.onButtonPressed(Button.B, function () {
radio.sendNumber(3)
})
radio.setGroup(1)

```