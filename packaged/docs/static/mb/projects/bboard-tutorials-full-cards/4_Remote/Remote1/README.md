# Remote:  SEND A MESSAGE WITH RADIO SIGNAL

![Send-Radio_Msg-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/4_Remote/Remote1/Send-Radio_Msg-EN.png?raw=true "Send-Radio_Msg-EN")

## Code Example

Example SEND A MESSAGE WITH RADIO SIGNAL using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendString("You are brilliant")
})
radio.setGroup(1)

```