# 📒 b.Board Tutorial Cards / 📒 Cartes de tutoriel b.Board:

# `LIGHTS-LUMIERES`

| English | French |
| ------------------------------- | ------------------------------- | 
| [Make it Light Up](#make-it-light-up) | [Faites le allumer](#faites-le-allumer)  | 
| [Make it Light Different Colors](#make-it-light-different-colors) | [Faites le allumer differentes couleurs](#faites-le-allumer-differentes-couleurs) |
| [Make it Light Up Different Colors Using a Button](#make-it-light-up-different-colors-using-a-button) | [Faites le allumer de differentes couleurs a laide d bouton](#faites-le-allumer-de-differentes-couleurs-a-laide-d-bouton) | 
| [Add Your Name Screen](#add-your-name-screen)  | [Ajoutez votre nom l ecrean del](#ajoutez-votre-nom-l-ecrean-del)  |
| [Make it Light a LED](#make-it-light-a-led) | [Faire allumer une led](#faire-allumer-une-led) |
| [Make a Night Light ](#make-a-night-light) | [Fabriquez une veilleuse](#fabriquez-une-veilleuse) |
| [Light Up Dark](#light-up-dark) | [S allumer quad il fait noir](#s-allumer-quad-il-fait-noir) |

---
---
# `🇬🇧 ENGLISH`
---
## Make it Light Up
![Mkt_Light_UP-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights1/Mkt_Light_UP-EN.png?raw=true "MAKE IT LIGHT UP!")
### Code Example
Example MAKE IT LIGHT UP! using the b.Board
```blocks
basic.forever(function () {
BLiXel.showColour(0xff9da5)
})
```
---
##### [🔙 Back Menu](#lights-lumieres) 
---
## Make it Light Different Colors
![Mkt_Light-Up_Diff_Color-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights2/Mkt_Light-Up_Diff_Color-EN.png?raw=true "Mkt_Light-Up_Diff_Color-EN!")
### Code Example
Example MAKE IT LIGHT UP different COLORS ! using the b.Board
```blocks
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.one), 0xffff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.two), 0x00ff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.three), 0xffffff)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.four), 0xff0000)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.five), 0x007fff)
```
---
##### [🔙 Back Menu](#lights-lumieres) 
---
## Make it Light Up Different Colors Using a Button

![Mkt_Light-Up_Diff_Color_Button-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights3/Mkt_Light-Up_Diff_Color_Button-EN.png?raw=true "Mkt_Light-Up_Diff_Color_Button-EN!")
### Code Example
Example MAKE IT LIGHT UP different COLORS using a button ! using the b.Board
```blocks
input.onButtonPressed(Button.A, function () {
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.one), 0xffff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.two), 0x00ff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.three), 0xffffff)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.four), 0xff0000)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.five), 0x007fff)
})
```
---
##### [🔙 Back Menu](#lights-lumieres) 
---
## Add Your Name Screen
![Add_Your_Name_Screen-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights4/Add_Your_Name_Screen-EN.png?raw=true "Add_Your_Name_Screen-EN!")
### Code Example
Example ADD YOUR NAME TO THE LED SCREEN! using the b.Board
```blocks
basic.forever(function () {
basic.showString("Bob")
})
```
---
##### [🔙 Back Menu](#lights-lumieres) 
---
## Make it light a LED
![Mkt_Light_Led-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights5/Mkt_Light_Led-EN.png?raw=true "Mkt_Light_Led-EN!")
### Code Example
Example Make it light a LED using the b.Board
```blocks
input.onButtonPressed(Button.A, function () {
pins.digitalWritePin(DigitalPin.P0, 1)
})
input.onButtonPressed(Button.B, function () {
pins.digitalWritePin(DigitalPin.P0, 0)
})
```
---
##### [🔙 Back Menu](#lights-lumieres) 
---
## Make a Night Light 
![Mkt_Night_Light-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights6/Mkt_Night_Light-EN.png?raw=true "Mkt_Night_Light-EN")
---
##### [🔙 Back Menu](#lights-lumieres) 
---
## Light Up Dark
![Light_Up_Dark-EN](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights7/Light_Up_Dark-EN.png?raw=true "Light_Up_Dark-EN")
## Code Example
Example   LIGHT UP WHEN ITS DARK using the b.Board
```blocks
basic.forever(function () {
BLiXel.showColour(0x000000)
while (input.lightLevel() < 50) {
BLiXel.showColour(0xffffff)
}
})
```
---
##### [🔙 Back Menu](#lights-lumieres) 


---
---
# `🇫🇷 FRENCH`
---
## Faites le allumer
<!-- ![Mkt_Light_UP-FR](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights1/Mkt_Light_UP-FR.png?raw=true "MAKE IT LIGHT UP!") -->
![Mkt_Light_UP-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights1/Mkt_Light_Up-FR.png?raw=true "MAKE IT LIGHT UP!")

### Exemple de code
Exemple FAIS-LE S’ALLUMER ! en utilisant la b.Board
```blocks
basic.forever(function () {
BLiXel.showColour(0xff9da5)
})
```
---
##### [🔙 Menu Retour](#lights-lumieres) 
---
## Faites le allumer differentes couleurs
![Mkt_Light-Up_Diff_Color-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights2/Mkt_Light-Up_Diff_Color-FR.png?raw=true "Mkt_Light-Up_Diff_Color-FR!")

### Exemple de code
Exemple FAIS-LE S’ALLUMER EN DIFFÉRENTES COULEURS ! en utilisant la b.Board
```blocks
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.one), 0xffff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.two), 0x00ff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.three), 0xffffff)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.four), 0xff0000)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.five), 0x007fff)
```
---
##### [🔙 Menu Retour](#lights-lumieres) 
---
## Faites le allumer de differentes couleurs a laide d bouton

![Mkt_Light-Up_Diff_Color_Button-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights3/Mkt_Light-Up_Diff_Color_Button-FR.png?raw=true "Mkt_Light-Up_Diff_Color_Button-FR!")

### Exemple de code
Exemple FAIS-LE S’ALLUMER EN DIFFÉRENTES COULEURS AVEC UN BOUTON ! en utilisant la b.Board
```blocks
input.onButtonPressed(Button.A, function () {
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.one), 0xffff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.two), 0x00ff00)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.three), 0xffffff)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.four), 0xff0000)
BLiXel.setPixelColour(BLiXel.blixel_index(BLiXelIndex.five), 0x007fff)
})
```
---
##### [🔙 Menu Retour](#lights-lumieres) 
---
## Ajoutez votre nom l ecrean del
![Add_Your_Name_Screen-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights4/Add_Your_Name_Screen-FR.png?raw=true "Add_Your_Name_Screen-FR!")

### Exemple de code
Exemple AJOUTE TON NOM SUR L’ÉCRAN À LED ! en utilisant la b.Board
```blocks
basic.forever(function () {
basic.showString("Bob")
})
```
---
##### [🔙 Menu Retour](#lights-lumieres) 
---
## Faire allumer une led
![Mkt_Light_Led-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights5/Mkt_Light_Led-FR.png?raw=true "Mkt_Light_Led-FR!")

### Exemple de code
Exemple FAIS ALLUMER UNE LED en utilisant la b.Board
```blocks
input.onButtonPressed(Button.A, function () {
pins.digitalWritePin(DigitalPin.P0, 1)
})
input.onButtonPressed(Button.B, function () {
pins.digitalWritePin(DigitalPin.P0, 0)
})
```
---
##### [🔙 Menu Retour](#lights-lumieres) 
---
## Fabriquez une veilleuse 
![Mkt_Night_Light-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights6/Mkt_Night_Light-FR.png?raw=true "Mkt_Night_Light-FR")

---
##### [🔙 Menu Retour](#lights-lumieres) 
---
## S allumer quad il fait noir
![Light_Up_Dark-FR](https://raw.githubusercontent.com/Brilliant-Labs/code.bl/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-full-cards/2_Lights/Lights7/Light_Up_Dark-FR.png?raw=true "Light_Up_Dark-FR")

## Exemple de code
Exemple ALLUME LA LUMIÈRE LORSQU’IL FAIT SOMBRE en utilisant la b.Board
```blocks
basic.forever(function () {
BLiXel.showColour(0x000000)
while (input.lightLevel() < 50) {
BLiXel.showColour(0xffffff)
}
})
```
---
##### [🔙 Menu Retour](#lights-lumieres) 
---