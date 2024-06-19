# Lights:  Make it light a LED

![Mkt_Light_Led-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/2_Lights/Lights5/Mkt_Light_Led-EN.png?raw=true "Mkt_Light_Led-EN!")

![Mkt_Light_Led-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/2_Lights/Lights5/Mkt_Light_Led-EN.png?raw=true "Mkt_Light_Led-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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