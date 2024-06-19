# Remote:  CODE A TEMPERATURE REMOTE CONTROL USING RADIO SIGNAL

![Code_Temp_Radio_Ctrl-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/4_Remote/Remote5/Code_Temp_Radio_Ctrl-EN.png?raw=true "Code_Temp_Radio_Ctrl-EN")

![Code_Temp_Radio_Ctrl-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/4_Remote/Remote5/Code_Temp_Radio_Ctrl-EN.png?raw=true "Code_Temp_Radio_Ctrl-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example CODE A TEMPERATURE REMOTE CONTROL USING RADIO SIGNAL using the b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(input.temperature())
})
radio.setGroup(1)

```