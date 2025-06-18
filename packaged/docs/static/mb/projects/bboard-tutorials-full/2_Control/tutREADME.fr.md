#📒 Tutoriel b.Board - Clickboards :

# `CONTRÔLE`

<!-- - [Button G](#button-g) 
- [Keylock](#keylock) 
- [Relay](#relay) 
- [Servo](#servo)
- [Moteur](#moteur)
- [Mini LCD](#mini-lcd)
---
-->

## Bouton G
# Neopixels + Button_G
# ACTIVE TON RYTHME

![alt text](\docs\static\mb\projects\bboard-tutorials-full\2_Control\button-g\button_A.gif "For more info: www.brilliantlabs.ca")

Tu as un super projet Neopixel ultra lumineux, mais aucun moyen de lancer ton code ? Ne cherche pas plus loin que la ClickBoardTM Bouton G. Elle peut être étendue grâce à notre carte d’extension connectée à ta b.Board pour vraiment démarrer le spectacle lumineux. Non seulement le bouton G est agréable à presser, mais il dispose aussi d'une LED intégrée qui attirera l’attention de tes invités. Ce bouton n’attend qu’une chose : qu’on l’appuie ! Joyeux codage !

## ÉTAPE 1
**Planifie ton installation.**
Les Neopixels sont vraiment brillants, mais nécessitent un peu de réflexion. Chaque Neopixel est adressable individuellement : quelle couleur veux-tu ? Où doit-elle apparaître sur la bande ? Combien de temps doit-elle rester allumée ? D’autres questions à se poser :

- Combien de Neopixels as-tu besoin ?
- Quelle intensité lumineuse ?
- La lumière doit-elle être diffusée ?
- Faut-il utiliser une bande, un anneau, un modèle nu, un montage sur breadboard, ou autre chose ?
- Ton installation doit-elle être permanente ? Utiliseras-tu les pinces Gator de la b.Board, les borniers à vis ou soudes-tu directement ?
- À quelle distance le bouton G doit-il être de ta b.Board ?
- Autres idées...

## ÉTAPE 2
**Quel est le < HELLO WORLD / > de ton projet ?**
Quand tu prototyperas ton code, commence par quelque chose de simple et fiable. Ton code final sera peut-être très complexe – pas de panique – motive-toi avec un petit ensemble de blocs pour faire démarrer ton projet.

## Initialiser les Neopixels
Aussi brillants que puissent te paraître ta micro:bit et ta b.Board, elles ne peuvent pas deviner la présence des Neopixels. Il ne suffit pas de les brancher aux pinces Gator et d’allumer la carte. Tu dois indiquer à ta micro:bit et à ta b.Board où sont les Neopixels, combien sont en série, et quel est leur type.
Pour cela, suis les étapes suivantes :

1. Clique sur la catégorie ``||Neopixel||`` pour afficher les options. Voici un exemple de configuration :

![enter image description here](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/button-g/neopixel_start_basic.png)

<!-- ![enter image description here](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/button-g/neopixel_start_basic.png?raw=true) -->

2. Choisis un motif lumineux simple pour vérifier si ta bande est bien initialisée. Par exemple :

```blocks
let strip = neopixel.create(DigitalPin.P0, 24, NeoPixelMode.RGB)
strip.setBrightness(100)
basic.forever(function () {
if (input.buttonIsPressed(Button.A)) {
strip.showColor(neopixel.colors(NeoPixelColors.Purple))
} else {
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
}
})
```

3. Si tout est bien codé, la bande doit s’illuminer en bleu, et passer au violet lorsque ``||Button A: Is Pressed||``.
**REMARQUE:** Si ta b.Board fonctionne avec des piles, réduis la ``||luminosité des Neopixels||`` pour éviter de les changer toutes les heures. Admire ce violet éclatant !

## ÉTAPE 3
** Clique vers un vrai Bouton G**
Appuyer sur ``||Button A||`` de la micro:bit, c’est bien. Mais tu sais ce qui est encore mieux ? Utiliser la vraie ClickBoardTM Bouton G.

<!-- ![alt text](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/button-g/glowy.gif?raw=true "For more info: www.brilliantlabs.ca") -->
![alt text](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/button-g/glowy.gif "For more info: www.brilliantlabs.ca")

Ce bouton fonctionne avec un code similaire à celui du ||Button A||. Pense à la distance que tu veux entre ton bouton et la b.Board. Tu peux utiliser notre future carte d’extension ou un Shuttle Click.

Voici un exemple de code :

```blocks
let ButtonG2 = ButtonG.createButtonG(BoardID.zero, ClickID.A)
let strip = neopixel.create(DigitalPin.P0, 30, NeoPixelMode.RGB)
strip.setBrightness(100)
basic.forever(function () {
    if (ButtonG2.getSwitch() == 1) {
        strip.showColor(neopixel.colors(NeoPixelColors.Purple))
    } else {
        strip.showColor(neopixel.colors(NeoPixelColors.Blue))
    }
})
```
## Quelques rappels en utilisant les blocs pour le Bouton G :
1. L’état enfoncé/appuyé du bouton correspond à 0/1.
2. Utilise la catégorie ||Logique|| pour trouver la fonction d’égalité.
3. Vérifie bien la position de la ClickBoard utilisée sur ta b.Board.
4. Essaie les blocs lumineux pour rendre ton installation encore plus brillante.
<!-- ![alt text](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/button-g/button_g_click.png?raw=true "For more info: www.brilliantlabs.ca")-->
![alt text](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/button-g/button_g_click.png "For more info: www.brilliantlabs.ca")

## BONNE FABRICATION
N’oublie pas de tweeter tes projets @brilliant_labs avec le hashtag #makeSomethingBrilliant.

---
---

## Keylock


<!-- ![Keylock Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/keylock/keylock.jpg?raw=true "Keylock Click")-->

![Keylock Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/keylock/keylock.jpg "Keylock Click")

## Description

Ce mécanisme de verrouillage Keylock Click BoardTM possède une serrure intégrée pouvant être utilisée comme interrupteur d'entrée. Il est fourni avec deux clés qui peuvent devenir votre propre point d'accès unique pour votre code. Utilisez notre port d'extension pour placer le keylock où vous en avez besoin. Ce capteur d'entrée dispose également de 3 positions de clé : 0-2.

<!-- ![Keylock Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/keylock/keylock-click.jpg?raw=true "Keylcok Click")-->

![Keylock Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/keylock/keylock-click.jpg "Keylock Click")

## Exemple de Code

Cet exemple utilise le Keylock Click connecté au MikroBus #1 de la b.Board.

Le keylock dispose de 3 positions !

Trouvez le Keylock dans le groupe Boutons & interrupteurs des Clickboards.

```blocks
let Keylock2 = Keylock.createkeylock(BoardID.zero, ClickID.A)
basic.forever(function () {
    if (Keylock2.getLockPosition() == 0) {
        basic.showIcon(IconNames.No)
    } else if (Keylock2.getLockPosition() == 1) {
        basic.showIcon(IconNames.Yes)
    } else if (Keylock2.getLockPosition() == 2) {
        basic.showIcon(IconNames.Heart)
    }
})
```

## Idée de Projet

PROTÉGEZ VOTRE PROJET

Soyez le seul à pouvoir exécuter votre expérience, allumer votre robot ou même entrer dans votre laboratoire de savant fou avec ce Keylock Click.

<!-- ![Keylock](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/keylock/keylock-gif.gif?raw=true "Let's Keep things locked") -->

![Keylock](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/keylock/keylock-gif.gif "Let's Keep things locked")


---
---

## Relais

<!-- ![Relay](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/relay/relay.png?raw=true "Relay") -->

![Relay](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/relay/relay.png "Relay")

## Description
Contrôle une large gamme d'appareils à forte puissance. Vous avez un jouet alimenté par batterie que vous souhaitez rendre intelligent ? Cette carte le permet.

FAITES TRÈS ATTENTION LORSQUE VOUS TRAVAILLEZ AVEC DE HAUTES TENSIONS. CE PRODUIT DOIT ÊTRE UTILISÉ SOUS LA SUPERVISION D'UN ADULTE.

<!-- ![Relay](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/relay/relay-click.jpg?raw=true "Relay Click") -->
![Relay](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/relay/relay-click.jpg "Relay Click")


## Exemple de Code


Cet exemple utilise le Relay Click connecté au MikroBus #1 de la b.Board.
Trouvez les blocs ``|| Relay ||``

```blocks
input.onButtonPressed(Button.A, function () {
    Relay2.relayOnOff(Relay.onOff.On, Relay.relay.Relay1)
})
input.onButtonPressed(Button.B, function () {
    Relay2.relayOnOff(Relay.onOff.Off, Relay.relay.Relay1)
})
let Relay2: Relay.Relay = null
Relay2 = Relay.createRelay(BoardID.zero, ClickID.A)
```

## Idée de Projet


TRANSFORMEZ VOTRE JOUET

Complétez ou interrompez un circuit avec le Relay Click BoardTM. Cette carte astucieuse agit comme un interrupteur on/off pour tous vos besoins en circuits. Combinez-la avec un Click BoardTM WiFi BLE pour offrir un contrôle à distance où que vous soyez connecté à Internet.


<!-- ![Relay](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/relay/relayclick-gif.gif?raw=true "Let's Keep things nifty") -->

![Relay](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/relay/relayclick-gif.gif "Let's Keep things nifty")
<!-- 
##### [🔙 Back Menu](#control) 
-->

## Servo
<!-- ![Servo Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servoinside.jpg?raw=true "Servo Click") -->
![Servo Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/servo/servoinside.jpg "Servo Click")

## Description
Vous avez remarqué que votre b.Board dispose de 6 connecteurs servo 5V intégrés, mais seulement 3 sont utilisables en même temps ? Votre projet nécessite encore plus de servos ? Cette carte vous offre 16 connecteurs servo !

<!-- ![Servo Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servoarm.jpg?raw=true "Servo Click") -->
![Servo Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/servo/servoarm.jpg "Servo Click")

Assurez-vous simplement que votre b.Board est alimentée via un adaptateur secteur. Connectez jusqu'à 30 Servo Click supplémentaires en chaîne via le port d'extension de la b.Board pour contrôler plus de 500 servos !
<!-- ![Servo Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servo-click.jpg?raw=true "Servo Click") -->
![Servo Click](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/servo/servo-click.jpg "Servo Click")
## Exemple de Code

Cet exemple utilise le Servo Click connecté au MikroBus #1 de la b.Board.

Vous pouvez placer les blocs du Servo Click pour faire bouger vos servos comme vous le souhaitez !

let Servo2 = Servo.createServo(BoardID.zero, ClickID.A)
```blocks
let Servo2 = Servo.createServo(BoardID.zero, ClickID.A)
input.onButtonPressed(Button.A, function () {
    Servo2.setServoAngle(1, 120)
    Servo2.setServoAngle(8, 90)
    Servo2.setServoAngle(16, 180)
    basic.pause(1000)
    Servo2.setServoAngle(1, 40)
    Servo2.setServoAngle(8, 120)
    Servo2.setServoAngle(16, 0)
})
```

















































## Idée de Projet

Art interactif !

Faites bouger votre monde, et votre art, avec le Servo Click ultime ! Cette carte peut contrôler 16 moteurs servo. Les possibilités sont infinies, et les projets collaboratifs sont encouragés ! Essayez de créer une œuvre d'art en mouvement avec vos amis. Plutôt branché robotique ? Le Servo Click est votre compagnon idéal pour contrôler 16 servos simultanément !





<!-- ![Servo](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/servo/servogif.gif?raw=true "Let's Keep things moving") -->
![Servo](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/servo/servogif.gif "Let's Keep things moving")




---
---


## Moteur
<!-- ![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/dcmotor.jpg?raw=true "Motor Click 3") -->
![Motor Click 3](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/motor-click-3/dcmotor.jpg "Motor Click 3")

## Description

Ce pilote de moteur vous permettra d’utiliser n’importe quel moteur DC que vous pourriez avoir dans votre makerspace. Les moteurs peuvent être plus grands que les moteurs jaunes souvent fournis avec les petits robots.

<!-- ![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/gearmotor.jpg?raw=true "Motor Click 3") -->
![Motor Click 3](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/motor-click-3/gearmotor.jpg "Motor Click 3")

Avec une capacité de sortie de 3,5 A sous 30V, vous pouvez utiliser des moteurs de très grande taille.

<!-- ![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/dcpower.png?raw=true "Motor Click 3") -->
![Motor Click 3](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/motor-click-3/dcpower.png "Motor Click 3")

Assurez-vous simplement de récupérer du 5V depuis le rail servo de la b.Board ou d'une autre source d'alimentation à l'aide d’un câble jumper.

<!-- ![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/motor-3-click.jpg?raw=true "Motor Click 3") -->


![Motor Click 3](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/motor-click-3/motor-3-click.jpg "Motor Click 3")







## Exemple de Code

Cet exemple utilise le Motor 3 Click connecté au MikroBus #1 de la b.Board.

Nous pouvons placer les blocs du Motor Click 3 où et comme vous le souhaitez pour faire bouger un moteur DC. Cela peut être déclenché par un bouton, une condition IF / ELSE, ou tout autre déclencheur.

```blocks
input.onButtonPressed(Button.A, function () {
    DC_Motor3.motorSpeedDirection(100, DC_Motor3.MotorDirection.Forward, clickBoardID.one)
    basic.pause(2000)
    DC_Motor3.motorSpeedDirection(0, DC_Motor3.MotorDirection.Reverse, clickBoardID.one)
})

```

## Idée de Projet

Il fait chaud ici ! Pouvez-vous utiliser le capteur de température du micro:bit ou le Temp Log 2 Click pour activer un ventilateur avec le Motor 3 Click ? Ou faire avancer une voiture avec un moteur à engrenage ?

<!-- ![Motor Click 3](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/motor-click-3/fangif.gif?raw=true "Let's Keep things spinning") -->
![Motor Click 3](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/motor-click-3/fangif.gif "Let's Keep things spinning")


---
---
## Mini LCD
<!-- ![NFC](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/lcd-mini/simplestLCD.jpg?raw=true "LCD MINI") -->
![NFC](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/lcd-mini/simplestLCD.jpg "LCD MINI")


## Description

Ce petit écran LCD à deux lignes vous permet d’afficher jusqu’à 16 caractères sur 2 lignes différentes. Utilisez-le pour ajouter un retour textuel à votre projet.

<!-- ![LCD MINI](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/lcd-mini/lcd-mini-click.jpg?raw=true "LCD MINI Click") -->
![LCD MINI](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/lcd-mini/lcd-mini-click.jpg "LCD MINI Click")



## Exemple de Code

Cet exemple utilise le LCD MINI Click connecté au MikroBus #1 de la b.Board.

Envoyez simplement vos textes, chaînes et valeurs d'entrée à votre écran LCD MINI à l’aide des blocs LCD Mini, ou convertissez toute valeur ou réponse que vous souhaitez afficher sur l’écran.

L’écran dispose de 2 lignes pouvant chacune afficher jusqu’à 16 caractères.

Le LCD MINI vous aide à afficher des données et des mots sur un écran LCD.

Trouvez les blocs LCD_MINI

```blocks
let LCDSettings = LCD_Mini.createLCDSettings(BoardID.zero, ClickID.A)
basic.forever(function () {
    LCDSettings.lcd_writeString("Hello", LCD_Mini.lineNumber.one)
    LCDSettings.lcd_writeString("World", LCD_Mini.lineNumber.two)
    basic.pause(1000)
    LCDSettings.lcd_clearDisplay()
})
```

## Idée de Projet

HAÏKU INTERACTIF

Le format d’un haïku est déjà parfait pour ce mini écran LCD. Créez un projet utilisant plusieurs Click Boards pour permettre d’interagir et de modifier le ton de votre haïku en fonction d’un facteur externe. Génial !

<!-- ![Noise](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/lcd-mini/lcdgif.gif?raw=true "Let's Keep things noisy") -->



![Noise](https://raw.githubusercontent.com/Brilliant-Labs/bboard-tutorials-v3/master/lcd-mini/lcdgif.gif "Let's Keep things noisy")



---
---