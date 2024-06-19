# Remote:  RECEIVE A NUMBER VALUE WITH RADIO SIGNAL

![Receiving_Radio_Num-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/4_Remote/Remote4/Receiving_Radio_Num-EN.png?raw=true "Receiving_Radio_Num-EN")

![Receiving_Radio_Num-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/4_Remote/Remote4/Receiving_Radio_Num-EN.png?raw=true "Receiving_Radio_Num-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example RECEIVE A NUMBER VALUE WITH RADIO SIGNAL using the b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(receivedNumber)
})
radio.setGroup(1)

```