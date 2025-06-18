# 📒 b.Board Tutorial Cards / 📒 Cartes de tutoriel b.Board:

# `REMOTE-TELECOMMANDE`

| English | French |
| ------------------------------- | ------------------------------- | 
| [Sending Radio Msg](#sending-radio-msg) | [Envoyer un message avec le signal radio](#envoyer-un-message-avec-le-signal-radio) | 
| [Receving Radio Msg](#receving-radio-msg) | [Recevoir un message par signal radio](#recevoir-un-message-par-signal-radio) |
| [Sending Radio Num](#sending-radio-num) | [Envoyer une valeur nombre avec le signal radio](#envoyer-une-valeur-nombre-avec-le-signal-radio) | 
| [Receiving Radio Num](#receiving-radio-num) | [Recevoir une valeur nombre avec la radio](#recevoir-une-valeur-nombre-avec-la-radio)  |
| [Code Temp Radio Ctrl](#code-temp-radio-ctrl) | [Codez un thermometre telecommande](#codez-un-thermometre-telecommande) |
---
---
# `🇬🇧 ENGLISH`
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
##### 🔙 [Back Menu](#remote-telecommande) 
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
##### 🔙 [Back Menu](#remote-telecommande) 
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
##### 🔙 [Back Menu](#remote-telecommande) 
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
##### 🔙 [Back Menu](#remote-telecommande) 
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
##### 🔙 [Back Menu](#remote-telecommande) 





















---
---
# `🇫🇷 FRENCH`
---
## Envoyer un message avec le signal radio
![Send-Radio_Msg-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote1/Send-Radio_Msg-FR.png?raw=true "Send-Radio_Msg-FR")
### Exemple de code
Exemple ENVOIE UN MESSAGE AVEC UN SIGNAL RADIO avec la b.Board
```blocks
input.onButtonPressed(Button.A, function () {
radio.sendString("You are brilliant")
})
radio.setGroup(1)
```
---
##### 🔙 [Menu Retour](#remote-telecommande) 
---
## Recevoir un message par signal radio
![Receving_Radio_Msg-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote2/Receving_Radio_Msg-FR.png?raw=true "Receving_Radio_Msg-FR")
### Exemple de code
Exemple RÉCEPTIONNE UN MESSAGE AVEC UN SIGNAL RADIO avec la b.Board
```blocks
radio.onReceivedString(function (receivedString) {
basic.showString(receivedString)
})
radio.setGroup(1)
```
---
##### 🔙 [Menu Retour](#remote-telecommande) 
---
## Envoyer une valeur nombre avec le signal radio
![Send_Radio_Num-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote3/Send_Radio_Num-FR.png?raw=true "RSend_Radio_Num-FR")
### Exemple de code
Exemple ENVOIE UN NOMBRE AVEC UN SIGNAL RADIO avec la b.Board
```blocks
input.onButtonPressed(Button.A, function () {
radio.sendNumber(0)
})
radio.setGroup(1)
```
---
##### 🔙 [Menu Retour](#remote-telecommande) 
---
## Recevoir une valeur nombre avec la radio
![Receiving_Radio_Num-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote4/Receiving_Radio_Num-FR.png?raw=true "Receiving_Radio_Num-FR")
### Exemple de code
Exemple REÇOIS UNE VALEUR NUMÉRIQUE AVEC UN SIGNAL RADIO avec la b.Board
```blocks
radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(receivedNumber)
})
radio.setGroup(1)
```
---
##### 🔙 [Menu Retour](#remote-telecommande) 
---
## Codez un thermometre telecommande
![Code_Temp_Radio_Ctrl](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/4_Remote/Remote5/Code_Temp_Radio_Ctrl-FR.png?raw=true "Code Temperature Radio Control")
### Exemple de code
Exemple CODE UNE TÉLÉCOMMANDE DE TEMPÉRATURE UTILISANT UN SIGNAL RADIO avec la b.Board
```blocks
radio.onReceivedNumber(function (receivedNumber) {
basic.showNumber(input.temperature())
})
radio.setGroup(1)
```
---
##### 🔙 [Menu Retour](#remote-telecommande) 