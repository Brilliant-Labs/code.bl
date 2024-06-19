# Move:  MAKE IT REACT TO MOVEMENT

![Mkt_React_Movement-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/5_Move/Move7/Mkt_React_Movement-EN.png?raw=true "Mkt_React_Movement-EN")

![Mkt_React_Movement-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/5_Move/Move8/Mkt_React_Movement-EN.png?raw=true "Mkt_React_Movement-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT REACT TO MOVEMENT using the b.Board

```blocks

input.onGesture(Gesture.Shake, function () {
for (let index = 0; index < 4; index++) {
BLiXel.showColour(0xff0000)
basic.pause(500)
BLiXel.showColour(0x000000)
basic.pause(500)
}
})

```