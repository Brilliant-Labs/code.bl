
---
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝**Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
---

# 2_MAC and IP Address

The Media Access Control (MAC) Address 🆔 is a 12-digit hexadecimal number assigned to each device connected to a network. It appears in the following format:
### 34:ab:95:98:d1
The MAC Address 🆔 is unique; every computer, phone, tablet, __b.Board__, or electronic device connected to any network has its own MAC address 🆔.

The IP Address is an Internet Protocol 📮 number used for devices to communicate with each other over networks. It serves as a way to share their locations for data transmission. An IP address is 32 bits long and typically looks like this:
### 192.168.4.2
It can be either private or public.
The M5 module will assign an IP address 📮 to each __b.Board__ in __Cyberville__, as it will serve as our access point 📳.

MAC 🆔 and IP 📮 addresses work together within a network. The MAC Address 🆔 enables device identification, while the IP Address 📮 provides the location necessary for sending and receiving data.

## Activity: 
### Find the b.Board's MAC 🆔 and IP 📮 Address

This activity consists of finding the MAC 🆔 and IP address 📮 for each __b.Board__. Students will publish it on a label or __Cyberville__ ID card. Therefore, students 🧑‍🎓 can identify these addresses as unique and owned in __Cyberville__ when they make comparisons with each other, and it is useful to recognize them in the network.

Additionally, the teachers 🧑‍🏫 and students 🧑‍🎓 should publish the MAC and IP addresses on the __Cyberville__ ID  card:

### 🧑‍🏫  __*Teachers ID Card*__
Download the ID Card for Teachers 🧑‍🏫 [__⬇️ Here__](https://drive.google.com/file/d/14gh8mT6u4rgxHwiSSV6rtSel3Gz4WwM_/view?usp=drive_link)

### 🧑‍🎓 __*Students ID Card*__
Download the ID Card for Students 🧑‍🎓 [__⬇️ Here__](https://drive.google.com/file/d/1uYi49zPMzKYuliF4TlS2NQBoPTkMTcoD/view?usp=drive_link)

This is an example of what to expect for this activity: 
<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Example_EN.png?raw=true" alt="ID" title="ID Example." width="300" />
![ID Example](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Example_EN.png?raw=true "ID Example")  

*Let's start!*

__1.__ Go to https://code-alpha.brilliantlabs.ca/ and create a new project or use the Cyber_Network project created in the previous activity.

__2.__ Within the project, use the 🧩 ``||on button A pressed||`` block.

__3.__ Replace the “Hello!” text in the 🧩 ``||show string||`` block with the 🧩 ``||Get the b.Board´s MAC Address||`` block. This is located under "b.Board blocks" in "CyberSecurity".

![Step5](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step5.png?raw=true "Step 3")

__4.__ Add a new 🧩 ``||on button A pressed||`` block, however this time select "on button B pressed".

__5.__ Replace the “Hello!” text in the 🧩 ``||show string||`` block with the 🧩 ``||Get the bBoard´s IP Address||`` block. This is located under "b.Board blocks" in "CyberSecurity".

![Step6](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step6.png?raw=true "Step 5")

__6.__ Turn on the __b.Board__ and establish communication between the PC, micro:bit and __b.Board__.

![Step7](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step7.png?raw=true "Download to microbit")

__7.__ ⬇️ Download the code to micro:bit.

__8.__ The student's will now display their unique MAC Address 🆔 on micro:bit screen pressing A button, and the IP Address 📮 pressing B button.

The MAC address 🆔 will be displayed on micro:bit display, similar to this (Scrolling ⏪):  
__`My MAC: 34:ab:95:98:d1:f8`__      
And the IP address 📮 will be displayed on Microbit display, similar to this (Scrolling ⏪):  
__`My IP: 192.168.4.2`__
       
__9.__ At the end of this activity 🧑‍🏫 teachers should talk with their 🧑‍🎓 students about why 🆔 MAC and 📮 IP addresses are crucial for cybersecurity and the development of __Cyberville__.

***

📌 __*Notes:*__

If you would like, you can also see the 🆔 MAC and 📮 IP address on the __*Show Console Device*__.

### ~ avatar
*Once you download your code...*
1. Click on the refresh button 🔄 (circular arrow icon) in the simulator window.
2. __Wait__ until *Show console Device* button apears on console output window.
3. Click on it.

![Console](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Console.png?raw=true "Console Device")
### ~

## Code Example
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex). 
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")

_**`Please do not forget to set up the correct name and password for the access point. Mute the PC sound to listen the b.Board sound.`**_

You can use this code example to obtain the 🆔 MAC and 📮 IP addresses.

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