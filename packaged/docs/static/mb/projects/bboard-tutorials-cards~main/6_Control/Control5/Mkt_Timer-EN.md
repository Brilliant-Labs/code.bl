# Control MAKE IT A TIMER

![Mkt_Timer-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/6_Control/Control5/Mkt_Timer-EN.png?raw=true "Mkt_Timer-EN")

## Code Example

Example MAKE IT A TIMER using the b.Board

```blocks

let seconds = 0
input.onButtonPressed(Button.A, function () {
if (seconds < 50) {
seconds += 10
basic.showNumber(seconds)
basic.clearScreen()
}
})
input.onButtonPressed(Button.B, function () {
while (seconds > 0) {
basic.showNumber(seconds)
basic.pause(1000)
seconds += 0 - 1
}
})

```