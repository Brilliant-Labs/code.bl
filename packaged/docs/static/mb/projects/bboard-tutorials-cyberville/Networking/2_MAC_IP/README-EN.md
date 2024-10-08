# 2_MAC and IP Address

The Media Access Control Address or MAC Address 🆔 is a 12-digit hexadecimal number assigned to each device connected to the network. The MAC Addres 🆔 is unique. Each b.Board and M5 module in Cyber Security Kit has one.

The IP address is an Internet Protocol 📮 number used in networks for devices to share their locations, it is 32 bits long. It can be private or public.
The M5 module will assign an IP address 📮 to each b.board on __Cyberville__ because it will be our access point.

As well as the MAC 🆔 and IP 📮 addresses working together in the network, one is identifying while the other is locating.

## Activity: 
### Find b.Board MAC 🆔 and IP 📮 Address

This activity consists of finding the MAC and IP address in each b.Board connected to __Cyberville__. Students will publish it on a label or __Cyberville__ ID card. Therefore, students 🧑‍🎓 can identify these addresses as unique and owned in __Cyberville__ when they make comparisons with each other, and it is useful to recognize them in the network.

Additionally, the teachers 🧑‍🏫 and students 🧑‍🎓 should publish the MAC and IP addresses on the __Cyberville__ ID  card:

### 🧑‍🏫  __*Teachers ID Card*__
Download the ID Card for Teachers 🧑‍🏫 [Here](https://drive.google.com/file/d/14gh8mT6u4rgxHwiSSV6rtSel3Gz4WwM_/view?usp=drive_link)

### 🧑‍🎓 __*Students ID Card*__
Download the ID Card for Students 🧑‍🎓 [Here](https://drive.google.com/file/d/1uYi49zPMzKYuliF4TlS2NQBoPTkMTcoD/view?usp=drive_link)

This is an example what to expect for this activity:  

<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Example_EN.png?raw=true" alt="ID" title="ID Example." width="300" />
  

*Let's start!*

__1.__ Go to 'https://code-alpha.brilliantlabs.ca/' and create a new project or use the Cyber_Network project created in the previous activity.

__2.__ Within the project, use the on button A pressed block.

__3.__ Replace the "Hello!" text in the show string block with the Get the b.Board´s MAC Address block. it is located under b.Board blocks in CyberSecurity 

![Step5](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step5.png?raw=true "Step 3")

__4.__ Add a new block on button A pressed, but this time select on button B pressed.

__5.__ Replace the "Hello!" text in the show string block with the Get the b.Board´s IP Address block. It is located under b.Board blocks in CyberSecurity.

![Step6](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step6.png?raw=true "Step 5")

__6.__ Turn on the b.Board and establish communication between the PC, micro:bit and b.Board.

![Step7](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step7.png?raw=true "Download to microbit")

__7.__ Download the code to Microbit.

__8.__ The student's will now display their unique MAC Address 🆔 on Microbit screen pressing button A, and the IP Address 📮 pressing button B.

The MAC address 🆔 will be displayed on Microbit display, similar to this (Scrolling ⏪):

       My MAC: 34:ab:95:98:d1:f8

And the IP address 📮 will be displayed on Microbit display, similar to this (Scrolling ⏪):

       My IP: “192.168.4.2”

__9.__ Ultimately, 🧑‍🏫 teachers should inquire of their 🧑‍🎓 students why the 🆔 MAC and 📮 IP addresses are crucial for cybersecurity and the development of __Cyberville__.

***

📌 __*Notes:*__

__*Another Option to see your information:*__
You can also see the MAC and IP address on the __*Show Console Device*__.

### ~ avatar
*Once you download your code...*
1. Click on the refresh button 	🔄 (circular arrow icon) in the simulator window.
2. __Wait__ until *Show console Device* button apears on console output window.
3. Click on it.

![Console](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Console.png?raw=true "Console Device")
### ~


## Code Example

You can download the code for this activity from `https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex` the file will be in Recent Download History, just drag and drop it into a new project.  

Or use this code example to obtain the MAC 🆔 and IP 📮 addresses.

__*Please do not forget to set up the correct name for the access point. Mute the PC sound to listen the b.Board sound.*__

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