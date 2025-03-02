# 1_CONFIDENTIALITY
Do you want to keep a secret safe? 🤫 Then confidentiality is the best place to start! It’s like having a top-secret vault where only the people you trust and give permission (like your best friend… maybe 😉) can access the information.
🕵️‍♂️ But What If a Sneaky Snoop Tries to Peek?
Hackers (a.k.a. digital troublemakers) are always looking for ways to sneak into your private information. They might try to: 🔑 Guess your password, 🕶️ Steal secret codes, 🤥 Trick you into giving them access.
But don’t worry! Good cybersecurity helps keep them out and protects your secrets! 💪

Oh no! The 🏢 Government Parking Lot is under cyber attack! Someone created fake ID passes, which means the parking lot lost its Confidentiality. In this mission, we’ll dive deeper into __Confidentiality__ and learn how to protect our information just like the Government Parking Lot should have!

There are several ways in which we can protect your privacy (Confidentiality), and here are a few of them:
Passwords & Locks 🔑 – Computers use passwords to keep information safe.
Secret Codes (Encryption) 🔐 – Even if someone gets in, they’ll just see a bunch of jumbled-up nonsense unless they have the secret key!
Security Guards (Firewalls & Antivirus) – They act like bodyguards, keeping the bad guys away.
Multi-factor authentication (or 2FA) - Require two or more pieces of evidence to access.
Access control (Approval) - Enable to manage who is autorized to access adata and resources.

## __Activity Description__
For this activity, we're going to explore some ways to protect our information: 🔑 __Passwords__, 🔐 Encription, and 🪪 Multifactor Authentication!

## __🧑‍🏫 Teachers:__
For __Mission 3__ Fake Parking Passe__ Please follow the next steps that you will find on M5 module:

__1.__ Load __Mission 3__ Fake Parking Passe__ into 📳 M5 module. You can see this [__video__](https://www.canva.com/design/DAGJhm69_Mk/JdN1bb74mN-bKiclzST5Ag/watch?utm_content=DAGJhm69_Mk&utm_campaign=designshare&utm_medium=link&utm_source=editor) if you want to remember how to do it.
__2.__ Press the first button __GO!!!__, then guide the 🧑‍🎓 students for the activity. 
__3.__ Share the current __Access Point name__ created by the  📳 M5 module with the classroom and the password if it is the case. For example:  AP name 📳: __Cyberville #1__ 
__4.__ In order to involve the student in the __Confidentialy__ concept, 🧑‍🏫 theachers need to setup a 🔑Password. Remember that there are three differents ways to setup passwords on  📳 M5 module for Cyberville network. Agree with student which password are you going to use for this activity. 

- [__No Password__](https://www.canva.com/design/DAGJhwOPNfA/C7i4j-8NuAyaVB4WW4ZQLg/watch?utm_content=DAGJhwOPNfA&utm_campaign=designshare&utm_medium=link&utm_source=editor). Just a friendly reminder: don't press any buttons! Thanks!

- [__Default Password__](https://www.canva.com/design/DAGJh3x2cWc/WLy_dI8ckApegcX8nVluYw/watch?utm_content=DAGJh3x2cWc&utm_campaign=designshare&utm_medium=link&utm_source=editor). In this case the Default Password is __BL_Cybr1__. Just wanted to let you know that you must press the first button to set the default password. 

- [__Custom Password__](https://www.canva.com/design/DAGJhzixXtc/zuFnnSe0t3ZZR298o1uEjg/watch?utm_content=DAGJhzixXtc&utm_campaign=designshare&utm_medium=link&utm_source=editor). We highly recommend this option to involve the students, just press middle button on  📳  M5 module, and enter the agreed 8 characters of the password agreed between the student and the teacher, for example __BL_cyb24__, at the end please press the middle button again for three seconds to set it. That is all!
__5.__ Once the password is set by the 🧑‍🏫 teacher, for example Password 🔑: __BL_Cybr1__ *(if you are using default one)* must find the way to securely share the Password  with the  🧑‍🎓 students doing a broken phone game or ecryption game like this:



### 🧑‍🎓 __Students__
__1.__ Students should follow the steps in Activity 1_Connecting for __Networking__, but add the __Password__ that 🧑‍🏫 teacher should share in a secure and confidential way. 

![Set_Psw] https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/1_Setting_Pws/SetPsw.png



Just a quick note to ask that you please __make sure that b.Board is connected__. 









https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif

If you get a ✅, you are connected to Access Point 📳.
__2.__ It is crucial for the students to know the IP address of the b.Board in order to succeed in this mission 3, the students must fill out the ID card again, but in this case only with the name and IP address. Remember that you can download and print the ID card from these links
### 🧑‍🎓 __*Students ID Card*__
Download the ID Card for Students 🧑‍🎓 [__⬇️ Here__] https://drive.google.com/file/d/1uYi49zPMzKYuliF4TlS2NQBoPTkMTcoD/view?usp=drive_link


For this first part of the activity, this should be a good example of how to fill out the Cyberville ID card.

## Code Example
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex). 
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")

_**`Please do not forget to set up the correct name and password for the access point. Mute the PC sound to listen the b.Board sound.`**_

You can use this code example to obtain the 📮 IP addresses.

```blocks
input.onButtonPressed(Button.A, function () {
 basic.showString(Cybersec.getIPaddressbBoard())
})
Cybersec.WifiConnect("Cyberville #?", "")
basic.forever(function () { 
})
```

📌 __*Notes:*__
If you would like, you can also see the 📮 IP address on the __*Show Console Device*__.
### ~ avatar
*Once you download your code...*
1. Click on the refresh button 🔄 (circular arrow icon) in the simulator window.
2. __Wait__ until *Show console Device* button apears on console output window.
3. Click on it.

![Console](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Console.png?raw=true "Console Device")
### ~