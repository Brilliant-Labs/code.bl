# 📒 b.Board Tutorial Cards / 📒 Cartes de tutoriel b.Board:

# `MOVE-DEPLACER`

| English | French |
| ------------------------------- | ------------------------------- | 
| [Adding Motors](#adding-motors) | [Ajout de moteurs cd](#ajout-de-moteurs-cd) | 
| [Make it Roll Tilt Remote Code](#make-it-roll-tilt-remote-code) | [Faites le rouler avec une manette inclinable code de la manette](#faites-le-rouler-avec-une-manette-inclinable-code-de-la-manette) |
| [Make it Roll Vehicule Code](#make-it-roll-vehicule-code) | [Faites le rouler a laide d une telecommande](#faites-le-rouler-a-laide-d-une-telecommande) |
| [Make it Button RC](#make-it-button-rc) | [Faites le rouler a laide d une telecommande a bouton](#faites-le-rouler-a-laide-d-une-telecommande-a-bouton) | 
| [Make it Roll](#make-it-roll) | [Faites le rouler](#faites-le-rouler) |
| [Make it Turn Servo](#make-it-turn-servo) | [Faites tourner](#faites-tourner) |
| [Make it Intruder Alert](#make-it-intruder-alert) | [Faire une alerte intrus](#faire-une-alerte-intrus) |
| [Make it React Movement](#make-it-react-movement) | [Faites le reagir au mouvement](#faites-le-reagir-au-mouvement) |
---
---
# `🇬🇧 ENGLISH`
---
## Adding Motors
![Adding_motors-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move1/Adding_motors-EN.png?raw=true "Adding_motors-EN")

---
##### 🔙 [Back Menu](#move-deplacer) 
---
---
## Make it Roll Tilt Remote Code
![Mkt_Roll_Tilt_Remote_Code-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move2/Mkt_Roll_Tilt_Remote_Code-EN.png?raw=true "Mkt_Roll_Tilt_Remote_Code-EN")

## Code Example

Example MAKE IT ROLL USING A TILT REMOTE - remote code using the b.Board

```blocks

input.onGesture(Gesture.LogoUp, function () {
radio.sendNumber(1)
})
input.onGesture(Gesture.TiltLeft, function () {
radio.sendNumber(3)
})
input.onGesture(Gesture.TiltRight, function () {
radio.sendNumber(4)
})
input.onGesture(Gesture.LogoDown, function () {
radio.sendNumber(2)
})
radio.setGroup(1)

```
---
##### 🔙 [Back Menu](#move-deplacer) 
---
---
## Make it Roll Vehicule Code
![Mkt_Roll_Vehicule_Code-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move3/Mkt_Roll_Vehicule_Code-EN.png?raw=true "AMkt_Roll_Vehicule_Code-EN")

## Code Example

Example MAKE IT ROLL USING A REMOTE vehicule code using the b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
if (receivedNumber == 1) {
bBoard_Motor.motorLeftDuty(50)
bBoard_Motor.motorRightDuty(100)
} else if (receivedNumber == 2) {
bBoard_Motor.motorLeftDuty(100)
bBoard_Motor.motorRightDuty(50)
} else if (receivedNumber == 3) {
bBoard_Motor.motorDuty(100)
} else if (receivedNumber == 4) {
bBoard_Motor.motorDuty(-100)
} else {

}
})
radio.setGroup(1)

```
---
##### 🔙 [Back Menu](#move-deplacer) 
---
---
## Make it Button RC
![Mkt_Button_RC-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move4/Mkt_Button_RC-EN.png?raw=true "Mkt_Button_RC-EN")

## Code Example

Example MAKE IT ROLL USING A BUTTON REMOTE CONTROL remote code using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendNumber(1)
})
input.onButtonPressed(Button.AB, function () {
radio.sendNumber(2)
})
input.onButtonPressed(Button.B, function () {
radio.sendNumber(3)
})
radio.setGroup(1)

```
---
##### 🔙 [Back Menu](#move-deplacer) 
---
---
## Make it Roll
![Mkt_Roll-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move5/Mkt_Roll-EN.png?raw=true "Mkt_Roll-EN")

## Code Example

Example MAKE IT ROLL FOR LIMITED AMOUNTS OF TIME! using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorLeftTimed(100, 5000)
})
input.onButtonPressed(Button.AB, function () {
bBoard_Motor.motorTimed(100, 5000)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorRightTimed(100, 5000)
})

```
---
##### 🔙 [Back Menu](#move-deplacer) 
---
---
## Make it Turn Servo
![Mkt_Turn_Servo-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move6/Mkt_Turn_Servo-EN.png?raw=true "Mkt_Turn_Servo-EN")

## Code Example
 
ExampleMAKE IT TURN! using the b.Board

```blocks

basic.forever(function () {
for (let index = 0; index < 4; index++) {
pins.servoWritePin(AnalogPin.P0, 0)
basic.pause(1000)
pins.servoWritePin(AnalogPin.P0, 45)
basic.pause(1000)
pins.servoWritePin(AnalogPin.P0, 0)
basic.pause(1000)
}
})

```
---
##### 🔙 [Back Menu](#move-deplacer) 
---
---
## Make it Intruder Alert
![Mk_Intruder_Alert-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move7/Mk_Intruder_Alert-EN.png?raw=true "Mk_Intruder_Alert-EN")

## Code Example

Example MAKE AN INTRUDER ALERT using the b.Board

```blocks

let Motion2 = Motion.createMotion(BoardID.zero, ClickID.A)
Motion2.onMotionDetected(function () {
for (let index = 0; index < 4; index++) {
music.playTone(262, music.beat(BeatFraction.Whole))
BLiXel.showColour(0xff0000)
}
})

```
---
##### 🔙 [Back Menu](#move-deplacer) 
---
---
## Make it React Movement
![Mkt_React_Movement-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move8/Mkt_React_Movement-EN.png?raw=true "Mkt_React_Movement-EN")

## Code Example

Example MAKE IT REACT TO MOVEMENT using the b.Board

```blocks

input.onGesture(Gesture.Shake, function () {
for (let index = 0; index < 4; index++) {
BLiXel.showColour(0xff0000)
basic.pause(500)
BLiXel.showColour(0x000000)
basic.pause(500)
}
})

```
---
##### 🔙 [Back Menu](#move-deplacer) 












---
---
# `🇫🇷 FRENCH`
---
---
## Ajout de moteurs cd
![Adding_motors-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move1/Adding_motors-FR.png?raw=true "Adding_motors-FR")

---
##### 🔙 [Menu Retour](#move-deplacer) 
---
---
## Faites le rouler avec une manette inclinable code de la manette
![Mkt_Roll_Tilt_Remote_Code-FR](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move2/Mkt_Roll_Tilt_Remote_Code-FR.png?raw=true "Mkt_Roll_Tilt_Remote_Code-FR")

## Exemple de code
Exemple FAIS-LA ROULER EN UTILISANT UNE TÉLÉCOMMANDE À INCLINAISON – code de télécommande avec la b.Board

```blocks

input.onGesture(Gesture.LogoUp, function () {
radio.sendNumber(1)
})
input.onGesture(Gesture.TiltLeft, function () {
radio.sendNumber(3)
})
input.onGesture(Gesture.TiltRight, function () {
radio.sendNumber(4)
})
input.onGesture(Gesture.LogoDown, function () {
radio.sendNumber(2)
})
radio.setGroup(1)

```
---
##### 🔙 [Menu Retour](#move-deplacer) 
---
---
## Faites le rouler a laide d une telecommande
![Mkt_Roll_Vehicule_Code-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move3/Mkt_Roll_Vehicule_Code-FR.png?raw=true "AMkt_Roll_Vehicule_Code-FR")

## Exemple de code

Exemple FAIS-LA ROULER EN UTILISANT UNE TÉLÉCOMMANDE – code de véhicule avec la b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
if (receivedNumber == 1) {
bBoard_Motor.motorLeftDuty(50)
bBoard_Motor.motorRightDuty(100)
} else if (receivedNumber == 2) {
bBoard_Motor.motorLeftDuty(100)
bBoard_Motor.motorRightDuty(50)
} else if (receivedNumber == 3) {
bBoard_Motor.motorDuty(100)
} else if (receivedNumber == 4) {
bBoard_Motor.motorDuty(-100)
} else {

}
})
radio.setGroup(1)

```
---
##### 🔙 [Menu Retour](#move-deplacer) 
---
---
## Faites le rouler a laide d une telecommande a bouton
![Mkt_Button_RC-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move4/Mkt_Button_RC-FR.png?raw=true "Mkt_Button_RC-FR")

## Exemple de code

Exemple FAIS-LA ROULER EN UTILISANT UNE TÉLÉCOMMANDE À BOUTONS – code de télécommande avec la b.Board

```blocks

input.onButtonPressed(Button.A, function () {
radio.sendNumber(1)
})
input.onButtonPressed(Button.AB, function () {
radio.sendNumber(2)
})
input.onButtonPressed(Button.B, function () {
radio.sendNumber(3)
})
radio.setGroup(1)

```
---
##### 🔙 [Menu Retour](#move-deplacer) 
---
---
## Faites le rouler
![Mkt_Roll-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move5/Mkt_Roll-FR.png?raw=true "Mkt_Roll-FR")

## Exemple de code

Exemple FAIS-LA ROULER PENDANT UNE DURÉE LIMITÉE ! avec la b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorLeftTimed(100, 5000)
})
input.onButtonPressed(Button.AB, function () {
bBoard_Motor.motorTimed(100, 5000)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorRightTimed(100, 5000)
})

```
---
##### 🔙 [Menu Retour](#move-deplacer) 
---
---
## Faites tourner
![Mkt_Turn_Servo-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move6/Mkt_Turn_Servo-FR.png?raw=true "Mkt_Turn_Servo-FR")

## Exemple de code

Exemple FAIS-LA TOURNER ! avec la b.Board

```blocks

basic.forever(function () {
for (let index = 0; index < 4; index++) {
pins.servoWritePin(AnalogPin.P0, 0)
basic.pause(1000)
pins.servoWritePin(AnalogPin.P0, 45)
basic.pause(1000)
pins.servoWritePin(AnalogPin.P0, 0)
basic.pause(1000)
}
})

```
---
##### 🔙 [Menu Retour](#move-deplacer) 
---
---
## Faire une alerte intrus
![Mk_Intruder_Alert-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl//code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move7/Mk_Intruder_Alert-FR.png?raw=true "Mk_Intruder_Alert-FR")

## Exemple de code

Exemple CRÉE UNE ALERTE D’INTRUS avec la b.Board

```blocks

let Motion2 = Motion.createMotion(BoardID.zero, ClickID.A)
Motion2.onMotionDetected(function () {
for (let index = 0; index < 4; index++) {
music.playTone(262, music.beat(BeatFraction.Whole))
BLiXel.showColour(0xff0000)
}
})

```
---
##### 🔙 [Menu Retour](#move-deplacer) 
---
---
## Faites le reagir au mouvement
![Mkt_React_Movement-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/5_Move/Move8/Mkt_React_Movement-FR.png?raw=true "Mkt_React_Movement-FR")

## Exemple de code

Exemple FAIS-LA RÉAGIR AU MOUVEMENT avec la b.Board

```blocks

input.onGesture(Gesture.Shake, function () {
for (let index = 0; index < 4; index++) {
BLiXel.showColour(0xff0000)
basic.pause(500)
BLiXel.showColour(0x000000)
basic.pause(500)
}
})

```
---
##### 🔙 [Menu Retour](#move-deplacer) 
