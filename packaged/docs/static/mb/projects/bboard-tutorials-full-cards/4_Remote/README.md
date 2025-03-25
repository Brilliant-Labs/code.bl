# 📒 b.Board Tutorial Cards:

# `REMOTE`

- [Sending Radio Msg](#sending-radio-msg) 
- [Receving Radio Msg](#receving-radio-msg) 
- [Sending Radio Num](#sending-radio-num) 
- [Receiving Radio Num](#receiving-radio-num) 
- [Code Temp Radio Ctrl](#code-temp-radio-ctrl)

---
## Sending Radio Msg
![Send-Radio_Msg-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote1/Send-Radio_Msg-EN.png?raw=true "Send-Radio_Msg-EN")
### Code Example
Example SEND A MESSAGE WITH RADIO SIGNAL using the b.Board
```blocks
input.onButtonPressed(Button.A, function () {
radio.sendString("You are brilliant")
})
radio.setGroup(1)
```
---
##### 🔙 [Back Menu](#remote) 
---
## Receving Radio Msg
![Receving_Radio_Msg-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote2/Receving_Radio_Msg-EN.png?raw=true "Receving_Radio_Msg-EN")
### Code Example
Example RECEIVING A MESSAGE WITH RADIO SIGNAL using the b.Board
```blocks
radio.onReceivedString(function (receivedString) {
basic.showString(receivedString)
})
radio.setGroup(1)
```
---
##### 🔙 [Back Menu](#remote) 
---
## Sending Radio Num
![Send_Radio_Num-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote3/Send_Radio_Num-EN.png?raw=true "RSend_Radio_Num-EN")
### Code Example
Example SEND A NUMBER WITH RADIO SIGNAL using the b.Board
```blocks
input.onButtonPressed(Button.A, function () {
radio.sendNumber(0)
})
radio.setGroup(1)
```
---
##### 🔙 [Back Menu](#remote) 
---
## Receiving Radio Num
![Receiving_Radio_Num-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote4/Receiving_Radio_Num-EN.png?raw=true "Receiving_Radio_Num-EN")
### Code Example
Example RECEIVE A NUMBER VALUE WITH RADIO SIGNAL using the b.Board
```blocks
radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(receivedNumber)
})
radio.setGroup(1)
```
---
##### 🔙 [Back Menu](#remote) 
---
## Code Temp Radio Ctrl
![Code_Temp_Radio_Ctrl](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote5/Code_Temp_Radio_Ctrl-EN.png?raw=true "Code Temperature Radio Control")
### Code Example
Example CODE A TEMPERATURE REMOTE CONTROL USING RADIO SIGNAL using the b.Board
```blocks
radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(input.temperature())
})
radio.setGroup(1)
```
---
##### 🔙 [Back Menu](#remote) 
---
