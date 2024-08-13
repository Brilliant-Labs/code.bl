# 2_MAC and IP Address
## *Find b.Board MAC and IP Address*

The Media Access Control Address or MAC Address is a 12-digit hexadecimal number assigned to each device connected to the network. The MAC Address is unique. Each b.Board and M5 module in Cyber Security Kit has one.

The IP address is an Internet Protocol number used in networks for devices to share their locations, it is 32 bits long. It can be private or public.
The M5 module will assign an IP address to each b.board on Cyberville because it will be our access point.

As well as the MAC and IP addresses working together in the network, one is identifying while the other is locating.

## Activity

This activity consists of finding the MAC and IP address in each bBoard connected to Cyberville. Students will publish it on a label or Cyberville ID card. Therefore, students can identify these addresses as unique and owned in Cyberville when they make comparisons with each other, and it is useful to recognize them in the network.

Additionally, the teachers and students should publish the MAC and IP addresses on the Cyberville ID  card:

### 🧑‍🏫  __*Teachers ID Card*__
[Download Here](https://www.canva.com/design/DAGJ47YAKtA/2BVp4-fH0NbH9OvPOHU-Jg/view?utm_content=DAGJ47YAKtA&utm_campaign=designshare&utm_medium=link&utm_source=editor)

### 🧑‍🎓 __*Students ID Card*__
[Download Here](https://www.canva.com/design/DAGJ4uZJCmI/VMkcSyZzPpSwA5wGthh2gQ/view?utm_content=DAGJ4uZJCmI&utm_campaign=designshare&utm_medium=link&utm_source=editor)

Example:
<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/ID.png?raw=true" alt="ID" title="ID Example." width="300" />

Let's start!

__1.__ Go to 'https://code-alpha.brilliantlabs.ca/' and create a new project or use the Cyber_Network project created in the previous activity.

__2.__ Within the project, use the on button A pressed block.

__3.__ Replace the "Hello!" text in the show string block with the Get the b.Board´s MAC Address block. it is located under b.Board blocks in CyberSecurity 

![Step3](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step3.png?raw=true "Step3")

__4.__ Add a new block on button A pressed, but this time select on button B pressed.

__5.__ Replace the "Hello!" text in the show string block with the Get the b.Board´s IP Address block. It is located under b.Board blocks in CyberSecurity.

![Step4](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step4.png?raw=true "Step4")

__6.__ Turn on the b.Board and establish communication between the PC, micro:bit and b.Board.

__7.__ Download the code to micro:bit.

__8.__ The student's will now display their unique MAC Address on micro:bit screen pressing button A, and the IP Address pressing button B.

The MAC address will be displayed on Micro:bit display, similar to this (Scrolling ⏪):

       My MAC: 34:ab:95:98:d1:f8

And the IP address will be displayed on Micro:bit display, similar to this (Scrolling ⏪):

       My IP: “192.168.4.2”


***

📌 __*Notes:*__

__*Another Option to see your information:*__
You can also see the MAC and IP address on the __*Show Console Device*__.
╔═══════════════════════════════════╗

*Once you download your code...*
1. Click on the refresh button 	🔄 (circular arrow icon) in the simulator window.
2. __Wait__ until *Show console Device* button apears on console output window.
3. Click on it.

![Step5](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step5.png?raw=true "Step5")
╚═══════════════════════════════════╝

## Code Example

You can __download__ the code for this activity here:
https://alpha.brilliantlabs.ca/documents/cybersec/Cyber-Security-Activity-7B.hex

Or use this code example to obtain the MAC and IP addresses

```blocks
Cybersec.WifiConnect("Cyberville", "")
basic.forever(function () {
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.Disconnect()
    basic.showIcon(IconNames.Sad)
})
input.onButtonPressed(Button.A, function () {
    basic.showString(Cybersec.getMACaddressbBoard())
})
input.onButtonPressed(Button.B, function () {
    basic.showString(Cybersec.getIPaddressbBoard())
})
```