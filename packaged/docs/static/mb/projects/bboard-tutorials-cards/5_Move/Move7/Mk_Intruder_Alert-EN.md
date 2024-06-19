# Move:  MAKE AN INTRUDER ALERT

![Mk_Intruder_Alert-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/5_Move/Move7/Mk_Intruder_Alert-EN.png?raw=true "Mk_Intruder_Alert-EN")

![Mk_Intruder_Alert-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/5_Move/Move7/Mk_Intruder_Alert-EN.png?raw=true "Mk_Intruder_Alert-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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