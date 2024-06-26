# 3_Roles. *Take a role in Cyberville*

To complete this activity "Take a role in Cyberville", you need to belong to Cyberville to protect it from cyber attacks adquiring a role.

## Activity
Let's start!

__1.__ Fill out your Cyberville ID Card with names, MAC addresses, and IP addresses.

__2.__ Acquire an identity by choosing a role within Cyberville.

__3.__ Develop a code where your icon is always displayed on the micro:bit screen to indicate that you are connected to Wi-Fi in Cyberville.

__4.__ Program the micro:bit to play sound or  start melody (You can find it in music blocks) if you are not connected in Cyberville.

Remember, your role in Cyberville could be one of those important entities. 
![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol")

It should look like this for someone who chooses WATER, and it is connected..

![Step6](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Step6.png?raw=true "Step6")

Once you've successfully linked each b.Board in the classroom to Cyberville and assigned it a role, it's time for the fun part! Your teacher will simulate a __Cyber Attack__ by disabling the M5 module, which is the WiFi provider for Cyberville. This will disconnect all the devices in Cyberville, creating a situation of chaos and general fall in the Cyberville network!

## Code Example

You can __download__ the code for this activity here:
https://alpha.brilliantlabs.ca/documents/cybersec/Cyber-Security-Activity-7C.hex

Or use this code example to set up your role.

```blocks
Cybersec.WifiConnect("Cyberville", "")
basic.forever(function () {
    if (Cybersec.WiFi_Connected()) {
        basic.showIcon(IconNames.Square)
    } else {
        soundExpression.sad.play()
        basic.showIcon(IconNames.Sad)
    }
})
input.onButtonPressed(Button.A, function () {
    basic.showString(Cybersec.getMACaddressbBoard())
})
input.onButtonPressed(Button.B, function () {
    basic.showString(Cybersec.getIPaddressbBoard())
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.Disconnect()
    basic.showIcon(IconNames.Sad)
})
```