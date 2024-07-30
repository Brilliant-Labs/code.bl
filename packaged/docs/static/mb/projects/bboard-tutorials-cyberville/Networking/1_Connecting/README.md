# 1_Connecting

  It's time to connect to the WiFi Cyberville. Cyberville is a cool representation of a futuristicville developed by the awesome folks at Brilliant Labs. In this Cyberville, all clients or b.Boards are connected to the WiFi Cyberville network. The WiFi service on Cyberville is provided by the M5Core2 module, which will create the WiFi Access Point called Cyberville #?. Let´s connect us to belong to Cyberville!.  
## Activity
Let's start!   
__1.__ Go to `https://code-alpha.brilliantlabs.ca/` and create a new project using micro:bit V2,  naming it Cyber_Network.

![Step1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step1.png?raw=true "Step1")  

__2.__ Within the project, use the On Start block and place it inside the Connect to WiFi: ( ) with Password ( ) block.

__3.__ Set up the right WiFi name. For example: Cyberville. Don't use a password for this activity.

####  Access Point Name - Cyberville Number
Note that __we will not use a password__ for this activity, as the Cyberville number will change each time you restart the M5Core2.
![CybervilleNumb](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/CybervilleNumb.png?raw=true "Cyberville Number for Access Point")

__4.__ Create another block to disconnect from the network. You can use On logo Presed

![Step2](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step2.png?raw=true "Step2")

__5.__ Turn on the b.Board and establish communication between the PC, micro:bit and b.Board.

If you get a ✅, you are connected to Access Point.  

<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true" alt="Connected_gif" title="If you get a ✅, you are connected to Access Point" width="300" />

__6.__ Download the code and check the connection and disconnection code with the M5Core2 module WiFi access point.

Students will see smile face if they are connected.
![Connected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected.png?raw=true "Connected")

or a sad face if they are not.
Students will see smile face if they are connected.
![Disconnected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Disconnected.png?raw=true "Disconnected")

## Code Example

You can __download__ the code for this activity [here](https://alpha.brilliantlabs.ca/documents/cybersec/Cyber-Security-Activity-7A.hex).

Or use this code example is to connect the b.Board to M5Core2.

```blocks
Cybersec.WifiConnect("Cyberville", "")
basic.forever(function () {
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.Disconnect()
    basic.showIcon(IconNames.Sad)
})
```