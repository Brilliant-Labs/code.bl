# ACTIVITY 10
# PASSWORDS
---
##### ~avatar
Intro video about Cybersecurity Level 2 and __Cyberville__
https://www.youtube.com/watch?v=aapUlOM0EAo
##### ~
### [⎆ Go to Tasks](#passwords-tasks)
---
</br>
Welcome to __Activity 10: Passwords__ This activity takes place within the framwork of __Mission Weird Lights__. In this activity, you’ll learn some basic concepts and methods used in cybersecurity. These include passwords, brute force, dictionary, rainbow table, shoulder surfing, and more. In Mission Weird Lights, you'll need to solve a challenge and find the correct sequence to protect the school from a new cyberattack.

![Mission_1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/School_Under_Attack.gif?raw=true "Mission 1")

## Activity Description
__Cyberville__ has a traditional high school known as 🏫 'Lincoln High School' 2️⃣, with a student population of 350 students. The building is standard and uses some Internet of Things (IoT) components, such as heat control and automatic lighting that are able to automatically turned on during school hours and off at night.  These lights can also be controlled remotely by a supervisor working at the government building.  To save money, the school also controls heat and conditioning air with a remote-controlled thermostat from the 🏢 'Government Building' 5️⃣.

Recently, some reports have been sent to the supervisor about heat and light-related problems.  For example, one day the temperature in some classrooms went up without notice and was so uncomfortable that students and teachers had to leave the classroom.  Some events included lights flashing in the gymnasium and intermittent blinking in the school cafeteria.  Also, the number of phishing emails and spam mail has increased.  Last week, internet access was interrupted for a day.  Students and teachers couldn’t go on the Web for that period.

I just wanted to let you know that there is a proper way -*a sequence*- to turn on the devices affected by this situation to protect and save the school from the cyber attack. I know it can be tricky, but I'm sure you can find it!

In summary, the five affected devices are listed as __Heat Center, Air Conditioning, Lights Cafe, Lights Gym, and Internet__, which have a corresponding BLiXel number in the __b.board__. Provide the __Cyberville__ community with the right sequence using your __b.Board__ and pass this mission, saving 🏫 'Lincoln High School' 2️⃣!

![BliXels](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/BliXels.png?raw=true "BliXels")

Ready to level up your cybersecurity skills? As a complementary activity let's dive into the world of penetration testing! This is a great way to identify potential problems and find any malware that might have been installed on the school's web infrastructure. Once you find something, you get to be the detective and figure out where it came from, how to fix it, and how to make sure it doesn't happen again. The best part? You get to create a Cybersecurity Assessment Report, where you'll document all the problems you find, your solutions, and your recommendations to fix them. This is a great way to show off your skills and help keep the school’s digital space stay safe and secure!
__*Have fun!*__
---
---
# PASSWORDS TASKS

## - [1. SETTING PASSWORDS](#setting-passwords) 
## - [2. SEQUENCE TO ACCESS](#sequence-to-access) 
## - [3. PENETRATION TEST](#penetration-test) 
---
## SETTING PASSWORDS
![Set_Psw_Icon-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/1_Setting_Pws/Set_Psw_Icon-EN.png?raw=true "Set_Psw_Icon-EN") 
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝 **Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
</br>
__Passwords__ are super important in cybersecurity, and we're here to help you with that! They're the main way users can be sure they're who they say they are! Let's dive into some key points about passwords in cybersecurity together!
A strong password is usually long and complex, which makes it much harder for anyone to guess or crack them.

The most common passwords attack are __Brute Force, Phishing, Dictionary Attack, Credential Stuffing__.

Oh, yes! We’ve all been there, right? The __Cyberville__ 🏫 'Lincoln High School' 2️⃣ has been hacked, and that’s why you have to solve __Mission Weird Lights__. It can happen to anyone, and we totally get it if you're feeling a little overwhelmed right now. But don't you worry! There are ways you can protect yourself and our __Cyberville__ School from future attacks.

Let's learn together about some of the most common attacks on our passwords. Once we've done that, we'll solve the first mission, "Weird Lights - School Under Attack!"

---

### TASK 1: Setting Passwords!
Let's start! 

We've made it really easy for you to recreate the awesome environment from Mission Weird Lights while learning about cybersecurity. All you have to do is:

