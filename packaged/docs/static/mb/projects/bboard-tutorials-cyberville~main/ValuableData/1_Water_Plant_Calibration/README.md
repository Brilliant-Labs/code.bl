# 1_VALUABLE DATA ... Under Construction!

__Valuable Data__ is a really important topic in Cybersecurity. It's all about keeping and obtaining information safe and secure on a network. It's not just about digital data, but also about making sure social, mental, and technological security for you, your parents, and your Cyberville. It's so important to know where the information is stored, what the source is, how to find it, and try to protect it from unauthorized access and misuse. We're here to help you with all of that!

Let's learn together about some of the most common attacks on our Valuable Data. Once we've done that, we'll solve the Second Mission, "Polluted Water - Water Treatment Plant Under Attack!"

## Activity
Let's start!   

We've made it really easy for you to recreate the awesome environment from Mission 2 while learning about Cybersecurity. All you have to do is:

__1.__ [Download](https://www.canva.com/design/DAGJhxRPFpY/D54nS2FDqO65RD4bMEKsbQ/view?utm_content=DAGJhxRPFpY&utm_campaign=designshare&utm_medium=link&utm_source=editor), print and cover the b.board for Mission 2.  
<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Wate_Plant_Calibration/M2_Cover.png?raw=true" alt="M2" title="Mission 2 in M5Core2" width="300" />

![Cover](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/Cover_Gif_M2.gif?raw=true "Cover for M2.")

## 🧑‍🏫 __Teachers:__

Teachers will guide the proccess to obtain the neopixel level bar from the students.


## 🧑‍🎓 __Students:__

In this example, you'll find a suggested Water Plant Calibration environment for this activity. But don't be afraid to get creative! You can easily recreate two bars of neopixels for 10 BLixels each, in whatever way you like. Have fun!

![Level_Bar](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/1_Water_Plant_Calibration/LevelBar.gif?raw=true "Level Bar.")

## Code Example

You can __download__ the code for this activity [here](https://alpha.brilliantlabs.ca/documents/cybersec/Cyber-Security-Activity-7A.hex), or you can go to download from: `https://alpha.brilliantlabs.ca/documents/cybersec/Cyber-Security-Activity-7A.hex`.


Or use this code example is to connect the b.Board to M5Core2.

```blocks
input.onButtonPressed(Button.A, function () {
    General_Strip.clear()
    General_Strip.show()
    for (let Cont1 = 0; Cont1 <= 9; Cont1++) {
        CL_Strip.setPixelColor(Cont1 + (-10 + 5), neopixel.colors(NeoPixelColors.Blue))
    }
    CL_Strip.show()
    for (let Cont2 = 0; Cont2 <= 9; Cont2++) {
        FL_Strip.setPixelColor(Cont2 + (10 - 5), neopixel.colors(NeoPixelColors.Green))
    }
    FL_Strip.show()
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    CL_Strip.clear()
    CL_Strip.show()
    FL_Strip.clear()
    FL_Strip.show()
})
let FL_Strip: neopixel.Strip = null
let CL_Strip: neopixel.Strip = null
let General_Strip: neopixel.Strip = null
General_Strip = neopixel.create(DigitalPin.P2, 30, NeoPixelMode.RGB)
CL_Strip = General_Strip.range(0, 10)
FL_Strip = General_Strip.range(20, 10)
```