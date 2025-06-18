# 📒 b.Board Tutorial Cards:

# `SOUND`

- [Make it Listen](#make-it-listen) 
- [Make it Play Music](#make-it-play-music) 
- [Make it Talk](#make-it-talk) 
- [Make it Alarm](#make-it-alarm) 
---
## Make it Listen
![Mkt_Listen-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound1/Mkt_Listen-EN.png?raw=true "Mkt_Listen-EN")

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
---
##### 🔙 [Back Menu](#sound) 
---
## Make it Play Music
![Mkt_Play_Music-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound2/Mkt_Play_Music-EN.png?raw=true "Mkt_Play_Music-EN")

## Code Example

Example MAKE IT PLAY MUSIC using the b.Board

```blocks

music.playMelody("C5 B A G F E D C ", 293)
for (let index = 0; index < 4; index++) {
music.playTone(262, music.beat(BeatFraction.Whole))
music.rest(music.beat(BeatFraction.Whole))
music.playTone(392, music.beat(BeatFraction.Eighth))
}

```
---
##### 🔙 [Back Menu](#sound) 
---
## Make it Talk
![Mkt_Talk-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound3/Mkt_Talk-EN.png?raw=true "Mkt_Talk-EN")

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
---
##### 🔙 [Back Menu](#sound) 
---
## Make it Alarm
![Mk_Alarm-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound4/Mk_Alarm-EN.png?raw=true "Mk_Alarm-EN")
---
##### 🔙 [Back Menu](#sound) 
---