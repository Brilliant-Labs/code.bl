# Control:  MAKE IT A STOPWATCH

![Mkt_Stopwatch-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/6_Control/Control6/Mkt_Stopwatch-EN.png?raw=true "Mkt_Stopwatch-ENN")

## Code Example

Example MAKE IT A STOPWATCH using the b.Board

```blocks

let secondes = 0
input.onButtonPressed(Button.A, function () {
if (secondes < 50) {
secondes += 10
basic.showNumber(secondes)
basic.clearScreen()
}
})
input.onButtonPressed(Button.B, function () {
while (secondes > 0) {
basic.showNumber(secondes)
basic.pause(1000)
secondes += 0 - 1
}
})

```