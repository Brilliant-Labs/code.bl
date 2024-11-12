# Lights:  Make it light a LED

![Mkt_Light_Led-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/2_Lights/Lights5/Mkt_Light_Led-EN.png?raw=true "Mkt_Light_Led-EN!")

## Code Example

Example Make it light a LED using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
pins.digitalWritePin(DigitalPin.P0, 1)
})
input.onButtonPressed(Button.B, function () {
pins.digitalWritePin(DigitalPin.P0, 0)
})

```