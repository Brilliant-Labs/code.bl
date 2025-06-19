## ACTIVITY 9
# 📡 🕹️ REMOTE COMMANDS 

---
##### ~avatar
Intro video about Cybersecurity Level 2 and __Cyberville__
https://www.youtube.com/watch?v=aapUlOM0EAo
##### ~
</br>

# 📘 __*Guide Document:*__  
- Official Document in **English** [__👉 Here__](https://www.canva.com/design/DAGjA-4v45U/nwkQv_N8wEyc51at9ZnZTQ/edit)  
- Document officiel en **French** [__👉 Ici__](https://www.canva.com/design/DAGE9DpMoOo/1kgvrPWSxI5Ix_wXhTbzVQ/edit)
</br>
</br>

# 🚀 __*Let's get started!*__
## __``Task #1: Confidentiality``__

- 1️⃣ Conect you to __Cyberville__ wifi network.🧑‍🎓 Students do the steps in __Activity 7 Task Connecting__, but add the __Password__ that 🧑‍🏫 teacher should share in a __secure__ and __confidential__ way. 

- 2️⃣ Randomly draw a secret 🎟️ ID ticket from a bag and use their coding skills to find a classmate with the matching identification code and second authentication factor (MFA). Download the tickets for __Confidentiality__ activity: **EN**: [👉 Click here](https://drive.google.com/file/d/12b9a48Wd3usLQetgtnWsPsuGEiasOYXX/view?usp=sharing), **FR**: [👉 Cliquez ici](https://drive.google.com/file/d/133DRmbyUF0PooIGfG8PkBfk3jbTgqkA0/view?usp=sharing).

    ![Tickets](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/Tickets.png?raw=true "Tickets")

- 3️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://brilliantlabs.ca/documents/cybersec/Confidentiality.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

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

- 4️⃣ Create a table listing the roles of all 📮 IP addresses in the network and do the __*MATCH! 🤝*__ following the 📘 Guide Document.

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

- 5️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
</br>
</br>




## __``Task #2: Integrity``__  





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
You can download the .hex file for this task by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Availability_Local.hex), once downloaded, either drag and drop it into a new project. 
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

---
---
### ___Playing using Remote Commands:__
To use the 🎮 game of Availiability using Remote Commands, basically you have to consider 6 things.
1) A classmate will set the timer remotly, and you have to run before the 🚥 barrier close. so you need two bBoards.
2) Both needs to know thier own 📮 IP Address and classmate 📮 IP Address, so you have to be connected to the Access point 📳 M5 module, and be ready to hear any message.
3) Connect the servomotor (barrier control 🚥) in P0. (90º Open - 0º Close).
4) For Sending Timer b.Board side 
 Set a input block 🧩 to Send Number: (---) To IP: (---.---.---.---). For example on button A pressed.
Download the code.

When your classamate is ready, send the timer number, remember it is in miliseconds. This start the timer before the barrier will close on the receiving b.Board side.
5) For Receiving Runner b.Board side
Set a input block 🧩 to receive the timer value (data) from your classmate, use the 🧩Block Number received from IP: (---.---.---.---).
Set a input block 🧩 to start the 🎮 game Star Closing. For example on button A pressed
Set a input block 🧩 to start to move the 🚗💨 car into the micro:bit screen. For example on button B pressed

### ``|>_|`` Code Example Availability Game! (Sending Timer Remotely):
You can download the .hex file by clicking [__⬇️ Here__](https://brilliantlabs.ca/documents/cybersec/Availability_Timer_Remotely.hex), once downloaded, either drag and drop it into a new project. 
You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so.

```javascript
input.onButtonPressed(Button.A, function () {
 Cybersec.Num_UDP_Snd(1200, "192.168.4.?")
})
Cybersec.WifiConnect("Cyberville #?", "")
```
```blocks
input.onButtonPressed(Button.A, function () {
 Cybersec.Num_UDP_Snd(1200, "192.168.4.?")
})
Cybersec.WifiConnect("Cyberville #?", "")
```

### ``|>_|`` Code Example Availability Game! (Receiving Runner Remotely):
You can download the .hex file by clicking [__⬇️ Here__](https://brilliantlabs.ca/documents/cybersec/Availability_Runner_Remotely.hex), once downloaded, either drag and drop it into a new project. 
You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so.

```javascript
input.onButtonPressed(Button.A, function () {
 Cybersec.StartGame()
})
input.onButtonPressed(Button.B, function () {
 Cybersec.RunBC()
})
let Timer = 0
let Temp = 0
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
Cybersec.openbar()
basic.forever(function () {
 Temp = Cybersec.ReceiveNumber("192.168.4.?")
 if (Temp > 0) {
 Timer = Temp
 basic.showNumber(Timer)
 Cybersec.timeclose(Timer)
 }
})
```
```blocks
input.onButtonPressed(Button.A, function () {
 Cybersec.StartGame()
})
input.onButtonPressed(Button.B, function () {
 Cybersec.RunBC()
})
let Timer = 0
let Temp = 0
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
Cybersec.openbar()
basic.forever(function () {
 Temp = Cybersec.ReceiveNumber("192.168.4.?")
 if (Temp > 0) {
 Timer = Temp
 basic.showNumber(Timer)
 Cybersec.timeclose(Timer)
 }
})
```


### [[🔙 Back Tasks](#remote-commands-tasks)] | [[⏮️ Back Remote Commands](#remote-commands)]  
---