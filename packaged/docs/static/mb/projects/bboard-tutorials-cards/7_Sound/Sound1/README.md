# Sound:  MAKE IT LISTEN

![Mkt_Listen-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/7_Sound/Sound1/Mkt_Listen-EN.png?raw=true "Mkt_Listen-EN")

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