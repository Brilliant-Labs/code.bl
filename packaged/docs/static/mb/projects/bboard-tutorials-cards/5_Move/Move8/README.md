# Move:  MAKE IT REACT TO MOVEMENT

![Mkt_React_Movement-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/5_Move/Move8/Mkt_React_Movement-EN.png?raw=true "Mkt_React_Movement-EN")

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