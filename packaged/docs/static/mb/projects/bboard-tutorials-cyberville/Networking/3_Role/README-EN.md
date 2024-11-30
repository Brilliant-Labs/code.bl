
---
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝**Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
---

# 3_Roles

In this activity you will take on a role in Cyberville so that you can protect it from Cyber Attacks.

## Activity:
### Take a role in The Cyberville

*Let's start!*

__1.__ Fill out your __Cyberville ID__ Card with names, MAC addresses 🆔, and IP addresses 📮.

__2.__ Acquire an identity by choosing a role within __Cyberville__.

__3.__ Program the micro:bit so your icon is always displayed on the micro:bit screen to indicate that you are connected to the __Cyberville__ Wi-Fi network.

__4.__ Program the micro:bit to play a sound or a melody (You can find this in the music blocks) if you are not connected to the __Cyberville__ WiFi network.

Please choose one of the following roles in __Cyberville__: 
![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol")

As an example, if you chose __WATER__ and are connected to the WiFi Network, then your micro:bit should look like this:

![Step10](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Step10.png?raw=true "Step10")

Once you've successfully linked each __b.Board__ in the classroom to __Cyberville__ and assigned it a role, it's time for the fun part! Your teacher will simulate a __Cyber Attack__ by disabling the M5 module, which is the WiFi provider for __Cyberville__. This will disconnect all the devices in __Cyberville__, creating a situation of chaos within the __Cyberville__ network!

## Code Example
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_C.hex). 
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")

_**`Please do not forget to set up the correct name and password for the access point.Mute the PC sound to listen the __b.Board__ sound.`**_

You can use this code example to have a __Role 👤__ in __Cyberville__, please change the WETER-Umbrella for your own role.

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