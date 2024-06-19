# Move:  MAKE AN INTRUDER ALERT

![Mk_Intruder_Alert-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/5_Move/Move7/Mk_Intruder_Alert-EN.png?raw=true "Mk_Intruder_Alert-EN")

## Code Example

Example MAKE AN INTRUDER ALERT using the b.Board

```blocks

let Motion2 = Motion.createMotion(BoardID.zero, ClickID.A)
Motion2.onMotionDetected(function () {
for (let index = 0; index < 4; index++) {
music.playTone(262, music.beat(BeatFraction.Whole))
BLiXel.showColour(0xff0000)
}
})

```