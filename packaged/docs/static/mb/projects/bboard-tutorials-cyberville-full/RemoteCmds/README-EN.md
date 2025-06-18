# ACTIVITY 9
# REMOTE COMMANDS 

---
##### ~avatar
Intro video about Cybersecurity Level 2 and __Cyberville__
https://www.youtube.com/watch?v=aapUlOM0EAo
##### ~
### [⎆ Go to Tasks](#remote-commands-tasks)
---
</br>
Welcome to __Activity 9: Remote Commands!__ This activity takes place within the framework of __Mission Fake Parking ID__, where you'll learn the three main principles of cybersecurity, known as the CIA Triad! The __CIA Triad__ stands for Confidentiality, Integrity, and Availability. These three pillars are the foundation of keeping information safe.
When using __remote commands__, vulnerabilities can arise due to weak security measures, improper authentication, or lack of encryption. Some key risks could be: unsecured communication, weak authentication, command injection, privilege escalation,replay attacks, and denial of Service.
In __Mission Fake Parking ID__, your challenge will be to control a parking barrier __remotely__ and establish a robust way to keep your data safe, reducing the risk of it being stolen even using remote commands. To succeed, you must complete various tasks and solve different tasks.

Here we have some tips about __CIA Triad__

![CIA_Fox](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/RemoteCmds/CIA_Fox.png?raw=true "CIA_Fox")

##### ~avatar
__🤫 Confidenciality__  

• To Remember 🤔  
    Only the right people should be able to see important information.

• To Prevent ⚠️  
    Keep information safe so only the right people can see it.

• To Protect 🔰  
    ✔︎ Two factor authentication  
    ✔︎ Access control  
    ✔︎ Cryptography  
##### ~

##### ~avatar
__🤝 Integrity__  

• To Remember 🤔  
    Information should always be correct and not changed in a sneaky way.  

• To Prevent ⚠️  
    Make sure information stays correct and isn’t secretly changed.  

• To Protect 🔰  
    ✔︎ Hashing  
    ✔︎ Digital signatures  
    ✔︎ Keys  
##### ~

##### ~avatar
__🗓️ Availability__  

• To Remember 🤔  
    Information should be ready and easy to get when you need it!  

• To Prevent ⚠️  
    Keep information available so it can always be used, even if something goes wrong!  
    
• To Protect 🔰  
    ✔︎ Backup  
    ✔︎ Redundancy  
    ✔︎ Fault tolerance  
##### ~

![Mission_3](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/RemoteCmds/Parking_Pases.gif?raw=true "Mission 3")

## Activity Description
In __Cyberville__ there is a 🏢 government building 5️⃣ with many services to the population.  In one of their department, citizens with some physical disabilities can obtain a free parking pass to park their cars in a reserved parking zone when they move across the city.  This parking pass can’t be used by all citizens who must pay their parking fees when necessary.  Recently, several __fake Parking Passes and IDs__ were spotted by a couple of parking attendants.  The passes were used by people who shouldn’t have received a parking pass.  The police were informed and they discovered that there was a scam to sell fake parking passes.  They suspect someone working in the government building but have yet to discover who it is.

Your mission is to discover how someone inside or outside the government building has access to the network and how to prevent this scam from happening. You must evaluate how strong your cybersecurity is and apply the CIA triad to achieve success. You will need to complete a Cybersecurity Assessment Report and share it with government officials and the police.

For this activity, you will design a parking access control system using two __b.Boards__. You will work in pairs, with one __b.Board__ managing a barrier that grants access to individuals with physical disabilities who possess a free parking pass ID in __Cyberville 🏢 Goverment building__. The second __b.Board__ will __REMOTELY CONTROL ACCESS__ through the __Cyberville__ Wi-Fi access point provided by the 📳 M5 module.
This task is divided into three parts, following the principles of the CIA Triad in cybersecurity: Confidentiality, integrity, and Availability.
For this Mission 3, you will need the 🎫 ID card from the Networking activity, along with an understanding of IP addresses and Access Points. It is strongly recommended that you review the concepts covered in 🔵 🎩 Blue Hat and explore the importance of signal strength in the Valuable Data activity.
Additionally, you will need a servo motor to construct the parking control barrier. Here is an example:

