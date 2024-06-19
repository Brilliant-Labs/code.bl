# Move:  MAKE IT ROLL USING A BUTTON REMOTE CONTROL remote code

![Mkt_Button_RC-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/5_Move/Move4/Mkt_Button_RC-EN.png?raw=true "Mkt_Button_RC-EN")

![Mkt_Button_RC-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/5_Move/Move4/Mkt_Button_RC-EN.png?raw=true "Mkt_Button_RC-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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