__1.__ Download [__👉 Here__](https://drive.google.com/file/d/1ZSzu_0UeyHQE4gBJYJ9oBOPWgcrouhkD/view?usp=sharing), print and cover the __b.Board__ for Mission Weird Lights.

![Cover](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/1_Setting_Pws/M1_Cover.png?raw=true "Cover")

![Cover for Mission 1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/1_Setting_Pws/Cover_Gif_M1.gif?raw=true "Cover for M1.")

__2.__ Students and teachers, we just wanted to remind you that it's important to choose a password to set up the __Cyberville__ network. It should be eight characters long, so that it is easy for you to remember, but difficult for intruders to guess.
Teachers will setup the password on M5 Module, students will do it on their code for __b.Board__.

---

### 🧑‍🏫 __Teachers:__

There are three differents ways to setup passwords on M5 module to start with the activity __Mission Weird Lights__. 

##### ~avatar
Options to setup __Passwords__:

🔹__No Password:__ Don't press any buttons on the initializing screen. [🎬 __*Video*__](https://www.canva.com/design/DAGJhwOPNfA/C7i4j-8NuAyaVB4WW4ZQLg/watch?utm_content=DAGJhwOPNfA&utm_campaign=designshare&utm_medium=link&utm_source=editor). 

🔹__Default Password:__ In this case the Default Password is __BL_Cybr1__. You must press the first button on the initializing screen to set the default password. [🎬 __*Video*__](https://www.canva.com/design/DAGJh3x2cWc/WLy_dI8ckApegcX8nVluYw/watch?utm_content=DAGJh3x2cWc&utm_campaign=designshare&utm_medium=link&utm_source=editor). 

🔹__Custom Password:__ We highly recommend this option to involve the students, just press middle button on M5Core2 on the initializing screen, enter the 8 character password agreed between the students and the teacher. For example: __BL_cyb24__, at the end please press the middle button again for three seconds to set it. [🎬 __*Video*__](https://www.canva.com/design/DAGJhzixXtc/zuFnnSe0t3ZZR298o1uEjg/watch?utm_content=DAGJhzixXtc&utm_campaign=designshare&utm_medium=link&utm_source=editor). 
##### ~


### 🧑‍🎓 __Students:__

🧑‍🎓 Students should do the steps made in 1_Connecting for __Networking__ in the previuos activity 7, using the __password__ defined in class.

![Set_Psw](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/1_Setting_Pws/SetPsw.png?raw=true "Setting Password in the b.Board.")

Quick note: Please make sure that __*b.Board is connected*__. Thanks!

![Conected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true "Conected.")

If you get a ✅, you are connected to Access Point 📳.
### ~ avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
### [[🔙 Back Tasks](#passwords-tasks)] | [[⏮️ Passwords](#passwords)]  
---
---
## SEQUENCE TO ACCESS
![Seq_to_Access_Icon-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/2_Seq_to_Access/Seq_to_Access_Icon-EN.png?raw=true "Seq_to_Access_Icon-EN") 
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝 **Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
</br>
Guess what! Our __Cyberville__ school is under a cyber attack.

To start this task, the __🧑‍🏫 teacher__ will choose a preset __*Sequence*__, which will display the 📳 M5 Module for Mission 1 as A, B, C, or D. This sequence will remain secret to the 🧑‍🎓 students! 

The __🧑‍🎓 Students__ will need to obtain the right *sequence* to turn on the devices that have been attacked.    

---

### 🧑‍🏫  __Teachers__
For __Mission Weird Lights__ Please follow the next steps that you will find on 📳 M5 module:

__1.__ Load __Mission Weird Lights__ on the 📳 M5 module. You can view this [🎬 __*video*__](https://drive.google.com/file/d/1Ra37Ctwg_KHiViCR3XP2hXUteJ2BQ-y6/view?usp=sharing) if you don't remember how to do this.

__2.__ Press the first button __GO!!!__, then select the __code protection sequence A,B,C,or D__ you want to use as a challenge for your students. 

![M5Act10](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/M5Act10.png?raw=true "M5Act10")  

__3.__ Share the current __Access Point name__ created by the M5 module with the classroom and the password, if one has been set. For example:  

`AP name 📳 :`__`Cyberville #?`__      
`Password 🔑:`__`BL_Cybr1 `__ *(If you are using default one)*

__4.__ Finally, select one of the four options (A, B, C or D) on the screen. Your choice will be highlighted in yellow. That is all!.  

![M1_Selected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/M1Selected_EN.png?raw=true "Mission Selected")  
  
Help the students 🧑‍🎓 with the __`File Attack Methods`__ [__👉 Here__](https://drive.google.com/file/d/1-3ZPRzpDkgGmVSEik0hyGoPHzpaL4n5F/view?usp=sharing) to succeed in this activity.

### 🧑‍🎓 __Students:__

__1.__ Connect to the WiFi access point on the 📳 M5 module. The 🧑‍🏫 teacher must provide the AP name and __password__. Use the 🧩 ``||Connect to WiFi||`` block. Remember, it should looks like this (✅ on screen __b.Board__): 
    ![Conected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true "Conected.")
If you get a ✅, you are connected to Access Point.
If you got a small __x__ (❎ on screen __b.Board__), you are __*NOT*__ connected.   
  
__2.__ Choose your role 👤 in __Cyberville__:  

| Role 👤  | Icon  | Entity's name|
| :------------------   | :---: | :----------------- |
|    1️⃣ School           |🏫| `Lincoln School`  
|    2️⃣ Hospital         |🏥| `Hospital Cyberville`  
|    3️⃣ Water            |💧| `AquaPure`  
|    4️⃣ WiFi-BL          |📳| `(Not available as role)`    
|    5️⃣ Government       |🏢| `Cyberville Gov.Services`   
|    6️⃣ Brilliant Labs   |🏩| `Brilliant Labs`    
|    7️⃣ Bank             |🏦| `Pacific Bank`    
|    8️⃣ Factory          |🏭| `Volt Motors`  
|    9️⃣ Industry         |🏪| `Techmach Industries`  
|    1️⃣0️⃣ Art Center     |🎨| `Harmony Art Center`   
|    1️⃣1️⃣ Cyber Security |🕵️‍♂️| `(Not available as role)`    
|    1️⃣2️⃣ Citizens       |😎| `The Cyberville community`  

<br>
In IDE code environment looks like:

![ChooseRole](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/ChooseRole-EN.png?raw=true "Choose a Role")    

__3.__ Select a device to be protected:   
    ✴️ 1 Heat Control ❄️  
    ✴️ 2 Air Control  🌀  
    ✴️ 3 Lamps Cafe 💡☕  
    ✴️ 4 Lamps Gym  💡🏃    
    ✴️ 5 Internet     🛜  
 
In IDE code environment looks like:  
![ChooseDevice](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/ChooseDevice-EN.png?raw=true "Choose a Role")
__4.__ Code the __b.Board__ to complete the sequence to turn on the devices affected by the hack. Remember that this sequence is secret, and you have to figure out how to get it.

__5.__ Use the 🧩 ``||Send Protection Sequence||`` block at the end to check if you have the right sequence defined by your 🧑‍🏫 teacher, and remember to have fun!.

##### ~avatar
📌 __*Notes:*__

🎶 When you send your *protection sequence code*, you will hear the Giggle sound effect.

🌟 You will see the BLiXel turn on with the reading depending on your code.

⭐️ If it matches the teacher sequence, your device will always be on.  Otherwise it will turn off.

🙂 At the end of your sequence you will get a smiley face if you were successful in this Mission.

🙁 If you were unsuccessful you will get a sad face. No worries! You just need to start again and try a new sequence.

---

__*At the end of the Challenge...*__

The first one to obtain the right sequence __Wins__.

The 📳 M5 module will display the winner's __Role__ name.

The 📳 access point will be reset to start a new challenge.

Remember to setup a new password and select a new sequence on the 📳 M5 module.
##### ~

 *Just a quick note to remind you to stay connected (* ✅ *on the __b.Board__'s screen). If you're not connected (* ❎ *on the __b.Board__'s screen), your code protection sequence will be disqualified and won't be sent.       
 You can send your new code, when you see a triangle (* 🔺 *on the __b.Board__'s screen).*

### ``|>_|`` Code Example:
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://brilliantlabs.ca/documents/cybersec/M1-School-Sequence-Access.hex). Once downloaded, either drag and drop it into a new project.
<!--
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")
-->

You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```javascript
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

This code example to evaluate your code sequence and test it.

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

### ~ avatar
- Please do not forget to set up the correct name and password for the access point. 
- Mute the PC sound to listen the __b.Board__ sound.
##### ~
### [[🔙 Back Tasks](#passwords-tasks)] | [[⏮️ Passwords](#passwords)]  
---
---
## PENETRATION TEST
![PenTest_Icon-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/Passwords/3_Pen_Test/PenTest_Icon-EN.png?raw=true "PenTest_Icon-EN") 
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝 **Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
</br>
Hi there! Have you ever wondered what a __Penetration Test__ is? It's a way of testing the security of a computer system, network, or web application by simulating a cyber attack. The goal is to identify and exploit vulnerabilities to determine whether someone could gain unauthorized access or cause other problems.

Penetration testing is an important part of keeping your organization, in this case our __Cyberville__ 🏫 School, safe from cyber threats.

To help with this task you will use this simplified Cybersecurity Assessment template. We hope it will be useful in writing your report!.

![PenTest](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/3_Pen_Test/Penetration_T.png?raw=true "Penetration Test")

Download to print [__👉 Here__](https://drive.google.com/file/d/1zBgB3JVFkSTaR0ie_8YnBxF33F_utgzx/view?usp=sharing)

### [[🔙 Back Tasks](#passwords-tasks)] | [[⏮️ Passwords](#passwords)]  
---
---