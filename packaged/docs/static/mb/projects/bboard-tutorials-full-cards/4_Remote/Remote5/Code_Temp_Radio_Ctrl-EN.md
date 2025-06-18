# Remote:  CODE A TEMPERATURE REMOTE CONTROL USING RADIO SIGNAL

![Code_Temp_Radio_Ctrl-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/4_Remote/Remote5/Code_Temp_Radio_Ctrl.png?raw=true "Code_Temp_Radio_Ctrl-EN")

## Code Example

Example CODE A TEMPERATURE REMOTE CONTROL USING RADIO SIGNAL using the b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(input.temperature())
})
radio.setGroup(1)

```