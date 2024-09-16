# 3_Roles. 

To complete this activity you must acquire a role in Cyberville so that you can protect it from Cyber Attacks.

## Activity:
### Take a role in The Cyberville

*Let's start!*

__1.__ Fill out your __Cyberville ID__ Card with names, MAC addresses 🆔, and IP addresses 📮.

__2.__ Acquire an identity by choosing a role within __Cyberville__.

__3.__ Develop a code where your icon is always displayed on the micro:bit screen to indicate that you are connected to Wi-Fi in __Cyberville__.

__4.__ Program the Microbit to play sound or  start melody (You can find it in music blocks) if you are not connected in __Cyberville__.

Remember, your role in __Cyberville__ could be one of those important entities. 
![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol")

It should look like this for someone who chooses __WATER__, and it is connected.

![Step10](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Step10.png?raw=true "Step10")

Once you've successfully linked each b.Board in the classroom to __Cyberville__ and assigned it a role, it's time for the fun part! Your teacher will simulate a __Cyber Attack__ by disabling the M5 module, which is the WiFi provider for __Cyberville__. This will disconnect all the devices in __Cyberville__, creating a situation of chaos and general fall in the __Cyberville__ network!

## Code Example

You can download the code for this activity from `https://www.brilliantlabs.ca/documents/cybersec/Networking_C.hex` the file will be in Recent Download History, just drag and drop it into a new project.  

Or use this code example to know if you have and __active role 👤__ in __Cyberville__.

__*Please do not forget to set up the correct name for the access point. Mute the PC sound to listen the b.Board sound.*__

Or use this code example to set up your role 👤.

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