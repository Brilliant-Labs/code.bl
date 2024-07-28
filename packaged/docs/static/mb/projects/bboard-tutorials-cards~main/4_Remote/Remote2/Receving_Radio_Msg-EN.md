# Remote:  RECEIVING A MESSAGE WITH RADIO SIGNAL

![Receving_Radio_Msg-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/4_Remote/Remote2/Receving_Radio_Msg-EN.png?raw=true "Receving_Radio_Msg-EN")

## Code Example

Example RECEIVING A MESSAGE WITH RADIO SIGNAL using the b.Board

```blocks

radio.onReceivedString(function (receivedString) {
basic.showString(receivedString)
})
radio.setGroup(1)

```