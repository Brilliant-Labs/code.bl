# Remote:  SEND A NUMBER WITH RADIO SIGNAL

![Send_Radio_Num-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/4_Remote/Remote3/Send_Radio_Num-EN.png?raw=true "RSend_Radio_Num-EN")

![Send_Radio_Num-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/4_Remote/Remote3/Send_Radio_Num-EN.png?raw=true "Send_Radio_Num-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example SEND A NUMBER WITH RADIO SIGNAL using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendNumber(0)
})
radio.setGroup(1)

```