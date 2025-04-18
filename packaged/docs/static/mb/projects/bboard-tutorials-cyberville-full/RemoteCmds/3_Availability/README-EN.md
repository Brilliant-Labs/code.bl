
---
# ~avatar
_Please read the activity carefully and follow the steps provided. In the Code Example section, you will be able to_ 📝**Edit** _the sample code or_ ⬇️ **download** _it to your __b.Board__._
# ~
---

### TASK 3: Availability

Let's get started!
1. [__👉 Download__](https://drive.google.com/file/d/1lYtZyyQ5f7qhXzua5LGw7-LFFzpQwcW4/view?usp=sharing), print and cover the b.Board for Mission Fake Parking ID.
![Availability](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville-full/RemoteCmds/3_Availability/Availability.png?raw=true "Availability")

2. Connect the servomortor to P0, it will be your barrer control.
3. Code or download the game.
4. Play Locally or using Remote Commands
5. Enjoy!

#### Playing Locally:
To use the 🎮 game of Availiability basically you have to consider 4 things.
1) Connect the servomotor (barrier control 🚥) in P0. (90º Open - 0º Close)
2) Set the timer which the barrier control 🚥 will be open.
3) Set a input block 🧩 to start the 🎮 game. For example on button A pressed
4) Set a input block 🧩 to start to move the 🚗💨 car into the micro:bit screen. For example on button B pressed


### ``|>_|`` Code Example:
You can download the .hex file for this task by clicking [__⬇️ Here__](https://brilliantlabs.ca/documents/cybersec/Availability.hex) once downloaded, either drag and drop it into a new project. 
You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so.

##### ``|>_|`` *Side Control b.Board*

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


