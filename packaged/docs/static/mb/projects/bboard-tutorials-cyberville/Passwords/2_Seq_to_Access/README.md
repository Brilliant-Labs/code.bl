# 2_Sequence to Access

Guess what! Our Cyberville school is under cyber attack.
To develop this activity, the __teacher__ will choose a __*code protection sequence*__, which will display the M5Core2 for Mission 1 as A, B, C, or D. This sequence will be secret to the students! 

![M1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/M1.jpg?raw=true "Mission 1, Weird Lights - School Under Attack!")

They must obtain it to succeed in this mission! You'll go through four basic cybersecurity concepts.

- ### Brute Force
![Brute_Force](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/Brute_Force.png?raw=true "Brute Force")

- ### Dictionary
![Dictionary](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/Dictionary.png?raw=true "Dictionary")

- ### Rainbow Table
![Rainbow_Table](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/Rainbow_Table.png?raw=true "Rainbow Table")

- ### Rainbow Table
![Shoulder_Surfing](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/Shoulder_Surfing.png?raw=true "Shoulder Surfing")

## Teachers
Teachers this is Mission 1:
![Mission1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/Mission1.png?raw=true "Mission 1")

## Students
You can __download__ an exaple code for this activity here:
https://alpha.brilliantlabs.ca/documents/cybersec/Cyber-Security-Activity-8.hex

Or use this code example for a possible __*code protection sequence*__

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