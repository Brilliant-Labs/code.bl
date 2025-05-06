# ACTIVITY 7
# NETWORKING 

---
##### ~avatar
Intro video about the Internet and basic Networking
https://www.youtube.com/watch?v=T-YrekltWW8
##### ~ 
---

Official Document in **English** [__👉 Here__](https://www.canva.com/design/DAF-7f4_b20/UsBmppJ8Pcti1uN7xQaQLA/edit)

Document officiel en **French** [__👉 Ici__](https://www.canva.com/design/DAGE2NHE8Vs/2NNCaqrKK6dGwYJq4I7KKw/edit)

---

## CONNECTING

#### __🧑‍🎓 Students:__
__1.__ Create a new project using the micro:bit V2, ensuring that you are working with a __b.Board Rev 1.4__ and naming it "Networking_A". You can find instructions on how to identify the hardware and software version of your __b.Board__ [__👉Here__](https://drive.google.com/file/d/1yllWJcc--RhKsAEizD8vK-3rGGuAAV-P/view?usp=sharing).

<!-- ![Step1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step1.png?raw=true "Step1") -->
![Step1](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step1.png?raw=true "Step1") 

__2.__ Use the 🧩 ``||Connect to WiFi("") with Password("")||`` block and place it inside the 🧩 ``||On Start||`` block.

__3.__ Make sure you use the exact WiFi name as it appears on the M5 module. Ask the teacher 🧑‍🏫 for the correct information.

<!-- ![Step2](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step2.png?raw=true "Step2") --> 
![Step2](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step2.png?raw=true "Step2") 

__4.__ Use the logic conditional 🧩 ``||if||`` block to know if you are connected. If you are connected then display a 😃 smiley face on the micro:bit with the 🧩 ``||show icon||`` block.

__5.__ Next, create another block 🧩 to disconnect from the network. You can use the 🧩 ``||on logo pressed||`` input block for this and place 🧩 ``||WiFi Disconnect||`` block inside of it, additionally add a 🧩 ``||show icon||`` block after disconnecting to show a 🙁 sad face after disconnecting.

<!-- ![Step3](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step3.png?raw=true "Step3") -->
![Step3](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step3.png?raw=true "Step3")

__6.__ Turn on the __b.Board__ and establish communication between the PC, micro:bit and __b.Board__.

<!-- ![Step4](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step4.png?raw=true "Step4") -->
![Step4](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step4.png?raw=true "Step4")

__7.__ ⬇️ Download the code and check the connection and disconnection code with the 📳 M5 module WiFi access point.

## ``|>_|`` Code Example:
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_A.hex). 

Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes below to modify it in the 🧩 Blocks editor.
<!-- ![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")-->
This code example to evaluate your connection and test it.
```javascript
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.Disconnect()
    basic.showIcon(IconNames.Sad)
})
Cybersec.WifiConnect("Cyberville #?", "")
if (Cybersec.WiFi_Connected()) {
    basic.showIcon(IconNames.Happy)
}
```

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

### ~ avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
---

---
---
## MAC AND IP ADDRESS
#### 🧑‍🎓 __Students:__

__1.__ Go to https://code-alpha.brilliantlabs.ca/ and create a new project or use the Cyber_Network project created in the previous activity.

__2.__ Within the project, use the 🧩 ``||on button A pressed||`` block.

__3.__ Replace the “Hello!” text in the 🧩 ``||show string||`` block with the 🧩 ``||Get the b.Board´s MAC Address||`` block. This is located under "b.Board blocks" in "CyberSecurity".

<!-- ![Step5](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step5.png?raw=true "Step 3") -->
![Step5](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step5.png?raw=true "Step 3")

__4.__ Add a new 🧩 ``||on button A pressed||`` block, however this time select "on button B pressed".

__5.__ Replace the “Hello!” text in the 🧩 ``||show string||`` block with the 🧩 ``||Get the bBoard´s IP Address||`` block. This is located under "__b.Board__ blocks" in "CyberSecurity".

<!-- ![Step6](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step6.png?raw=true "Step 5") -->
![Step6](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step6.png "Step 5")

__6.__ Turn on the __b.Board__ and establish communication between the PC, micro:bit and __b.Board__.

<!-- ![Step7](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step7.png?raw=true "Download to microbit") -->
![Step7](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step7.png?raw=true "Download to microbit")


__7.__ ⬇️ Download the code to micro:bit.

__8.__ The student's will now display their unique MAC Address 🆔 on micro:bit screen pressing A button, and the IP Address 📮 pressing B button.

The MAC address 🆔 will be displayed on micro:bit display, similar to this (Scrolling ⏪):  
__`My MAC: 34:ab:95:98:d1:f8`__      
And the IP address 📮 will be displayed on Microbit display, similar to this (Scrolling ⏪):  
__`My IP: 192.168.4.2`__
       
__9.__ At the end of this activity 🧑‍🏫 teachers should talk with their 🧑‍🎓 students about why 🆔 MAC and 📮 IP addresses are crucial for cybersecurity and the development of __Cyberville__.

***

####  ``|>_|`` Code Example:
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex). 

Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes below to modify it in the 🧩 Blocks editor.
<!--![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")-->
You can use this code example to obtain the 🆔 MAC and 📮 IP addresses.

```javascript
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
##### ~avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
---

---
---
## ROLES
#### 🧑‍🎓 __Students:__
__1.__ Fill out your __Cyberville ID__ Card with names, MAC addresses 🆔, and IP addresses 📮.

__2.__ Acquire an identity by choosing a role within __Cyberville__.

__3.__ Program the micro:bit so your icon is always displayed on the micro:bit screen to indicate that you are connected to the __Cyberville__ Wi-Fi network.

__4.__ Program the micro:bit to play a sound or a melody (You can find this in the music blocks) if you are not connected to the __Cyberville__ WiFi network.

Please choose one of the following roles in __Cyberville__: 
<!--  ![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol") -->
![Rol](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol")

As an example, if you chose __💧 WATER__ and are connected to the WiFi Network, then your micro:bit should look like this:

<!-- ![Step10](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Step10.png?raw=true "Step10") -->
![Step10](https:/raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Step10.png?raw=true "Step10")

Once you've successfully linked each __b.Board__ in the classroom to __Cyberville__ and assigned it a role, it's time for the fun part! Your teacher will simulate a __Cyber Attack__ by disabling the M5 module, which is the WiFi provider for __Cyberville__. This will disconnect all the devices in __Cyberville__, creating a situation of chaos within the __Cyberville__ network!

#### ``|>_|`` Code Example:
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_C.hex). 

Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes below to modify it in the 🧩 Blocks editor.
<!-- ![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")-->

You can use this code example to have a __👤 Role__ in __Cyberville__, please change the 💧 WATER for your own role.

```javascript
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
##### ~avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
---

---
---
## PINGING
### Task
Let's quickly check if the access point 📳 M5Core2 Module is available. Just do a __Ping__, and we'll know in no time! It has a handy default IP address of 192.168.4.1, which is perfect for getting started using the command PING! 
It would be really fun to share our ID cards and find out who our classmates are connected to! Don't forget to set up your friends' IP addresses in the block 🧩 ``||Do PING to IP("")||``, and make sure you're connected to the right access point 📳.
You'll get a 😊 smiley face if your request role is available in the network, and a 😔 sad face if it's not.

#### ``|>_|`` Code Example:
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_D.hex). 
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes below to modify it in the 🧩 Blocks editor.
<!--  
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")-->
You can use this code example to __pinging__ your friends.
```javascript
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```
##### ~avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
---
