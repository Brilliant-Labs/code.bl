# Sound:  MAKE IT LISTEN

![Mkt_Listen-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/7_Sound/Sound1/Mkt_Listen-EN.png?raw=true "Mkt_Listen-EN")

![Mkt_Listen-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/7_Sound/Sound1/Mkt_Listen-EN.png?raw=true "Mkt_Listen-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT LISTEN using the b.Board

```blocks

basic.forever(function () {
basic.showIcon(IconNames.Happy)
})
bBoard_Mic.onMicThresh(bBoard_Mic.soundLevel.loud, function () {
basic.showIcon(IconNames.Surprised)
})

```