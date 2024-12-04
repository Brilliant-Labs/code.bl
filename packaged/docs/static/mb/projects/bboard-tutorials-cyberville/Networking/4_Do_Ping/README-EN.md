<!--
---
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝 **Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
---
-->
# 4_PINGING

Now that the __Cyberville__ network is up and running and everyone's roles are filled, it's time to find out if there's someone special in the network. To do that, we're going to use the command "__ping__."

A __"ping"__ is a simple Internet program that lets you test and verify if a particular destination __IP__ address exists and can accept requests in the __Cyberville__ network. It's really easy to use! Another great thing about __ping__ is that it lets you know if another __b.Board__ is trying to reach you and that it's working properly.
Let's use the __"ping"__ command to find out if other roles are in the __Cyberville__ network! 

## Activity
Let's quickly check if the access point 📳 M5 Module is available. Just do a __Ping__, and we'll know in no time! It has a handy default IP address of 192.168.4.1, which is perfect for getting started using the command PING! 
It would be really fun to share our ID cards and find out who our classmates are connected to! Don't forget to set up your friends' IP addresses in the block 🧩 ``||Do PING to IP("")||``, and make sure you're connected to the right access point 📳.
You'll get a 😊 smiley face if your request role is available in the network, and a 😔 sad face if it's not.

## Code Example
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_D.hex).
<!--
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")
-->
_**`Please do not forget to set up the correct name and password for the access point. Mute the PC sound to listen the __b.Board__ sound.`**_

You can use this code example to __pinging__ your friends.

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```