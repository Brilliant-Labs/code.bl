# Control:  MAKE IT COUNT

![Mkt_Count-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/6_Control/Control7/Mkt_Count-EN.png?raw=true "Mkt_Count-EN")

## Code Example

Example MAKE IT COUNT using the b.Board

```blocks

let Counting = 0
basic.forever(function () {
Counting += 1
basic.pause(1000)
basic.showString("" + (Counting))
})

```