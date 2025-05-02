#📒 Tutoriel b.Board - Clickboards :

# `CONTRÔLE`

- [Button G](#button-g) 
- [Keylock](#keylock) 
- [Relay](#relay) 
- [Servo](#servo)
- [Motor](#motor)
- [Mini LCD](#mini-lcd)
---

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

Clique sur la catégorie ||Neopixel|| pour afficher les options. Voici un exemple de configuration :


Choisis un motif lumineux simple pour vérifier si ta bande est bien initialisée. Par exemple :

blocks
Copy
Edit
let strip = neopixel.create(DigitalPin.P0, 24, NeoPixelMode.RGB)
strip.setBrightness(100)
basic.forever(function () {
    if (input.buttonIsPressed(Button.A)) {
        strip.showColor(neopixel.colors(NeoPixelColors.Purple))
    } else {
        strip.showColor(neopixel.colors(NeoPixelColors.Blue))
    }
})
Si tout est bien codé, la bande doit s’illuminer en bleu, et passer au violet lorsque ||Button A: Is Pressed||.
REMARQUE : Si ta b.Board fonctionne avec des piles, réduis la ||luminosité des Neopixels|| pour éviter de les changer toutes les heures. Admire ce violet éclatant !


ÉTAPE 3
Clique vers un vrai Bouton G
Appuyer sur ||Button A|| de la micro:bit, c’est bien. Mais tu sais ce qui est encore mieux ? Utiliser la vraie ClickBoardTM Bouton G.



Ce bouton fonctionne avec un code similaire à celui du ||Button A||. Pense à la distance que tu veux entre ton bouton et la b.Board. Tu peux utiliser notre future carte d’extension ou un Shuttle Click.

Voici un exemple de code :

blocks
Copy
Edit
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
Quelques rappels en utilisant les blocs pour le Bouton G :
L’état enfoncé/appuyé du bouton correspond à 0/1.

Utilise la catégorie ||Logique|| pour trouver la fonction d’égalité.

Vérifie bien la position de la ClickBoard utilisée sur ta b.Board.

Essaie les blocs lumineux pour rendre ton installation encore plus brillante.



BONNE FABRICATION
N’oublie pas de tweeter tes projets @brilliant_labs avec le hashtag #makeSomethingBrilliant.

🔙 Retour au menu