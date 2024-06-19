# Sound:  MAKE IT TALK

![Mkt_Talk-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/7_Sound/Sound3/Mkt_Talk-EN.png?raw=true "Mkt_Talk-EN")

![Mkt_Talk-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/7_Sound/Sound3/Mkt_Talk-EN.png?raw=true "Mkt_Talk-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT TALK using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
MP3.playSong(MP3_2.mp3FileNumbers.one)
})
input.onButtonPressed(Button.B, function () {
MP3.pause()
})
let MP3: MP3_2.KT403A = null
MP3 = MP3_2.createMP3Click(BoardID.zero, ClickID.A)

```