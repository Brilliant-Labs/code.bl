# Control:  MAKE IT COUNT

![Mkt_Count-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/6_Control/Control7/Mkt_Count-EN.png?raw=true "Mkt_Count-EN")

![Mkt_Count-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/6_Control/Control7/Mkt_Count-EN.png?raw=true "Mkt_Count-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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