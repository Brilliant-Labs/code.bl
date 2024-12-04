
---
# ~avatar
_Veuillez lire attentivement l'activité et suivre les étapes fournies. Dans la section Exemple de Code, vous pourrez_ 📝 **Modifier** _le code exemple ou le_ ⬇️ **télécharger** _sur votre __b.Board__._  
N'oubliez pas de changer la langue dans ⚙️ `More...` > 🌎 `Languaje` > `Français` dans le coin supérieur droit.
# ~
---

# 2_Adresse MAC et IP

L'adresse de contrôle d'accès au média (adresse MAC) 🆔 est un numéro hexadécimal à 12 chiffres attribué à chaque appareil connecté à un réseau. Elle apparaît dans le format suivant:
### 34:ab:95:98
L'adresse MAC 🆔 est unique ; chaque ordinateur, téléphone, tablette, b.Board ou appareil électronique connecté à un réseau possède sa propre adresse MAC 🆔.

L'adresse IP est un numéro de protocole Internet 📮 utilisé pour permettre aux appareils de communiquer entre eux sur les réseaux. Elle sert à partager leurs emplacements pour la transmission de données. Une adresse IP mesure 32 bits et ressemble généralement à ceci:
### 192.168.4.2
Elle peut être privée ou publique.
Le module M5 attribuera une adresse IP 📮 à chaque __b.Board__ dans Cyberville, car il servira de point d'accès 📳.

Les adresses MAC 🆔 et IP 📮 travaillent ensemble au sein d'un réseau. L'adresse MAC 🆔 permet l'identification des appareils, tandis que l'adresse IP 📮 fournit l'emplacement nécessaire à l'envoi et à la réception des données.

## Activité :
### Trouver l'adresse MAC 🆔 et l'adresse IP 📮 du __b.Board__

Cette activité consiste à trouver l'adresse MAC 🆔 et l'adresse IP 📮 de chaque __b.Board__. Les étudiants publieront ces informations sur une étiquette ou une carte d'identité de __Cyberville__. Ainsi, les étudiants 🧑‍🎓 pourront identifier ces adresses comme uniques et propres à __Cyberville__ lorsqu'ils effectuent des comparaisons entre elles, et cela sera utile pour les reconnaître dans le réseau.

De plus, les enseignants 🧑‍🏫 et les étudiants 🧑‍🎓 doivent publier les adresses MAC et IP sur la carte d'identité de __Cyberville__:

🧑‍🏫 Carte d'identité des enseignants
Téléchargez la carte d'identité pour les enseignants 🧑‍🏫 [__⬇️ Ici__](https://drive.google.com/file/d/1EnfeuJK2KT-1-K8Pp-kZ2VPfwaLjvDFZ/view?usp=sharing)

### 🧑‍🎓 Carte d'identité des étudiants
Téléchargez la carte d'identité pour les étudiants 🧑‍🎓 [__⬇️ Ici__](https://drive.google.com/file/d/1L_Q3F4pbEFy0FwHtw97My_tA7F-5hCj-/view?usp=sharing)

Voici un exemple de ce à quoi s'attendre pour cette activité:
<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Example_EN.png?raw=true" alt="ID" title="ID Example." width="300" />
![ID Example](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Example_EN.png?raw=true "ID Example")  

*Commençons !*

__1.__ Allez sur https://code-alpha.brilliantlabs.ca/ et créez un nouveau projet ou utilisez le projet Cyber_Network créé dans l'activité précédente.

__2.__ Dans le projet, utilisez le bloc 🧩``||lorsque le bouton A est presse||``.

__3.__ Remplacez le texte "Hello!" dans le 🧩``||afficher texte||`` par le bloc 🧩[Obtenir I’MAC du b.Board]. Il est situé dans les "blocs de b.Board" en "CyberSecurity".

![Step5](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step5_FR.png?raw=true "Step 3")

__4.__ Ajoutez un nouveau bloc 🧩``||lorsque le bouton A est presse||``, mais cette fois sélectionnez "lorsque le bouton B est presse".

__5.__ Remplacez le texte "Hello!" dans le bloc 🧩``||afficher texte||`` par le bloc 🧩``||Obtenir I’IP du b.Board||``. Ce dernier se trouve sous "__b.Board__ blocks" dans "CyberSecurity".

![Step6](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step6_FR.png?raw=true "Step 5")

__6.__ Allumez le __b.Board__ et établissez la communication entre le PC, le micro:bit et le __b.Board__.

![Step7](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Step7_FR.png?raw=true "Download to microbit")

__7.__ ⬇️ Téléchargez le code sur le micro:bit.

__8.__ Les étudiants afficheront maintenant leur adresse MAC unique 🆔 sur l'écran du micro:bit en appuyant sur le bouton A, et l'adresse IP 📮 en appuyant sur le bouton B.

L'adresse MAC 🆔 sera affichée sur l'écran du micro:bit, de manière similaire à ceci (défilement ⏪):
__`Mon MAC : 34:ab:95:98:d1:f8`__
Et l'adresse IP 📮 sera affichée sur l'écran du micro:bit, de manière similaire à ceci (défilement ⏪):
__`Mon IP : 192.168.4.2`__

__9.__ À la fin de cette activité, les enseignants 🧑‍🏫 devraient discuter avec leurs étudiants 🧑‍🎓 de l'importance des adresses 🆔 MAC et 📮 IP pour la cybersécurité et le développement de __Cyberville__.

***  

📌 __*Remarques:*__

Si vous le souhaitez, vous pouvez également voir l'adresse 🆔 MAC et l'adresse 📮 IP sur le __*Show Console Appareil*__. 

### ~ avatar
*Une fois que vous avez téléchargé votre code...*
1. Cliquez sur le bouton de rafraîchissement 🔄 (icône de flèche circulaire) dans la fenêtre du simulateur.
2. __Attendez__ jusqu'à ce que le bouton *Show Console Appareil* apparaisse dans la fenêtre de sortie de la console.
3. Cliquez dessus.

![Console](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/Console_FR.png?raw=true "Console Device")
### ~


## Exemple de code
Vous pouvez télécharger le fichier .hex pour cette activité en cliquant [__⬇️ Ici__](https://www.brilliantlabs.ca/documents/cybersec/Networking_B.hex).
Une fois téléchargé, glissez-déposez-le dans un nouveau projet, ou cliquez sur l'icône **📝 Modifier** dans les modes de langage de programmation pour le modifier dans l'éditeur de 🧩 Blocs.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit_FR.png?raw=true "IconEdit")

_**`N'oubliez pas de configurer le nom et le mot de passe corrects pour le point d'accès. Coupez le son du PC pour écouter le son de la b.Board.`**_

Vous pouvez utiliser cet exemple de code pour obtenir les adresses 🆔 MAC et 📮 IP.

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