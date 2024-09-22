
# 2_Adresse MAC et IP

L'adresse de contrôle d'accès média, ou adresse MAC 🆔, est un numéro hexadécimal à 12 chiffres attribué à chaque appareil connecté au réseau. L'adresse MAC 🆔 est unique. Chaque b.Board et module M5 dans le Cyber Security Kit en possède une.

L'adresse IP est un numéro de protocole Internet 📮 utilisé dans les réseaux pour permettre aux appareils de partager leurs emplacements. Elle est longue de 32 bits et peut être privée ou publique.
Le module M5 attribuera une adresse IP 📮 à chaque b.Board dans __Cyberville__ car il sera notre point d'accès.

Tout comme les adresses MAC 🆔 et IP 📮 fonctionnent ensemble dans le réseau, l'une identifie et l'autre localise.

## Activité :
### Trouver l'adresse MAC 🆔 et l'adresse IP 📮 de la b.Board
Cette activité consiste à trouver l'adresse MAC et l'adresse IP dans chaque b.Board connectée à __Cyberville__. Les élèves les publieront sur une étiquette ou une carte d'identité de __Cyberville__. Cela permettra aux élèves 🧑‍🎓 d'identifier ces adresses comme uniques et propres dans __Cyberville__ lorsqu'ils feront des comparaisons entre eux, et il sera utile de les reconnaître dans le réseau.

De plus, les enseignants 🧑‍🏫 et les élèves 🧑‍🎓 doivent publier les adresses MAC et IP sur la carte d'identité de __Cyberville__ :

### 🧑‍🏫 __*Carte d'identité des enseignants*__
Téléchargez la carte d'identité pour les enseignants 🧑‍🏫 
[Ici](https://drive.google.com/file/d/14gh8mT6u4rgxHwiSSV6rtSel3Gz4WwM_/view?usp=drive_link)

### 🧑‍🎓 __*Carte d'identité des élèves*___
Téléchargez la carte d'identité pour les élèves 🧑‍🎓 [Ici](https://drive.google.com/file/d/1uYi49zPMzKYuliF4TlS2NQBoPTkMTcoD/view?usp=drive_link)

Voici un exemple de ce à quoi s'attendre pour cette activité :
<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/IDbig.png?raw=true" alt="Exemple de carte d'identité" title="Exemple de carte d'identité" width="300" />

*Commençons !*

__1.__ Allez sur 'https://code-alpha.brilliantlabs.ca/' et créez un nouveau projet ou utilisez le projet Cyber_Network créé dans l'activité précédente.

__2.__ Dans le projet, utilisez le bloc on button A pressed.

__3.__ Remplacez le texte "Hello!" dans le bloc show string par le bloc Get the b.Board's MAC Address. Il est situé dans les blocs de b.Board en CyberSecurity.

![Step5](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step5.png?raw=true "Step 3")

__4.__ Ajoutez un nouveau bloc on button A pressed, mais cette fois sélectionnez on button B pressed.

__5.__ Remplacez le texte "Hello!" dans le bloc show string par le bloc Get the b.Board's IP Address. Il est situé dans les blocs de b.Board en CyberSecurity.

![Step6](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step6.png?raw=true "Step 5")

__6.__ Allumez la b.Board et établissez la communication entre le PC, le micro
et la b.Board.

![Step7](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step7.png?raw=true "Download to microbit")

__7.__ Téléchargez le code sur le Microbit.

__8.__ Les élèves afficheront maintenant leur adresse MAC 🆔 unique sur l'écran du micro
en appuyant sur le bouton A, et l'adresse IP 📮 en appuyant sur le bouton B.

L'adresse MAC 🆔 sera affichée sur l'écran du Microbit comme ceci (défilement ⏪) :

   Mon MAC : 34:ab:95:98:d1:f8

Et l'adresse IP 📮 sera affichée sur l'écran du Microbit
comme ceci (défilement ⏪) :

   Mon IP : “192.168.4.2”

__9.__ En fin de compte, les enseignants de 🧑‍🏫 devraient demander à leurs élèves de 🧑‍🎓 pourquoi les 🆔 adresses MAC et 📮 adresses IP sont cruciales pour la cybersécurité et le développement de __Cyberville__.

***  

📌 __*Remarques:*__

__*Une autre option pour voir vos informations :*__ 
Vous pouvez également voir l'adresse MAC et l'adresse IP sur le __*Show Console Appareil*__. ╔═══════════════════════════════════╗

*Une fois que vous avez téléchargé votre code...*

1. Cliquez sur le bouton de rafraîchissement 🔄 (icône de flèche circulaire) dans la fenêtre du simulateur.
2. __Attendez__ jusqu'à ce que le bouton *Show Console Appareil* apparaisse dans la fenêtre de sortie de la console.
3. Cliquez dessus.

![Console](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Console.png?raw=true "Console Device")
╚═══════════════════════════════════╝

## Exemple de code
Vous pouvez télécharger le code pour cette activité depuis `https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex`. Le fichier sera dans l'historique des téléchargements récents, il suffit de le glisser-déposer dans un nouveau projet.

Ou utilisez cet exemple de code pour obtenir les adresses MAC 🆔 et IP 📮.

__*N'oubliez pas de configurer le nom correct du point d'accès. Coupe le son du PC pour écouter le son du b.Board.*__

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString(Cybersec.getMACaddressbBoard())
})
input.onButtonPressed(Button.B, function () {
    basic.showString(Cybersec.getIPaddressbBoard())
})
Cybersec.WifiConnect("Cyberville #?", "")
basic.forever(function () {
	
})
```