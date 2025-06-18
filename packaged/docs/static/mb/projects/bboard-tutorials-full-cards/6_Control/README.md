# 📒 b.Board Tutorial Cards / 📒 Cartes de tutoriel b.Board:

# `CONTROL-CONTROLE`

| English | French |
| ------------------------------- | ------------------------------- | 
| [Use A-B Buttons](#use-ab-buttons) | [Utiliser les boutons AB](#utiliser-les-boutons-ab) | 
| [Pump a Balloon](#pump-a-balloon) | [Gonfler un ballon](#gonfler-un-ballon) |
| [Make it Keep Score](#make-it-keep-score) | [Faire un compteur de points](#faire-un-compteur-de-points) |
| [Make it Pump Water](#make-it-pump-water) | [Faire pomper de l eau](#faire-pomper-de-l-eau) | 
| [Make it Timer](#make-it-timer) | [Faire un minuteur](#faire-un-minuteur) |
| [Make it Stopwatch](#make-it-stopwatch) | [Faire un chronometrer](#faire-un-chronometrer) |
| [Make it Count](#make-it-count) | [Faire compter](#faire-compter) | 
| [Make it Detect Water](#make-it-detect-water) | [Faire detecter de l eau](#faire-detecter-de-l-eau) |
| [Temp Fan Controled Icon](#temp-fan-controled-icon) | [Icone de ventilateur controle par la temperature](#icone-de-ventilateur-controle-par-la-temperature)   |
| [Weather Station](#weather-station) | [Station météo](#station-meteo) |
| [Heads Tails](#heads-tails) | [Pile ou face](#pile-ou-face) |
| [Rock Paper Scissors](#rock-paper-scissors) | [Pierre papier ciseaux](#pierre-papier-ciseaux) |
| [Make it Emotions](#make-it-emotions) | [Exprimer des emotions](#exprimer-des-emotions) |
| [Make it Count Steps](#make-it-count-steps) | [Compter les pas](#compter-les-pas) |
| [Make a Die](#make-a-die) | [Faire un dé](#faire-un-de) |
---
---
# `🇬🇧 ENGLISH`
---
## Use AB Buttons
![Use_A-B_buttons-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control1/Use_A-B_buttons-EN.png?raw=true "Use_A-B_buttons-EN")

## Code Example

Example USE A,B AND AB BUTTONS using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
basic.showIcon(IconNames.Heart)
})
input.onButtonPressed(Button.B, function () {
basic.showIcon(IconNames.Yes)
})

```
---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Pump a Balloon

![Pump_a_balloon-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control2/Pump_a_balloon-EN.png?raw=true "Pump_a_balloon-EN")

## Code Example

Example PUMP UP AND DEFLATE A BALLON using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorLeftTimed(50, 1000)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorRightTimed(50, 1000)
})

```
---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Keep Score
![Mkt_Keep_Score-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control3/Mkt_Keep_Score-EN.png?raw=true "Mkt_Keep_Score-EN")

## Code Example

Example MAKE IT KEEP SCORE using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
Score += 1
})
input.onButtonPressed(Button.AB, function () {
Score = 0
})
input.onButtonPressed(Button.B, function () {
Score += -1
})
let Score = 0
Score = 0
basic.forever(function () {
basic.showNumber(Score)
})

```

---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Pump Water

![Mkt_Pump_Water-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control4/Mkt_Pump_Water-EN.png?raw=true "Mkt_Pump_Water-EN")

## Code Example

Example MAKE IT PUMP WATER using the b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorDuty(100)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorDuty(0)
})

```

---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Timer

![Mkt_Timer-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control5/Mkt_Timer-EN.png?raw=true "Mkt_Timer-EN")

## Code Example

Example MAKE IT A TIMER using the b.Board

```blocks

let seconds = 0
input.onButtonPressed(Button.A, function () {
if (seconds < 50) {
seconds += 10
basic.showNumber(seconds)
basic.clearScreen()
}
})
input.onButtonPressed(Button.B, function () {
while (seconds > 0) {
basic.showNumber(seconds)
basic.pause(1000)
seconds += 0 - 1
}
})

```

---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Stopwatch
![Mkt_Stopwatch-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control6/Mkt_Stopwatch-EN.png?raw=true "Mkt_Stopwatch-ENN")

## Code Example

Example MAKE IT A STOPWATCH using the b.Board

```blocks

let secondes = 0
input.onButtonPressed(Button.A, function () {
if (secondes < 50) {
secondes += 10
basic.showNumber(secondes)
basic.clearScreen()
}
})
input.onButtonPressed(Button.B, function () {
while (secondes > 0) {
basic.showNumber(secondes)
basic.pause(1000)
secondes += 0 - 1
}
})

```

---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Count
![Mkt_Count-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control7/Mkt_Count-EN.png?raw=true "Mkt_Count-EN")

## Code Example

Example MAKE IT COUNT using the b.Board

```blocks

let Counting = 0
basic.forever(function () {
Counting += 1
basic.pause(1000)
basic.showString("" + (Counting))
})

```

---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Detect Water

![Mkt_Detect_Water-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control8/Mkt_Detect_Water-EN.png?raw=true "Mkt_Detect_Water-EN")


---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Temp Fan Controled Icon
![Temp_Fan_Controled_Icon-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control9/Temp_Fan_Controled-EN.png?raw=true "Temp_Fan_Controled_Icon-EN")


---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Weather Station
![Weather_Station-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control10/Weather_Station-EN.png?raw=true "Weather_Station-EN")


---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Heads Tails
![Heads_Tails-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control11/Heads_Tails-EN.png?raw=true "Heads_Tails-EN")


---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Rock Paper Scissors
![Rock_Paper_Scissors-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control12/Rock_Paper_Scissors-EN.png?raw=true "Rock_Paper_Scissors-EN")


---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Emotions
![Mkt_Emotions-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control13/Mkt_Emotions-EN.png?raw=true "Mkt_Emotions-EN")


---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make it Count Steps

![Mkt_Count_Steps-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control14/Mkt_Count_Steps-EN.png?raw=true "Mkt_Count_Steps-EN")

---
##### 🔙 [Back Menu](#control-controle) 
---
---
## Make a Die
![Mk_a_Die-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control15/Mk_a_Die-EN.png?raw=true "Mk_a_Die-EN")

---
##### 🔙 [Back Menu](#control-controle) 



























---
---
# `🇫🇷 FRENCH`
---
---
## Utiliser les boutons AB
![Use_A-B_buttons-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control1/Use_A-B_buttons-FR.png?raw=true "Use_A-B_buttons-FR")

## Exemple de code

Exemple : UTILISER LES BOUTONS A, B ET AB avec la b.Board

```blocks

input.onButtonPressed(Button.A, function () {
basic.showIcon(IconNames.Heart)
})
input.onButtonPressed(Button.B, function () {
basic.showIcon(IconNames.Yes)
})

```
---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Gonfler un ballon

![Pump_a_balloon-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control2/Pump_a_balloon-FR.png?raw=true "Pump_a_balloon-FR")

## Exemple de code

Exemple : GONFLER ET DÉGONFLER UN BALLON avec la b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorLeftTimed(50, 1000)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorRightTimed(50, 1000)
})

```
---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Faire un compteur de points
![Mkt_Keep_Score-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control3/Mkt_Keep_Score-FR.png?raw=true "Mkt_Keep_Score-FR")

## Exemple de code

Exemple : FAIRE UN COMPTEUR DE POINTS avec la b.Board

```blocks

input.onButtonPressed(Button.A, function () {
Score += 1
})
input.onButtonPressed(Button.AB, function () {
Score = 0
})
input.onButtonPressed(Button.B, function () {
Score += -1
})
let Score = 0
Score = 0
basic.forever(function () {
basic.showNumber(Score)
})

```

---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Faire pomper de l eau

![Mkt_Pump_Water-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control4/Mkt_Pump_Water-FR.png?raw=true "Mkt_Pump_Water-FR")

## Exemple de code

Exemple : FAIRE POMPER DE L’EAU avec la b.Board

```blocks

input.onButtonPressed(Button.A, function () {
bBoard_Motor.motorDuty(100)
})
input.onButtonPressed(Button.B, function () {
bBoard_Motor.motorDuty(0)
})

```

---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Faire un minuteur

![Mkt_Timer-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control5/Mkt_Timer-FR.png?raw=true "Mkt_Timer-FR")

## Exemple de code

Exemple : EN FAIRE UN MINUTERIE avec la b.Board

```blocks

let seconds = 0
input.onButtonPressed(Button.A, function () {
if (seconds < 50) {
seconds += 10
basic.showNumber(seconds)
basic.clearScreen()
}
})
input.onButtonPressed(Button.B, function () {
while (seconds > 0) {
basic.showNumber(seconds)
basic.pause(1000)
seconds += 0 - 1
}
})

```

---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Faire un chronometrer
![Mkt_Stopwatch-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control6/Mkt_Stopwatch-FR.png?raw=true "Mkt_Stopwatch-FR")

## Exemple de code

Exemple : EN FAIRE UN CHRONOMÈTRE avec la b.Board

```blocks

let secondes = 0
input.onButtonPressed(Button.A, function () {
if (secondes < 50) {
secondes += 10
basic.showNumber(secondes)
basic.clearScreen()
}
})
input.onButtonPressed(Button.B, function () {
while (secondes > 0) {
basic.showNumber(secondes)
basic.pause(1000)
secondes += 0 - 1
}
})

```

---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Faire compter
![Mkt_Count-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control7/Mkt_Count-FR.png?raw=true "Mkt_Count-FR")

## Exemple de code

Exemple : LE FAIRE COMPTER avec la b.Board

```blocks

let Counting = 0
basic.forever(function () {
Counting += 1
basic.pause(1000)
basic.showString("" + (Counting))
})

```

---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Faire detecter de l eau

![Mkt_Detect_Water-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control8/Mkt_Detect_Water-FR.png?raw=true "Mkt_Detect_Water-FR")


---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Icone de ventilateur controle par la temperature
![Temp_Fan_Controled_Icon-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control9/Temp_Fan_Controled-FR.png?raw=true "Temp_Fan_Controled_Icon-FR")


---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Station meteo
![Weather_Station-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control10/Weather_Station-FR.png?raw=true "Weather_Station-FR")


---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Pile ou face
![Heads_Tails-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control11/Heads_Tails-FR.png?raw=true "Heads_Tails-FR")


---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Pierre Papier Ciseaux
![Rock_Paper_Scissors-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control12/Rock_Paper_Scissors-FR.png?raw=true "Rock_Paper_Scissors-FR")


---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Exprimer des emotions
![Mkt_Emotions-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control13/Mkt_Emotions-FR.png?raw=true "Mkt_Emotions-FR")


---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Compter les pas

![Mkt_Count_Steps-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control14/Mkt_Count_Steps-FR.png?raw=true "Mkt_Count_Steps-FR")

---
##### 🔙 [Menu Retour](#control-controle) 
---
---
## Faire un de
![Mk_a_Die-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control15/Mk_a_Die-FR.png?raw=true "Mk_a_Die-FR")

---
##### 🔙 [Menu Retour](#control-controle) 
