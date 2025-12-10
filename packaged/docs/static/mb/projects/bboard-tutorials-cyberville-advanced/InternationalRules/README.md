## ACTIVITY 13
# 🌍⚖️ INTERNATIONAL RULES

---
##### ~avatar
Intro video about Cybersecurity Level 3 Advanced
https://youtu.be/HIquW6LqKH8
##### ~
</br>

# 📘 __*Guide Document:*__  
- Official Document in **English** [__👉 Here__](https://www.canva.com/design/DAGvHD-m7yE/c9Lov7drZ2TSuBBH7fhZ6A/view?utm_content=DAGvHD-m7yE&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h4b1a848386)
- Document officiel en **French** [__👉 Ici__](https://www.canva.com/design/DAG1Kj7iqF8/nAsd5nnctZdd4ko46qTk8A/view?utm_content=DAG1Kj7iqF8&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h7ad7337795)
</br>
</br>

# 🚀 __*Let's get started!*__

## ⬇️ Download Codes </br>
- It’s a great idea to prepare four separate projects, each with the correct code for its task, before getting started. This will help you stay organized and feel ready when it’s time to work on them.

    👉 Download the next three .hex files, then for each file, create a ``➕ New Project`` and drag and drop the file for each task </br>
    + __``Task #1: Conveyor Belt Model``__ [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/ConveyorBelt.hex).</br>
    + __``Task #2: Cookies Factory Model - Factory Local``__  [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Factory-Local.hex).</br>
    + __``Task #3: Cookies Factory Cyberville``__  [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Factory-Cyberville.hex).</br>

## __``Task #1: Conveyor Belt Model``__
- 1️⃣ The conveyor belt model is represented by the 'NeoPixel' strip. Each lit pixel (blixel) on the strip represents a cookie that has been made. When a blixel turns on, it means one cookie is ready.
Once 10 cookies are ready, they are considered packaged and ready to sell.

- 2️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/ConveyorBelt.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onButtonPressed(Button.AB, function () {
    CybersecAdvanced.ResetBelt()
    Cookies = 0
    basic.clearScreen()
})
input.onPinReleased(TouchPin.P1, function () {
    if (Cookies < 30) {
        CybersecAdvanced.Cookcookies()
        Cookies += 1
        basic.showNumber(Cookies)
    }
})
let Cookies = 0
CybersecAdvanced.createbelt(DigitalPin.P2)
Cookies = 0
```

## __``Task #2: Cookies Factory Model``__
- 1️⃣ Once you understand how the conveyor belt and the servomotor work, it's time to bake cookies in your factory using the robot arm (based on the servomotor), the conveyor belt (using the NeoPixel strip), and the complete production machine.

- 2️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Factory-Local.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onButtonPressed(Button.A, function () {
    servos.P00.setAngle(180)
    basic.pause(500)
    servos.P00.setAngle(0)
})
input.onButtonPressed(Button.AB, function () {
    CybersecAdvanced.ResetBelt()
})
input.onPinReleased(TouchPin.P1, function () {
    CybersecAdvanced.Cookcookies()
})
CybersecAdvanced.createbelt(DigitalPin.P2)
servos.P00.setAngle(0)
```

## __``Task #3: Run Your Cookie Factory in Cyberville!``__  
- 1️⃣ Once you are connected to the Cyberville Network, you can start baking 🍪 cookies — but only when you have enough power from Cyberville’s electric power system through the 📳 M5 access point!
Remember, the power level is shown on the b.Board blixels. ⌛️ Don't let the countdown reach zero!!!

- 2️⃣ 👨‍🏫 The teacher should start and pause the countdown timer on the 📳 M5 module by pressing Button A, allowing time for the team’s speech. When the team finishes their presentation, the teacher should resume the timer by pressing Button A again — this will restore power and allow the cookies to start baking again. Don’t forget to raise your hand 🙋🏼‍♂️ when your cookies are ready to sell and when you’re prepared to give your 🎤 speech about the International Rules of Cybersecurity. Remember, this is how you help counteract the malware system infrastructure installed by the bad guys!

- 3️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Factory-Cyberville.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onButtonPressed(Button.A, function () {
    servos.P00.setAngle(180)
    basic.pause(500)
    servos.P00.setAngle(0)
})
input.onButtonPressed(Button.AB, function () {
    CybersecAdvanced.ResetBelt()
})
input.onPinReleased(TouchPin.P1, function () {
    if (CybersecAdvanced.PowerIsAvailable()) {
        CybersecAdvanced.Cookcookies()
    }
})
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
CybersecAdvanced.createbelt(DigitalPin.P2)
servos.P00.setAngle(0)
```