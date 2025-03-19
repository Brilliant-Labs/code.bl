### INTEGRITY
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


##### ``|>_|`` Code Example Controling Access Barrier 🚥:  
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
In this part of the task, 🧑‍🎓 students are encouraged to control the barrier by sending commands remotely from the *Control b.Board* to the *Device b.Board*.

#### __🧑‍🏫 Teachers:__
For __Integrity__ task in the frame from __Mission Fake Parking ID__ please follow the same steps for __Confidential__ task, in order to provide the 📳 access point name and password to the 🧑‍🎓 students.

---
#### __🧑‍🎓 Students:__
__1.__ Students should follow the steps in the __Confidential__ task to obtain their own 📮 IP address as well as their matched partner’s 📮 IP address.

__2.__ Once the matched teams are connected, they are ready to __Send Commands Remotely__ and control the parking access barrier 🚥. One team with a b.Board should act as the *Control b.Board*, while the matched partner should act as the *Device b.Board*.


### ``|>_|`` Code Example:
You can download the .hex file for this task by clicking [__⬇️ Here for Side *Control b.Board*__](https://brilliantlabs.ca/documents/cybersec/InegrityCnt.hex), or [__⬇️ Here for Side *Device b.Board*__](https://brilliantlabs.ca/documents/cybersec/InegrityDvc.hex) Once downloaded, either drag and drop it into a new project. 
You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so.
Agree with your match partner wich the side your are going to be part, *Control B.Board* or *Device b.Board*

##### ``|>_|`` *Side Control b.Board*
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
##### ``|>_|`` *Side Device b.Board*
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

<!--
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")
-->

```blocks
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
```


---
- *Please do not forget to set up the correct name and password for the access point.*
- *Mute the PC sound to listen the b.Board sound.*
---