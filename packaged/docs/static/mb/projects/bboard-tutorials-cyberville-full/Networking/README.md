## ACTIVITY 7
## 🔗 NETWORKING 

---
##### ~avatar
Intro video about the Internet and basic Networking
https://www.youtube.com/watch?v=T-YrekltWW8
##### ~

## 📘 __*Guide Document:*__  
- Official Document in **English** [__👉 Here__](https://www.canva.com/design/DAF-7f4_b20/UsBmppJ8Pcti1uN7xQaQLA/edit)
- Document officiel en **French** [__👉 Ici__](https://www.canva.com/design/DAGE2NHE8Vs/2NNCaqrKK6dGwYJq4I7KKw/edit)

## 🚀 __*Let's get started!*__
__``Task #1: Connecting``__

1. Create a new project using the micro:bit V2, ensuring that you are working with a __b.Board Rev 1.4__ and naming it "Networking_A". You can find instructions on how to identify the hardware and software version of your __b.Board__ **EN**: [__👉 Click here__](https://drive.google.com/file/d/1yllWJcc--RhKsAEizD8vK-3rGGuAAV-P/view?usp=sharing), **FR**: [__👉 Click here__](https://drive.google.com/file/d/1yllWJcc--RhKsAEizD8vK-3rGGuAAV-P/view?usp=sharing),

    ![Version](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/Version.png?raw=true "Version") 

2. Download the ID card for the __Networking__ activity: 
- __*Teachers ID Card*__ 🧑‍🏫 [__👉 Here__](https://drive.google.com/file/d/14gh8mT6u4rgxHwiSSV6rtSel3Gz4WwM_/view?usp=drive_link)
- __*Students ID Card*__ 🧑‍🎓 [__👉 Here__](https://drive.google.com/file/d/1uYi49zPMzKYuliF4TlS2NQBoPTkMTcoD/view?usp=drive_link) 

    This is an example of what to expect for this activity:
![ID Example](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Example_EN.png?raw=true "ID Example")  

3. Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_A.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.Disconnect()
    basic.showIcon(IconNames.Sad)
})
Cybersec.WifiConnect("Cyberville #?", "")
if (Cybersec.WiFi_Connected()) {
    basic.showIcon(IconNames.Happy)
}
```

4. Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.

__``Task #2: MAC and IP address``__  

1. Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString(Cybersec.getMACaddressbBoard())
})
input.onButtonPressed(Button.B, function () {
    basic.showString(Cybersec.getIPaddressbBoard())
})
Cybersec.WifiConnect("Cyberville #?", "")
basic.forever(function () {	
})
```

2. You should display their unique MAC Address 🆔 on micro:bit screen pressing A button, and the IP Address 📮 pressing B button.

    The MAC address 🆔 will be displayed on micro:bit display, similar to this (Scrolling ⏪):  
__`My MAC: 34:ab:95:98:d1:f8`__  
    And the IP address 📮 will be displayed on Microbit display, similar to this (Scrolling ⏪):  
__`My IP: 192.168.4.2`__

3. Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.

__``Task #3: Roles``__  

1. Please choose one of the following roles in __Cyberville__: 
![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol")

2. Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_C.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString(Cybersec.getMACaddressbBoard())
})
input.onButtonPressed(Button.B, function () {
    basic.showString(Cybersec.getIPaddressbBoard())
})
Cybersec.WifiConnect("Cyberville #?", "")
basic.forever(function () {
    if (Cybersec.WiFi_Connected()) {
        basic.showIcon(IconNames.Umbrella)
    } else {
        soundExpression.sad.play()
        basic.showIcon(IconNames.Sad)
    }
})
```
3. Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.


__``Task #4: Pinging``__  

1. Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_D.hex). 
    Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```

2. Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.


## 📌 __*Notes:*__

☑️ Please do not forget to set up the correct name and password for the access point.     
☑️ Mute the PC sound to listen the __b.Board__ sound.    
☑️ If you’d like, you can also view the data going in and out of the b.Board using the __*Show Console Device*__ option.    

    Once you download your code...
- Click on the refresh button 🔄 (circular arrow icon) in the simulator window.
- __Wait__ until *Show console Device* button apears on console output window.
- Click on it.

![Console](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Console.png?raw=true "Console Device")