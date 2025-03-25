# 📒 b.Board Tutorial Cards:

# `CONTROL`

- [Use A-B Buttons](#use-ab-buttons) 
- [Pump a Balloon](#pump-a-balloon) 
- [Make it Keep Score](#make-it-keep-score) 
- [Make it Pump Water](#make-it-pump-water) 
- [Make it Timer](#make-it-timer)
- [Make it Stopwatch](#make-it-stopwatch) 
- [Make it Count](#make-it-count) 
- [Make it Detect Water](#make-it-detect-water)
- [Temp Fan Controled Icon](#temp-fan-controled-icon) 
- [Weather Station](#weather-station) 
- [Heads Tails](#heads-tails) 
- [Rock Paper Scissors](#rock-paper-scissors) 
- [Make it Emotions](#make-it-emotions)
- [Make it Count Steps](#make-it-count-steps) 
- [Make a Die](#make-a-die) 
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
##### 🔙 [Back Menu](#control) 
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
##### 🔙 [Back Menu](#control) 
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
##### 🔙 [Back Menu](#control) 
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
##### 🔙 [Back Menu](#control) 
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
##### 🔙 [Back Menu](#control) 
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
##### 🔙 [Back Menu](#control) 
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
##### 🔙 [Back Menu](#control) 
---
---
## Make it Detect Water

![Mkt_Detect_Water-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control8/Mkt_Detect_Water-EN.png?raw=true "Mkt_Detect_Water-EN")


---
##### 🔙 [Back Menu](#control) 
---
---
## Temp Fan Controled Icon
![Temp_Fan_Controled_Icon-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control9/Temp_Fan_Controled-EN.png?raw=true "Temp_Fan_Controled_Icon-EN")


---
##### 🔙 [Back Menu](#control) 
---
---
## Weather Station
![Weather_Station-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control10/Weather_Station-EN.png?raw=true "Weather_Station-EN")


---
##### 🔙 [Back Menu](#control) 
---
---
## Heads Tails
![Heads_Tails-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control11/Heads_Tails-EN.png?raw=true "Heads_Tails-EN")


---
##### 🔙 [Back Menu](#control) 
---
---
## Rock Paper Scissors
![Rock_Paper_Scissors-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control12/Rock_Paper_Scissors-EN.png?raw=true "Rock_Paper_Scissors-EN")


---
##### 🔙 [Back Menu](#control) 
---
---
## Make it Emotions
![Mkt_Emotions-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control13/Mkt_Emotions-EN.png?raw=true "Mkt_Emotions-EN")


---
##### 🔙 [Back Menu](#control) 
---
---
## Make it Count Steps

![Mkt_Count_Steps-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control14/Mkt_Count_Steps-EN.png?raw=true "Mkt_Count_Steps-EN")

---
##### 🔙 [Back Menu](#control) 
---
---
## Make a Die
![Mk_a_Die-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/6_Control/Control15/Mk_a_Die-EN.png?raw=true "Mk_a_Die-EN")

---
##### 🔙 [Back Menu](#control) 
---
