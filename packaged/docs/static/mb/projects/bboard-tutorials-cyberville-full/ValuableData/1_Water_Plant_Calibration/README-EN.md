### WHAT VALUABLE DATA IS?
__Valuable Data__ is a really important topic in Cybersecurity. It's all about keeping and obtaining information safe and secure on a network. It's not just about digital data, but also about making sure social, mental, and technological security for you, your parents, and your __Cyberville__. It's so important to know where the information is stored, what the source is, how to find it, and try to protect it from unauthorized access and misuse. We're here to help you with all of that!

Let's learn together about some of the most common cyber attacks on our __*Valuable Data*__, for example __Phishing__, __Malware__, __Ransomware__, and how to protect us with __Encryption__ and others. Once we've done that, we'll solve the Mission Polluted Water - Water Treatment Plant Under Attack!.

🧑‍🎓 Students and 🧑‍🏫 teachers, we just wanted to remind you that it's important to choose a __*reliable, secure, safe, and protected source of information*__ on the __Cyberville__ network, to avoid exposing your __Valuable Data__. 

To develop the next tasks:

| Activity Name | Color Hat | Case Study|
| :------------------   | :---: | :----------------- |
| Reliable information  | 🔴 🎩 Red Hat| `Phishing` 🎣|
| Secure information    | ⚫ 🎩 Black Hat| `Malware`  🦠| 
| Safe information      | ⚪ 🎩 White Hat| `Ransomware`  💸|
| Protected information | 🟣 🎩 Blue Hat| `Encription` 🗝️|

<br>
the 📳 M5 Module will provide different __Websites__ selected by the 🧑‍🏫 teacher, which are based on hacker challenges with different __Color 🎩 Hats__ for each activity. It's up to you to choose the most reliable, secure, logical, and intuitive data to get the correct results. Be aware that not all information is credible; it could be infected or may require analysis. But don't worry! It should always be protected. You may fail in the attempt, but that's part of the fun!

---

##### __TASK 1:__ Water Plant Calibration!
All right, let's get started *Calibrating* our levels bar on our plant!

We've made it really easy for you to recreate the awesome environment from Mission Polluted Water while learning about Cybersecurity. All you have to do is download [__👉 Here__](https://drive.google.com/file/d/1CIb0Py6PW8po8vg_LG9Bqw2y229TC2ut/view?usp=sharing), print and cover the __b.board__ for Mission Polluted Water.  
    <img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/M2_Cover.png?raw=true" alt="M2" title="Mission 2 in M5Core2" width="450" />
<!--    ![Cover](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/M2_Cover.png?raw=true "Cover")-->

![Cover for M2](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/Cover_Gif_M2.gif?raw=true "Cover for M2.")

### 🧑‍🏫 __Teachers:__
Teachers will guide the proccess to obtain the neopixel level bar from the students 🧑‍🎓.
### 🧑‍🎓 __Students:__
In this example, you'll find a suggested Water Plant Calibration environment for this activity. But don't be afraid to get creative! You can easily recreate two bars of neopixels for 10 BLixels each, in whatever way you like.

![Level_Bar](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/1_Water_Plant_Calibration/LevelBar.gif?raw=true "Level Bar.")

## ~avatar
__⚠️ Important: WiFi Connection Setup__  
1️⃣ Connect your PC to the WiFi access point broadcast by your 📳 M5 module   
2️⃣ Once connected, open your web browser  
3️⃣ Navigate to: __``http://192.168.4.1``__  
4️⃣ Get the clues to solve the tasks
## ~
### ``|>_|`` Code Example:
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://brilliantlabs.ca/documents/cybersec/M2-Water-Plant-Calibration.hex). Once downloaded, either drag and drop it into a new project.

You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```javascript
input.onButtonPressed(Button.A, function () {
    for (let Count = 0; Count <= 9; Count++) {
        CL_Strip.setPixelColor(Count + (10 - Cybersec.indexcl(Index_CL.five)), neopixel.colors(NeoPixelColors.Blue))
        FL_Strip.setPixelColor(Count + (-10 + Cybersec.indexfl(Index_FL.five)), neopixel.colors(NeoPixelColors.Green))
    }
    Full_Strip.show()
})
let FL_Strip: neopixel.Strip = null
let CL_Strip: neopixel.Strip = null
let Full_Strip: neopixel.Strip = null
Full_Strip = neopixel.create(DigitalPin.P2, 30, NeoPixelMode.RGB)
CL_Strip = Full_Strip.range(20, 10)
FL_Strip = Full_Strip.range(0, 10)
```
<!--or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit") -->

Or use the example code below as a new project. Please pay attention that strip is connected to __P2__, and the levels are __5 for 🧪Chlorine__ and __5 for 🧪 Fluoride__, also notice that we are using the 🧩 ``||Level of Chlorine (#)||`` block, and the 🧩 ``||Level of Fluoride (#)||`` block to set the levels of `Chorine` and `Fluoride`.

##### ~avatar
You should change the values for __🧪Chloride__ and __🧪Flouride__ according to each activity, that means you need to modify this code using the __Level of Choride__ and __Level of Flouride__ Blocks in to section `... more` under CyberSecurity button from __b.Board__. 
##### ~

```blocks
input.onButtonPressed(Button.A, function () {
    for (let Count = 0; Count <= 9; Count++) {
        CL_Strip.setPixelColor(Count + (10 - Cybersec.indexcl(Index_CL.five)), neopixel.colors(NeoPixelColors.Blue))
        FL_Strip.setPixelColor(Count + (-10 + Cybersec.indexfl(Index_FL.five)), neopixel.colors(NeoPixelColors.Green))
    }
    Full_Strip.show()
})
let FL_Strip: neopixel.Strip = null
let CL_Strip: neopixel.Strip = null
let Full_Strip: neopixel.Strip = null
Full_Strip = neopixel.create(DigitalPin.P2, 30, NeoPixelMode.RGB)
CL_Strip = Full_Strip.range(20, 10)
FL_Strip = Full_Strip.range(0, 10)
```
</br>
</br>

<!--### Main Website preview from M5 Webserver - Activities Valuable Data![Main](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/Webs_png/Web_Main_EN.png?raw=true "Main")-->

<!--# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝**Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~ -->