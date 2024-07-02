# 2_Sequence to Access

Guess what! Our Cyberville school is under a cyber attack.

To develop this activity, the __teacher__ will choose a __*code protection sequence*__, which will display the M5Core2 for Mission 1 as A, B, C, or D. This sequence will be secret to the students! 

![M1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/M1.jpg?raw=true "Mission 1, Weird Lights - School Under Attack!")

The __*Students*__ will need to obtain the right *sequence* to turn on the devices that have been attacked.

## Teachers
Teachers this is Mission 1 that you will find on M5Core2 module:

![Mission1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/Mission1.png?raw=true "Mission 1")

Please follow the next steps:

1. Load __Mission_1: Weird Lights__ into M5Core2. You can see this [video](https://www.canva.com/design/DAGJhm69_Mk/JdN1bb74mN-bKiclzST5Ag/watch?utm_content=DAGJhm69_Mk&utm_campaign=designshare&utm_medium=link&utm_source=editor) if you want to remember how to do it.

2. Press the first button __Go!!__, then select the __code protection sequence__ you want to use as a challenge for your students. 

3. Share the current __Access Point__ name created by the M5Core2 with the classroom. For example:
                Cyberville #1

4. Finally, press on the screen between options A, B, C or D. Your selection will turn on in yellow color. That is all!  Help the students with the [file attack methods](https://www.canva.com/design/DAGHlrBxBfU/6qFptClpEV4OzdJmi5frkQ/view?utm_content=DAGHlrBxBfU&utm_campaign=designshare&utm_medium=link&utm_source=editor). 

## Students

1. Connect to the WiFi access point. The teacher should have provided the correct name. Use the *Connect to WiFi* block. Remember, it should look like this:
![Connected_gif](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true "Connected_gif")

2. Code the b.Board to do sequence to turn on the devices affected by the hacked, remembering that it is secret from your teacher and you have to get it.

3. Use a block *Send protection sequence* at the end to check if it is the right sequence defined by the teacher, have fan!

***

📌 __*Notes:*__

╔═══════════════════════════════════╗

🏫 The entire classroom role for Mission 1 is "__School__".

🔊 When you send your *protection sequence code*, you will hear the song Giggle.

🌟 You will shortly see the BLiXel device turn on according to your code.

⭐️ If it matches the teacher sequence, your device will always be on.  Otherwise it will turn off.

🙂 At the end of your sequence you will get a smiley face if you were successful in this Mission 1.

🙁 Or maybe a sad face if not. No worries! You've just got to start again.

╚═══════════════════════════════════╝
***

You can __download__ an example code for this activity in this web site: `https://alpha.brilliantlabs.ca/documents/cybersec/Cyber-Security-Activity-8.hex`

Or use this code example for a possible __*code protection sequence*__ to obtain the right sequense to turn on the devices affected by the hacked.

Allways be sure that you are connected in the right Cyberville network, before you try a new code.

```blocks
Cybersec.WifiConnect("Cyberville", "BL_Cyb1")
basic.forever(function () {
})
input.onButtonPressed(Button.A, function () {
    Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.one))
    Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.two))
    Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.three))
    Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.four))
    Cybersec.MissionLights(Cybersec.blixel_indexR(BLiXelIndexR.one), Cybersec.appliance_index(ApplianceIndex.five))
    Cybersec.sendprot()
})
```