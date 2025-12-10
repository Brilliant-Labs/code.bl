## ACTIVITY 7
# 🔗 NETWORKING 

---
##### ~avatar
Intro video about the Internet and basic Networking
https://www.youtube.com/watch?v=T-YrekltWW8
##### ~
</br>

# 🏙️ __*Welcome to Cyberville:*__  
__Cyberville__ is a fun and futuristic city created by Brilliant Labs, where all the citizens or b.Boards are connected to a special Wi-Fi network called Cyberville.

This network is powered by an M5 module, which acts like the city's Wi-Fi provider. It creates a safe and secure access point that lets everyone in Cyberville stay connected.

In the upcoming activities, you’ll become part of this digital community. Help us protect __Cyberville__ from different kinds of cyberattacks!

![Cyberville_MAP](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/Cyberville-EN.png?raw=true "Cyberville MAP")
</br>
</br>

# 📘 __*Guide Document:*__  
- Official Document in **English** [__👉 Here__](https://www.canva.com/design/DAF-7f4_b20/0SFvUdKbH6VVmrPRU3j28w/view?utm_content=DAF-7f4_b20&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h8e9d724200)
- Document officiel en **French** [__👉 Ici__](https://www.canva.com/design/DAGE2NHE8Vs/j7WelLKiHV_mHTBhTRYKaw/view?utm_content=DAGE2NHE8Vs&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hb4d97300ff)
</br>
</br>

# 🚀 __*Let's get started!*__

## ⬇️ Download Codes </br>
- It’s a great idea to prepare four separate projects, each with the correct code for its task, before getting started. This will help you stay organized and feel ready when it’s time to work on them.

    👉 Download the next four .hex files, then for each file, create a ``➕ New Project`` and drag and drop the file for each task </br>
    + __``Task #1: Connecting``__ [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking-Task-1.hex).</br>
    + __``Task #2: MAC and IP address``__  [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking-Task-2.hex).</br>
    + __``Task #3: Roles``__  [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking-Task-3.hex).</br>
    + __``Task #4: Pinging``__ [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking-Task-4.hex).</br>


## __``Task #1: Connecting``__

- 1️⃣ 🧑‍🏫  __Teachers__    
You have received, for activities 7 to 12, an ESP32 touchscreen 📳 M5Stack Core2 module for the Internet of Things (IoT). This will be useful for creating a Wi-Fi network inside your classroom, functioning as an access point. It has already been programmed to broadcast a Wi-Fi signal within your classroom. However, it does not allow access to external websites such as Google or others.

    Teachers must select the __Networking__ activity on the M5Core2 module, and follow the steps according to the 📘 Guide Document.

    To select any activity within M5 module, see this **EN** [🎬 __*video*__](https://drive.google.com/file/d/1Ra37Ctwg_KHiViCR3XP2hXUteJ2BQ-y6/view?usp=sharing) or **FR** [🎬 __*video*__](https://drive.google.com/file/d/10wwarSBpShICwBmd_FT7_MREetXONrN8/view?usp=sharing).

    This is a basic spec sheet for the M5 Module:

    <img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/M5core2.png?raw=true" alt="M5core2" title="Spec sheet M5Core2" width="400" />

- 🧑‍🎓 __Students__  
    Create a new project using the micro:bit V2, ensuring that you are working with a __b.Board Rev 1.4__ and naming it "Networking_A".      You can find instructions on how to identify the hardware and software version of your __b.Board__ **EN**: [__👉 Click here__](https://drive.google.com/file/d/1yllWJcc--RhKsAEizD8vK-3rGGuAAV-P/view?usp=sharing), or **FR**: [__👉 Click here__](https://drive.google.com/file/d/1CNfE8U6z9BpZur0wZq9BgEN3jootvnbB/view?usp=sharing).
    
    ![Version](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Networking/Version.png?raw=true "Version")

- 2️⃣ Download the ID card for the __Networking__ activity: 
    - 🧑‍🏫 Teachers ID Card **EN** [__👉 Here__](https://drive.google.com/file/d/14gh8mT6u4rgxHwiSSV6rtSel3Gz4WwM_/view?usp=drive_link), or **FR** [__👉 Here__](https://drive.google.com/file/d/1L_Q3F4pbEFy0FwHtw97My_tA7F-5hCj-/view?usp=sharing).  
    - 🧑‍🎓 Students ID Card **FR** [__👉 Here__](https://drive.google.com/file/d/1uYi49zPMzKYuliF4TlS2NQBoPTkMTcoD/view?usp=drive_link),  or **FR** [__👉 Here__](https://drive.google.com/file/d/1EnfeuJK2KT-1-K8Pp-kZ2VPfwaLjvDFZ/view?usp=sharing).

        This is an example of what to expect for this activity:
![ID Example](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Example_EN.png?raw=true "ID Example")

</br>

- 3️⃣ Download the ``Code Example`` .hex file (if you haven't already) for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_A.hex). 
Once downloaded, you can either drag and drop it into a new project.

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

- 4️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
</br>
</br>

## __``Task #2: MAC and IP address``__  

- 1️⃣ Download the ``Code Example`` .hex file (if you haven't already)  for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex). 
Once downloaded, you can either drag and drop it into a new project.

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

- 2️⃣ You should display their unique MAC Address 🆔 on micro:bit screen pressing A button, and the IP Address 📮 pressing B button.

    The MAC address 🆔 will be displayed on micro:bit display, similar to this (Scrolling ⏪):  

        My MAC: 34:ab:95:98:d1:f8   
    And the IP address 📮 will be displayed on Microbit display, similar to this (Scrolling ⏪):  

        My IP: 192.168.4.2
</br>
- 3️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
</br>
</br>

## __``Task #3: Roles``__  

- 1️⃣ Please choose one of the following roles in __Cyberville__: 
![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol")
</br>
</br>

- 2️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_C.hex). 
Once downloaded, you can either drag and drop it into a new project.

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

- 3️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
</br>
</br>

## __``Task #4: Pinging``__  

- 1️⃣ Download the ``Code Example`` .hex file (if you haven't already) for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Networking_D.hex). 
    Once downloaded, you can either drag and drop it into a new project.

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```

- 2️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
</br>
</br>
---
# 📌 __*Notes:*__
☑️ Please do not forget to set up the correct name and password for the access point.     
☑️ Mute the PC sound to listen the __b.Board__ sound.    
☑️ If you’d like, you can also view the data going in and out of the b.Board using the __*Show Console Device*__ option.    

        Once you download your code...
- Click on the refresh button 🔄 (circular arrow icon) in the simulator window.
- __Wait__ until *Show console Device* button apears on console output window.
- Click on it.

![Console](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Console.png?raw=true "Console Device")




</br>
</br>

---
#  ⬇️ 📜 *Download JavaScript* </br>
Want to keep this tutorial open while exploring the example code in parallel?
Follow the steps!

__``Task #1: Connecting. ``__</br>
- Click __JavaScript__ in the top menu</br>
- Delete any existing code.</br>
- Paste this code:

        input.onLogoEvent(TouchButtonEvent.Pressed, function () {
            bBoard_WiFi.Disconnect()
            basic.showIcon(IconNames.Sad)
        })
        Cybersec.WifiConnect("Cyberville #?", "")
        if (Cybersec.WiFi_Connected()) {
            basic.showIcon(IconNames.Happy)
        }
 
- Switch back to __Blocks__ view if you prefer.

__``Task #2: MAC and IP address. ``__</br>
- Click __JavaScript__ in the top menu</br>
- Delete any existing code.</br>
- Paste this code:

        input.onButtonPressed(Button.A, function () {
            basic.showString(Cybersec.getMACaddressbBoard())
        })
        input.onButtonPressed(Button.B, function () {
            basic.showString(Cybersec.getIPaddressbBoard())
        })
        Cybersec.WifiConnect("Cyberville #?", "")
        basic.forever(function () {
	
        })
- Switch back to __Blocks__ view if you prefer.

__``Task #3: Roles. ``__</br>
- Click __JavaScript__ in the top menu</br>
- Delete any existing code.</br>
- Paste this code:

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
- Switch back to __Blocks__ view if you prefer.


__``Task #4: Pinging. ``__</br>
- Click __JavaScript__ in the top menu</br>
- Delete any existing code.</br>
- Paste this code:

        input.onButtonPressed(Button.A, function () {
            Cybersec.PingbBfrend("192.168.4.1")
        })
        Cybersec.WifiConnect("Cyberville #?", "")
- Switch back to __Blocks__ view if you prefer.


</br>   
</br>
