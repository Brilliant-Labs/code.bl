# Remote:  RECEIVE A NUMBER VALUE WITH RADIO SIGNAL

![Receiving_Radio_Num-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/4_Remote/Remote4/Receiving_Radio_Num-EN.png?raw=true "Receiving_Radio_Num-EN")

## Code Example

Example RECEIVE A NUMBER VALUE WITH RADIO SIGNAL using the b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(receivedNumber)
})
radio.setGroup(1)

```