![ParkingBar](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/RemoteCmds/ParkingBar.png?raw=true "ParkingBar")

It's a great way to show off your skills and help protect the Parking Lot __🏢 Government Building__ from getting scammed and keep the information safe.
__*Have fun!*__
---
---
# REMOTE COMMANDS TASKS

## - [1. CONFIDENTIALITY](#confidentiality) 
## - [2. INTEGRITY](#integrity) 
## - [3. AVAILABILITY](#availability) 
---
## CONFIDENTIALITY
![Confidentiality-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/1_Confidentiality/Confidentiality-EN.png?raw=true "Confidentiality-EN") 
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝 **Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
</br>
Do you want to keep a secret safe? 🤫 Then __confidentiality__ is the best place to start! It’s like having a top-secret vault where only the people you trust and give permission (like your best friend… maybe 😉) can access the information.

🕵️‍♂️ But What If a Sneaky Snoop Tries to Peek?
Hackers (a.k.a. digital troublemakers) are always looking for ways to sneak into your private information. They might try to: 🔑 Guess your password, 🕶️ Steal secret codes, 🤥 Trick you into giving them access.
But don’t worry! Good cybersecurity helps keep them out and protects your secrets! 💪

Oh no! The 🏢 Government Parking Lot is under cyber attack! Someone created fake ID passes, which means the parking lot lost its Confidentiality. In this task, we’ll dive deeper into __Confidentiality__ and learn how to protect our information just like the 🏢 Government Parking Lot should have!

There are several ways in which we can protect your privacy (Confidentiality), and here are a few of them:
- Passwords & Locks 🔑 – Computers use passwords to keep information safe.
- Secret Codes (Encryption) 🔐 – Even if someone gets in, they’ll just see a bunch of jumbled-up nonsense unless they have the secret key!
- Security Guards (Firewalls & Antivirus) 🛡️ – They act like bodyguards, keeping the bad guys away.
- Multi-factor authentication (or 2FA) ⛓️ - Require two or more pieces of evidence to access.
- Access control (Approval) 🛂 - Enable to manage who is autorized to access adata and resources.

---

### TASK 1: Confidentiality
Let's start! 

This __Confidentiality__ task is divided into two parts, where we’ll explore how to protect our information using key cybersecurity concepts like 🔑 Passwords, 🔐 Encryption, and 🪪 Multifactor Authentication (MFA) or Two Factor Authentication.

In the first part, 🧑‍🎓 students will connect to Cyberville’s 📳 network, find their assigned 📮 IP addresses, and complete their Cyberville 🎫 ID cards. In the second part, they’ll randomly draw a secret 🎟️ ID ticket from a bag and use their coding skills to find a classmate with the matching identification code and second authentication factor (MFA). Get ready to learn, connect, and have fun! 🤫.  

---
#### __Part One: Connecting...__
##### __🧑‍🏫 Teachers:__
For __Mission Fake Parking ID__ Please follow the next steps that you will find on 📳 M5 module:

