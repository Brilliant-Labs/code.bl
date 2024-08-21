# 1_VALUABLE DATA

__Valuable Data__ is a really important topic in Cybersecurity. It's all about keeping and obtaining information safe and secure on a network. It's not just about digital data, but also about making sure social, mental, and technological security for you, your parents, and your __Cyberville__. It's so important to know where the information is stored, what the source is, how to find it, and try to protect it from unauthorized access and misuse. We're here to help you with all of that!

Let's learn together about some of the most common attacks on our __*Valuable Data*__. Once we've done that, we'll solve the Second Mission, "Polluted Water - Water Treatment Plant Under Attack!"

## Activity
__Let's start!__   

We've made it really easy for you to recreate the awesome environment from Mission 2 while learning about Cybersecurity. All you have to do is:

__1.__ [Download](https://www.canva.com/design/DAGJhxRPFpY/D54nS2FDqO65RD4bMEKsbQ/view?utm_content=DAGJhxRPFpY&utm_campaign=designshare&utm_medium=link&utm_source=editor), print and cover the b.board for Mission 2.  

<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/M2_Cover.png?raw=true" alt="M2" title="Mission 2 in M5Core2" width="450" />

![Cover](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/Cover_Gif_M2.gif?raw=true "Cover for M2.")

## 🧑‍🏫 __Teachers:__

Teachers will guide the proccess to obtain the neopixel level bar from the students 🧑‍🎓.


## 🧑‍🎓 __Students:__

In this example, you'll find a suggested Water Plant Calibration environment for this activity. But don't be afraid to get creative! You can easily recreate two bars of neopixels for 10 BLixels each, in whatever way you like. __Have fun!__

![Level_Bar](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/LevelBar.gif?raw=true "Level Bar.")

## Code Example

You can download the code for this activity from `https://brilliantlabs.ca/documents/cybersec/M2-Water-Plant-Calibration.hex` the file will be in Recent Download History, just drag and drop it into a new project.  

Or use this code as example. Please pay attention that strip is connected to __P2__, and the levels are __5 for 🧪 Chlorine__ and __5 for 🧪 Fluoride__. You should change this values according to the next activity __*"Get Reliable Information"*__.

```blocks
input.onButtonPressed(Button.A, function () {
    for (let Count = 0; Count <= 9; Count++) {
        FL_Strip.setPixelColor(Count + (-10 + Flouride), neopixel.colors(NeoPixelColors.Green))
        CL_Strip.setPixelColor(Count + (10 - Chloride), neopixel.colors(NeoPixelColors.Blue))
    }
    Full_Strip.show()
})
let Chloride = 0
let Flouride = 0
let CL_Strip: neopixel.Strip = null
let FL_Strip: neopixel.Strip = null
let Full_Strip: neopixel.Strip = null
Full_Strip = neopixel.create(DigitalPin.P2, 30, NeoPixelMode.RGB)
FL_Strip = Full_Strip.range(0, 10)
CL_Strip = Full_Strip.range(20, 10)
Flouride = 5
Chloride = 5
```