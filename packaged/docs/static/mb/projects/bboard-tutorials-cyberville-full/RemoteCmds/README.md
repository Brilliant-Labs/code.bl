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

- 1️⃣ Connect to the Cyberville Wi-Fi network. follow the steps in __Activity 7 – Task: Connecting__, but be sure to add the Password, which the 🧑‍🏫 teacher should share in a __secure__ and __confidential__ way.

</br>

- 2️⃣ Randomly draw a secret 🎟️ ID ticket from a bag and use their coding skills to find a classmate with the matching identification code and second authentication factor (MFA). Download the tickets for __Confidentiality__ activity: **EN**: [👉 Click here](https://drive.google.com/file/d/12b9a48Wd3usLQetgtnWsPsuGEiasOYXX/view?usp=sharing), **FR**: [👉 Cliquez ici](https://drive.google.com/file/d/133DRmbyUF0PooIGfG8PkBfk3jbTgqkA0/view?usp=sharing).

    ![Tickets](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/Tickets.png?raw=true "Tickets")

</br>

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

- 5️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
</br>
</br>

## __``Task #2: Integrity``__  

This __Integrity__ task is divided into two parts:
- 1️⃣ __First part, controlling a parking access barrier 🚥 Locally:__  (No matched pairs b.Boards is needed).

    Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
    Program a b.Board to control a servomotor __locally__ to understand how it functions.

    </br>  
- 2️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://brilliantlabs.ca/documents/cybersec/Integrity-Local.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

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
Cybersec.Localparkbar()
basic.forever(function () {
    servos.P00.setAngle(Cybersec.getValueDeg())
})
```
</br>

- 3️⃣ __Second part, controlling a parking access barrier 🚥 Remotely__ (For matched pairs b.Boards.)
    
    Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
    Control the barrier by sending commands remotely from the b.Board *Control* to the b.Board *Barrier*.

    * Download the ``Code Example Control Remotely`` .hex file for this activity by clicking [⬇️ Here b.Board *Control*](https://brilliantlabs.ca/documents/cybersec/Integrity_Control_Remotely.hex). 

    * Download the ``Code Example Barrier Remotely`` .hex file for this activity by clicking [⬇️ Here b.Board *Barrier*](https://brilliantlabs.ca/documents/cybersec/Integrity_Barrier_Remotely.hex).  

    Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

``|>_| Code Example Control Remotely``
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
``|>_| Code Example Barrier Remotely``
```blocks
Cybersec.WifiConnect("Cyberville #?", "")
Cybersec.Rdy2listen()
```
</br>
</br>

## __``Task #3: Availability``__  

This game about __Availability__ is divided into two parts: one is local, and the other is remote.

- 1️⃣ Download the b.Board cover for the __Availability__ activity: **EN**: [👉 Click here](https://drive.google.com/file/d/1lYtZyyQ5f7qhXzua5LGw7-LFFzpQwcW4/view?usp=sharing), **FR**: [👉 Cliquez ici](https://drive.google.com/file/d/1_HTOF8bkxYe9E68t4K5V7bJIeHRwRawb/view?usp=sharing).  

    ![Availability](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/3_Availability/Availability.png?raw=true "Availability")


- 2️⃣ ___Playing Locally:__
    Download the ``Code Example Playing Locally`` .hex file for this activity by clicking [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Availability_Local.hex). 
    Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

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
</br>

- 3️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and complete the full activity.
    Program a b.Board to control a servomotor __locally__ to understand how it functions.

</br>

- 4️⃣ __Playing using Remote Commands:__
    Play the game with a b.Board partner, one team should be the Timer and the other the Runner.
    * Download the ``Code Example Sending Timer Remotely`` .hex file for this activity by clicking [⬇️ Here](https://brilliantlabs.ca/documents/cybersec/Availability_Timer_Remotely.hex). 

    * Download the ``Code Example Receiving Runner Remotely`` .hex file for this activity by clicking [⬇️ Here](https://brilliantlabs.ca/documents/cybersec/Availability_Runner_Remotely.hex). 

    Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:



``|>_| Code Example Sending Timer Remotely``
```blocks
input.onButtonPressed(Button.A, function () {
 Cybersec.Num_UDP_Snd(1200, "192.168.4.?")
})
Cybersec.WifiConnect("Cyberville #?", "")
```
``|>_| Code Example Receiving Runner Remotely``
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

- 4️⃣ Based on the Cybersecurity skills you’ve developed in class, and the 📘 Guide Document download your customized code onto the b.Board and enjoy the game.
</br>
</br>
</br>

---
# 📌 __*Notes:*__
☑️ Please do not forget to set up the correct name and password for the access point.     
☑️ Mute the PC sound to listen the __b.Board__ sound.    
☑️ If you’d like, you can also view the data going in and out of the b.Board using the __*Show Console Device*__ option.    

        Once you download your code...
- Click on the refresh button 🔄 (circular arrow icon) in the simulator window.
- __Wait__ until *Show console Device* button apears on console output window.
- Click on it.

![Remote](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/Remote.png?raw=true "Remote")