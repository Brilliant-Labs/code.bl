# Remote:  RECEIVING A MESSAGE WITH RADIO SIGNAL

![Receving_Radio_Msg-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/4_Remote/Remote3/Receving_Radio_Msg-EN.png?raw=true "Receving_Radio_Msg-EN")

![Receving_Radio_Msg-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/4_Remote/Remote2/Receving_Radio_Msg-EN.png?raw=true "Receving_Radio_Msg-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example RECEIVING A MESSAGE WITH RADIO SIGNAL using the b.Board

```blocks

radio.onReceivedString(function (receivedString) {
basic.showString(receivedString)
})
radio.setGroup(1)

```