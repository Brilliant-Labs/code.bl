# Remote:  SEND A MESSAGE WITH RADIO SIGNAL

![Send-Radio_Msg-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/4_Remote/Remote1/Send-Radio_Msg-EN.png?raw=true "Send-Radio_Msg-EN")

![Send-Radio_Msg-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/4_Remote/Remote1/Send-Radio_Msg-EN.png?raw=true "Send-Radio_Msg-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example SEND A MESSAGE WITH RADIO SIGNAL using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendString("You are brilliant")
})
radio.setGroup(1)

```