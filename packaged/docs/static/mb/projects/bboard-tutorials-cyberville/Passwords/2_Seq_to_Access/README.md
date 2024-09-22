# 2_SEQUENCE TO ACCESS

Guess what! Our __Cyberville__ school is under a cyber attack.

To develop this activity, the __🧑‍🏫 teacher__ will choose a __*code protection sequence*__, which will display the 📳 M5 Module for Mission 1 as A, B, C, or D. This sequence will be secret to the 🧑‍🎓 students! 

The __🧑‍🎓 Students__ will need to obtain the right *sequence* to turn on the devices that have been attacked.  

---  

### 🧑‍🏫  __Teachers__
For __Mission 1- Weird Light__ Please follow the next steps that you will find on M5Core2 module:

1. Load __Mission_1: Weird Lights__ into M5Core2. You can see this [__video__](https://www.canva.com/design/DAGJhm69_Mk/JdN1bb74mN-bKiclzST5Ag/watch?utm_content=DAGJhm69_Mk&utm_campaign=designshare&utm_medium=link&utm_source=editor) if you want to remember how to do it.

2. Press the first button __GO!!!__, then select the __code protection sequence A,B,C,or D__ you want to use as a challenge for your students. ![Act8_M1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/Act8_M1.png?raw=true "Activity 8 Mission 1")

3. Share the current __Access Point name__ created by the M5Core2 with the classroom and the password if it is the case. For example:  
        AP name  📳: __Cyberville #1__  
        Password 🔑: __BL_Cybr1__ *(if you are using default one)*

4. Finally, press on the screen between options A, B, C or D. Your choice will be highlighted in yellow. That is all!.  

![M1_Selected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/M1Selected.png?raw=true "Mission Selected")  
  
Help the students 🧑‍🎓 with the [__File Attack Methods__](https://drive.google.com/file/d/1jTZZxPD-yWJKPnu3njlZYRXsEjrpXb3o/view?usp=drive_link) to succeed in this activity.

### 🧑‍🎓 __Students__

__1.__ Connect to the WiFi access point 📳 M5 Module. The 🧑‍🏫 teacher must provide the AP name and __password__. Use the *Connect to WiFi* block. Remember, it should looks like this (✅ on screen b.Board):
<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true" alt="Connected_gif" title="If you get a ✅, you are connected to Access Point" width="300" />  

If you got a small __x__ (❎ on screen b.Board), you are __*NOT*__ connected.   
  
__2.__ Choose your role 👤 in __Cyberville__:  
    1 School          🏫  `Lincoln School`  
    2 Hospital        🏥  `Hospital Cyberville`  
    3 Water           💧  `AquaPure`  
    4 WiFi-BL         📳  (Not available as role)    
    5 Government      🏢  `Cyberville Gov.Services`   
    6 Brilliant Labs  🏩  `Brilliant Labs`    
    7 Bank            🏦  `Pacific Bank`    
    8 Factory         🏭  `Volt Motors`  
    9 Industry        🏪  `Techmach Industries`  
    10 Art Center     🎨  `Harmony Art Center`   
    11 Cyber Security 🕵️‍♂️  (Not available as role)    
    12 Citizens       😎  `The Cyberville community`  
    
In IDE code environment looks like:  
![ChooseRole](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/ChooseRole.png?raw=true "Choose a Role")    

__3.__ Select a device to be protected:   
    1 Heat Control ❄️  
    2 Air Control  🌀  
    3 Lamps Cafe 💡☕  
    4 Lamps Gym  💡🏃    
    5 Internet     🛜  
 
In IDE code environment looks like:  
    ![ChooseDevice](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/ChooseDevice.png?raw=true "Choose a Role")

__4.__ Code the b.Board to do sequence to turn on the devices affected by the hacked, remembering that it is secret from your teacher 🧑‍🏫 and you have to get it.

__5.__ Use a block *Send protection sequence* at the end to check if it is the right sequence defined by the teacher, have fan!
  
***

##### ~avatar
📌 __*Notes:*__

🎶 When you send your *protection sequence code*, you will hear the song Giggle.

🌟 You will shortly see the BLiXel device turn on according to your code.

⭐️ If it matches the teacher sequence, your device will always be on.  Otherwise it will turn off.

🙂 At the end of your sequence you will get a smiley face if you were successful in this Mission 1.

🙁 Or maybe a sad face if not. No worries! You've just got to start again.

---

__*At the end of the Challenge...*__

The first one to obtain the right sequence __Wins__.

The 📳 M5 module will display the winner's __Role__ name.

The 📳 access point will be reset to start a new challenge.

Remember to setup a new password and select a new sequence on the 📳 M5 module.
##### ~



---

 *Just a quick note to remind you to stay connected*
 (✅ on screen b.Board). *If you're not connected* (❎ on screen b.Board)*, your code protection sequence will be disqualified* *and won't be sent.       
 You can send your new code, when you see a triangle* (🔺 on screen b.Board).*

---

## Code Example

You can download the code for this activity from `https://brilliantlabs.ca/documents/cybersec/M1-School-Sequence-Access.hex` the file will be in Recent Download History, just drag and drop it into a new project.  

Or use this code example to evaluate your code sequence and test it.

__*Please do not forget to set up the correct name and password for the access point.*__

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.WifiConnect("Cyberville #?", "")
    if (Cybersec.WiFi_Connected()) {
        Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.one))
        Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.two))
        Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.three))
        Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.four))
        Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.five))
        Cybersec.sendprot()
    } else {
        basic.showLeds(`
            # . . . #
            . # . # .
            . . # . .
            . # . # .
            # . . . #
            `)
    }
})

```