__1.__ Load __Mission Fake Parking ID__ into 📳 M5 module. You can see this [__🎬 video__](https://www.canva.com/design/DAGJhm69_Mk/JdN1bb74mN-bKiclzST5Ag/watch?utm_content=DAGJhm69_Mk&utm_campaign=designshare&utm_medium=link&utm_source=editor) if you want to remember how to do it.

__2.__ Press the first button __GO!!!__, then guide the 🧑‍🎓 students for the activity. 

![M5Act9](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/RemoteCmds/1_Confidentiality/M5Act9.png?raw=true "M5Act9")  

__3.__ Share the current __Access Point name__ created by the  📳 M5 module with the classroom and the password if it is the case. For example:  AP name 📳: __Cyberville #1__ 

__4.__ In order to involve the student in the __Confidentialy__ concept, 🧑‍🏫 theachers need to setup a 🔑 Password. Remember that there are three differents ways to setup passwords on 📳 M5 module for __Cyberville__ network it was shown on __Activity 7 Task Connecting__.

__5.__ Once the password is set by the 🧑‍🏫 teacher, for example:
Password 🔑: __BL_Cybr1__ *(if you are using default one)* 
must find the way to __*securely share*__ the Password  with the  🧑‍🎓 students doing a __broken phone game__ or __Encryption game__ like this: [__👉 Encryption Game__](https://drive.google.com/file/d/1KjibW5lbxdzsJBPX9-FPsGgk9ciXYbkl/view?usp=sharing)

---
##### 🧑‍🎓 __Students:__
__1.__ Students should the steps in __Activity 7 Task Connecting__, but add the __Password__ that 🧑‍🏫 teacher should share in a __secure__ and __confidential__ way. 

![Set_Psw](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/1_Setting_Pws/SetPsw.png?raw=true "Set_Psw")
Just a quick note to ask that you please __make sure that b.Board is connected__. 
![Connected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true "Connected")
If you get a ✅, you are connected to Access Point 📳.

__2.__ It is crucial for the students to know the 📮 IP address of the __b.Board__ in order to succeed in this Mission Fake Parking ID, the students must fill out the ID card again, but in this case only with the name and IP address. Remember that you can download and print the ID card from these links [__👉 Here__](https://drive.google.com/file/d/1uYi49zPMzKYuliF4TlS2NQBoPTkMTcoD/view?usp=drive_link)

For this first part of the task, this should be a good example of how to fill out the Cyberville ID card.
![Example](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/RemoteCmds/1_Confidentiality/Example_M3.jpg?raw=true "Example")

---
#### __Part Two: Matching...__
##### __🧑‍🏫 Teachers:__
Teachers will print pairs of tickets from [__⬇️ here__](https://drive.google.com/file/d/19U47aArl-HJ-QXbhx-lrOQb27WTFAI0G/view?usp=sharing), as shown below. Each ticket contains the same Authentication Code and Multifactor Code. These tickets are confidential for each b.Board in the classroom. The teacher will place all secret 🎟️ ID tickets into a bag so that students can randomly draw one. Teachers must ensure that students do not share this information with anyone.

##### __ 🎟️ Tickets__
![Match](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/RemoteCmds/1_Confidentiality/Match.png?raw=true "Match")

🧑‍🏫 Teachers will see the clients connected to the Cyberville network on the  📳 M5 module screen. This allows them to share the available 📮 IP addresses with 🧑‍🎓 students, helping them identify their potential partners for matching.

![Clients](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/RemoteCmds/1_Confidentiality/Clients.png?raw=true "Clients")

---

##### __🧑‍🎓 Students:__
__1.__ Once the students are connected to the __Cyberville__ network and have their 🎟️ ID secret tickets, they must be able to hear messages from the network using the 🧩 block ``||set to hear any MSG||``. They will see a "hi" word on the micro:bit screen, which means they are ready to listen to you through the __Cyberville__ network in a public way. The messages go and back will be published to the Window Console Device.

__2.__ Students will send a welcome message to ALL! in the network using the 🧩 block ``||Send Public Message||``, be aware that this message is __NOT CONFIDENTIAL__. Keep an eye on the Window Console Device to see the information is being published on the __Cyberville__ network.

__3.__ Students will create a table listing the roles of all 📮 IP addresses in the network. Like this:

| Role 👤  | Icon  | Entity's name| IP Address  |
| :------------------   | :---: | :--------------------- | :------------------|
|    1️⃣ School           |🏫| `Lincoln School`           | 192.168.-----.-----
|    2️⃣ Hospital         |🏥| `Hospital Cyberville`      | 192.168.-----.-----
|    3️⃣ Water            |💧| `AquaPure`                 | 192.168.-----.-----
|    5️⃣ Government       |🏢| `Cyberville Gov.Services`  | 192.168.-----.-----
|    6️⃣ Brilliant Labs   |🏩| `Brilliant Labs`           | 192.168.-----.-----
|    7️⃣ Bank             |🏦| `Pacific Bank`             | 192.168.-----.-----
|    8️⃣ Factory          |🏭| `Volt Motors`              | 192.168.-----.-----
|    9️⃣ Industry         |🏪| `Techmach Industries`      | 192.168.-----.-----
|    1️⃣0️⃣ Art Center     |🎨| `Harmony Art Center`       | 192.168.-----.-----
|    1️⃣2️⃣ Citizens       |😎| `The Cyberville community` | 192.168.-----.-----
<br>
__4.__ Once the listing table is done. they must send a __CONFIDENTIAL__ (private) message to each 📮 IP on the network using the 🧩 block ``||Send Private Message||`` asking for a partner with the same Autentication Code.

__5.__ Students with the same code, for example: __QSX1__. They will send a message back to doble ckeck sending a __CONFIDENTIAL__ mesage with their Two Factor Authentication or MFA, for example: ZS3E.

__6.__ If they have the same Authentication code and the MFA they are __*MATCH! 🤝*__

This is the end of the task. Well done!!!😎👍
---

### ``|>_|`` Code Example:
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://brilliantlabs.ca/documents/cybersec/Confidentiality.hex). Once downloaded, either drag and drop it into a new project. 
You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```javascript
input.onButtonPressed(Button.A, function () {
    Cybersec.MSG_UPD_SndtoAll(Cybersec.blixel_indexR(BLiXelIndexR.one), "Hello everyone!")
})
input.onButtonPressed(Button.B, function () {
    Cybersec.TXT_UPD_Snd("Just between us...", "192.168.4.?")
})
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
```
<!--
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")
-->
Or use this code as example in a __New Projet__. You can use this code example to connect to __Cyberville__ network, send a __Public__ message to everyone and send a __Confidential__ message to a specific 📮 IP address.
```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.MSG_UPD_SndtoAll(Cybersec.blixel_indexR(BLiXelIndexR.one), "Hello everyone!")
})
input.onButtonPressed(Button.B, function () {
    Cybersec.TXT_UPD_Snd("Just between us...", "192.168.4.?")
})
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
```

### ~ avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
### [[🔙 Back Tasks](#remote-commands-tasks)] | [[⏮️ Back Remote Commands](#remote-commands)]  
---
---
## INTEGRITY
![Integrity-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/2_Integrity/Integrity-EN.png?raw=true "Integrity-EN") 
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝 **Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
</br>
Imagine you write a letter to your friend, sharing a secret plan for a game. Now, imagine someone changes your letter before it reaches them. Instead of saying, "Let's meet at 3 PM," they change it to "Let's meet at 5 PM." That would cause confusion, right?

__🤝 Integrity__ in cybersecurity ensures that information remains correct and unchanged unless authorized individuals update it.

Examples of __🤝 Integrity__
- Homework Online 📚 – If you submit homework on a school website, __Integrity__ means no one can change your answers after you upload them.
- Bank Account 💰 – If you have $100 in your account, __Integrity__ ensures that no one can change it to $50 without permission.
- Gaming Scores 🎮 – If you get a high score in a game, __Integrity__ makes sure no one cheats and changes your score.  
For this task, we must ensure that the parking control barrier for a 🏢 government building is not altered and that its position displayed on the remote device is reliable. This is an example of __Integrity__.  

🛠️ How Do We Protect __Integrity__?  
- Passwords 🔑 – Only the right people should be able to change information.
- Backups 📂 – If something gets changed by accident, we can restore the original version.
- Checksums & Hashing 🔢 – Computers use special codes to check if data has been changed.

---

### TASK 2: Integrity

Let's get started!

This __Integrity__ task involves sharing information between two b.Boards. The *Control b.Board* will have buttons to ⬆️ raise and ⬇️ lower the barrier remotely, while the *Device b.Board* will be attached to a servomotor that controls the barrier's movement. For this task, you will need to work in pairs of b.Boards. We recommend collaborating with your match partner from Task 1, __Confidentiality__.

The *Control b.Board* will also display the barrier's position on its micro:bit screen as part of the __Integrity__ concept.

This __Integrity__ task is divided into two parts:

1. Controlling a parking access barrier 🚥 Locally - For each b.Board team.
2. Controlling a parking access barrier 🚥 Remotely - For matched pairs b.Boards.

---
#### __Part One:__
##### __Controlling a parking access barrier 🚥 Locally...__

Each team will program a b.Board to control a servomotor locally to understand how it functions. 🧑‍🎓 Students can use the following code to operate a parking access barrier 🚥 (servomotor) in a 🏢 Government parking area:

### ``|>_|`` Code Example Controling Access Barrier 🚥:  
You can download the .hex file for this task by clicking [⬇️ Here](https://brilliantlabs.ca/documents/cybersec/Integrity-Local.hex). Once downloaded, either drag and drop it into a new project. 

```javascript
input.onButtonPressed(Button.A, function () {
    Cybersec.increase()
})
input.onButtonPressed(Button.AB, function () {
    Cybersec.closebar()
})
input.onButtonPressed(Button.B, function () {
    Cybersec.decrease()
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.openbar()
})
Cybersec.Localparkbar()
basic.forever(function () {
    servos.P00.setAngle(Cybersec.getValueDeg())
})
```
---
#### __Part Two:__
__Controlling a parking access barrier 🚥 Remotely...__
In this part of the task, 🧑‍🎓 students are encouraged to control the barrier by sending commands remotely from the *Control* to the *Barrier*.

#### __🧑‍🏫 Teachers:__
For __Integrity__ task in the frame from __Mission Fake Parking ID__ please follow the same steps for __Confidential__ task, in order to provide the 📳 access point name and password to the 🧑‍🎓 students.

---
#### __🧑‍🎓 Students:__
__1.__ Students should follow the steps in the __Confidential__ task to obtain their own 📮 IP address as well as their matched partner’s 📮 IP address.

__2.__ Once the matched teams are connected, they are ready to __Send Commands Remotely__ and control the parking access barrier 🚥. One team with a b.Board should act as the *Control Remotely*, while the matched partner should act as the *Barrier Remotely*.


### ``|>_|`` Code Example:
You can download the .hex file for this task by clicking [__⬇️ Here *Control*__](https://brilliantlabs.ca/documents/cybersec/Integrity_Control_Remotely.hex). Once downloaded, either drag and drop it into a new project. 
You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so.
Agree with your match partner wich the side your are going to be part, *Control B.Board* or *Device b.Board*

##### ``|>_|`` *Control Remotely*

```javascript
input.onButtonPressed(Button.A, function () {
    Cybersec.increase()
})
input.onButtonPressed(Button.AB, function () {
    Cybersec.closebar()
})
input.onButtonPressed(Button.B, function () {
    Cybersec.decrease()
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.openbar()
})
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
Cybersec.Localparkbar()
basic.forever(function () {
    servos.P00.setAngle(Cybersec.getValueDeg())
    Cybersec.Num_UDP_Snd(Cybersec.getValueDeg(), "192.168.4.?")
})
```
```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.increase()
})
input.onButtonPressed(Button.AB, function () {
    Cybersec.closebar()
})
input.onButtonPressed(Button.B, function () {
    Cybersec.decrease()
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.openbar()
})
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
Cybersec.Localparkbar()
basic.forever(function () {
    servos.P00.setAngle(Cybersec.getValueDeg())
    Cybersec.Num_UDP_Snd(Cybersec.getValueDeg(), "192.168.4.?")
})
```


##### ``|>_|`` *Barrier Remotely*
You can download the .hex file for this task by clicking [__⬇️ Here *Barrier*__](https://brilliantlabs.ca/documents/cybersec/Integrity_Barrier_Remotely.hex). Once downloaded, either drag and drop it into a new project.

```javascript
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
```

```blocks
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
```

<!--
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")
-->

---
- *Please do not forget to set up the correct name and password for the access point.*
- *Mute the PC sound to listen the b.Board sound.*
---

### ~ avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
### [[🔙 Back Tasks](#remote-commands-tasks)] | [[⏮️ Back Remote Commands](#remote-commands)]  
---
---

## AVAILABILITY
![Availability-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/3_Availability/Availability-EN.png?raw=true "Availability-EN") 
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝 **Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
</br>
Imagine you have a favorite online game that you love playing with your friends. One day, you try to log in, but the game won’t load! 😟 That’s because the game’s servers are down, or maybe too many people are trying to play at the same time. This is an example of a problem with Availability 🚧 in cybersecurity.

What is Availability?
🚧 Availability means that information and computer systems should always be ready and accessible whenever we need them. Just like a school needs to be open for students to learn, websites, apps, and online services need to be available for people to use.

Why is Availability Important?
Without Availability, we wouldn’t be able to:
 ✅ Send messages to friends 📩
 ✅ Watch videos online 🎥
 ✅ Use learning websites for homework 📚
 ✅ Play multiplayer games 🎮

What Can Go Wrong?
Sometimes, hackers or technical problems can stop a website or service from working. Here’s how:
Too much traffic (like when too many people try to buy concert tickets at once, and the website crashes).
Cyberattacks (like DDoS attacks, where bad people send too much fake traffic to a website, making it stop working).
Power failures (if a server loses electricity, it can’t keep a website running).

How Do We Protect Availability?
To keep websites and services available, cybersecurity experts use:
 🔹 Backup servers – extra computers that take over if one fails.
 🔹 Load balancing – spreading out the work so no single computer gets overloaded.
 🔹 Cyberattack defenses – firewalls and security systems to stop bad traffic.

### TASK 3: Availability
This task is actually a fun game! In cybersecurity, Availability means making sure computers, websites, and data are always working and ready when people need them.

In the Cyberville Mission: Fake Parking ID environment, Availability is like being able to enter a parking lot. When the barrier is open, you can get in—everything is available. But once the barrier closes, access is no longer available!

The time the barrier stays open is set by the user. This can be done on the spot (locally) or by using Remote Commands.
So, start the timer and run as fast as you can before the barrier closes and access is gone. 
Have fun!

Let's get started!
We've made it really easy for you to recreate the awesome environment from Mission Fake Parking ID while learning about cybersecurity. All you have to do is:
1. Download [__👉 Here__](https://drive.google.com/file/d/1lYtZyyQ5f7qhXzua5LGw7-LFFzpQwcW4/view?usp=sharing) print and cover the b.Board for Mission Fake Parking ID.
![Availability](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/3_Availability/Availability.png?raw=true "Availability")
2. Connect the servomortor to P0, it will be your barrer control.
3. Code or download the game.
4. Play Locally or using Remote Commands
5. Have Fun!

### __Playing Locally:__
To use the 🎮 game of Availiability basically you have to consider 4 things.
1) Connect the servomotor (barrier control 🚥) in P0. (90º Open - 0º Close)
2) Set the timer which the barrier control 🚥 will be open.
3) Set a input block 🧩 to start the 🎮 game. For example on button A pressed
4) Set a input block 🧩 to start to move the 🚗💨 car into the micro:bit screen. For example on button B pressed

### ``|>_|`` Code Example Availability Game! (Locally):
You can download the .hex file for this task by clicking [__⬇️ Here__](https://brilliantlabs.ca/documents/cybersec/Availability.hex), once downloaded, either drag and drop it into a new project. 
You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so.

```javascript
input.onButtonPressed(Button.A, function () {
 Cybersec.StartGame()
})
input.onButtonPressed(Button.B, function () {
 Cybersec.RunBC()
})
Cybersec.openbar()
Cybersec.timeclose(1200)
```

```blocks
input.onButtonPressed(Button.A, function () {
 Cybersec.StartGame()
})
input.onButtonPressed(Button.B, function () {
 Cybersec.RunBC()
})
Cybersec.openbar()
Cybersec.timeclose(1200)
```
### [[🔙 Back Tasks](#remote-commands-tasks)] | [[⏮️ Back Remote Commands](#remote-commands)]  
---
---