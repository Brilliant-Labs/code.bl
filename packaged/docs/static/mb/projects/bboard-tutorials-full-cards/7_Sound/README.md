# 📒 b.Board Tutorial Cards / 📒 Cartes de tutoriel b.Board:

# `SOUND-SON`

| English | French |
| ------------------------------- | ------------------------------- | 
| [Make it Listen](#make-it-listen) | [Le faire ecouter](#le-faire-ecouter) | 
| [Make it Play Music](#make-it-play-music) | [Faire jouer de la musique](#faire-jouer-de-la-musique) |
| [Make it Talk](#make-it-talk) | [le faire parler](#le-faire-parler) |
| [Make it Alarm](#make-it-alarm) | [Faire de l alarme](#faire-de-l-alarme) | 
---
---
# `🇬🇧 ENGLISH`
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
##### 🔙 [Back Menu](#sound-son) 
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
##### 🔙 [Back Menu](#sound-son) 
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
##### 🔙 [Back Menu](#sound-son) 
---
## Make it Alarm
![Mk_Alarm-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound4/Mk_Alarm-EN.png?raw=true "Mk_Alarm-EN")
---
##### 🔙 [Back Menu](#sound-son) 
---
---







# `🇫🇷 FRENCH`
---
---
## Le faire ecouter
![Mkt_Listen-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound1/Mkt_Listen-FR.png?raw=true "Mkt_Listen-FR")

## Exemple de code

Exemple FAIS-LE ÉCOUTER avec la b.Board

```blocks

basic.forever(function () {
basic.showIcon(IconNames.Happy)
})
bBoard_Mic.onMicThresh(bBoard_Mic.soundLevel.loud, function () {
basic.showIcon(IconNames.Surprised)
})

```
---
##### 🔙 [Menu Retour](#sound-son) 
---
## Faire jouer de la musique
![Mkt_Play_Music-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound2/Mkt_Play_Music-FR.png?raw=true "Mkt_Play_Music-FR")

## Exemple de code

Exemple FAIS-LE JOUER DE LA MUSIQUE avec la b.Board

```blocks

music.playMelody("C5 B A G F E D C ", 293)
for (let index = 0; index < 4; index++) {
music.playTone(262, music.beat(BeatFraction.Whole))
music.rest(music.beat(BeatFraction.Whole))
music.playTone(392, music.beat(BeatFraction.Eighth))
}

```
---
##### 🔙 [Menu Retour](#sound-son) 
---
## Le faire parler
![Mkt_Talk-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound3/Mkt_Talk-FR.png?raw=true "Mkt_Talk-FR")

## Exemple de code

Exemple FAIS-LE PARLER avec la b.Board

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
##### 🔙 [Menu Retour](#sound-son) 
---
## Faire de l alarme
![Mk_Alarm-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/7_Sound/Sound4/Mk_Alarm-FR.png?raw=true "Mk_Alarm-FR")
---
##### 🔙 [Menu Retour](#sound-son) 