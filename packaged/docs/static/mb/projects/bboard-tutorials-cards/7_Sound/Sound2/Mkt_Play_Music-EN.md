# Sound:  MAKE IT PLAY MUSIC

![Mkt_Play_Music-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/7_Sound/Sound2/Mkt_Play_Music-EN.png?raw=true "Mkt_Play_Music-EN")

![Mkt_Play_Music-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/7_Sound/Sound2/Mkt_Play_Music-EN.png?raw=true "Mkt_Play_Music-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

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