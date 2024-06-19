# Control:  MAKE IT KEEP SCORE

Mkt_Keep_Score_Icon-FR


![Mkt_Keep_Score-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/6_Control/Control3/Mkt_Keep_Score-EN.png?raw=true "Mkt_Keep_Score-EN")

![Mkt_Keep_Score-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/6_Control/Control3/Mkt_Keep_Score-EN.png?raw=true "Mkt_Keep_Score-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT KEEP SCORE using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
Score += 1
})
input.onButtonPressed(Button.AB, function () {
Score = 0
})
input.onButtonPressed(Button.B, function () {
Score += -1
})
let Score = 0
Score = 0
basic.forever(function () {
basic.showNumber(Score)
})

```