# Remote:  SEND A NUMBER WITH RADIO SIGNAL

![Send_Radio_Num-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/4_Remote/Remote3/Send_Radio_Num-EN.png?raw=true "RSend_Radio_Num-EN")

## Code Example

Example SEND A NUMBER WITH RADIO SIGNAL using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendNumber(0)
})
radio.setGroup(1)

```