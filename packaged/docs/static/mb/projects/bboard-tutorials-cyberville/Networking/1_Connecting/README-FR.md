# 1_CONNEXION

Il est temps de se connecter au réseau Wi-Fi de __Cyberville__. __Cyberville__ est une ville fictive futuriste développée par l'équipe géniale de Brilliant Labs. Dans __Cyberville__, tous les clients ou b.Boards sont connectés au réseau Wi-Fi de __Cyberville__. Le service Wi-Fi à __Cyberville__ est fourni par le module M5Core2, qui crée le point d'accès Wi-Fi 📳 appelé "Cyberville #?". Connectons-nous au réseau __Cyberville__.

## Description de l'activité
Les 🧑‍🎓 étudiants devraient être capables de se connecter au point d'accès Wi-Fi de __Cyberville__ créé par le 🧑‍🏫 enseignant.

*Commençons !*
## 🧑‍🏫 Enseignants :
Pour établir le point d'accès 📳 requis, il est essentiel d'utiliser le module M5Core2, car cela facilitera la connexion nécessaire. L'activité __Networking_BL_EN__, qui se trouve dans le module M5Core2, doit être sélectionnée et chargée.

#### ~avatar
Il est essentiel que les étudiants reçoivent le nom et le numéro du point d'accès qui a été créé.
#### ~

Il peut être utile de partager votre adresse MAC 🆔 et votre adresse IP 📮 générées par le module M5Core2 avec les étudiants, car cela leur fournira une représentation visuelle du format.

#### Nom du point d'accès - Numéro de Cyberville
Notez que nous n'utiliserons pas de mot de passe pour cette activité, car le numéro de __Cyberville__ changera chaque fois que vous redémarrez le M5Core2.
![CybervilleNumb](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/CybervilleNumb_FR.png?raw=true "Cyberville Number for Access Point")

## __🧑‍🎓 Étudiants:__
__1.__ Créez un nouveau projet en utilisant le micro:bit V2, en vous assurant que vous travaillez avec une __b.Board Rev 1.4__ et en le nommant "Networking_A". Vous pouvez trouver des instructions sur la façon d’identifier la version matérielle et logicielle de votre b.Board [ici](https://drive.google.com/file/d/1g5fHso1ON-yVFHqaRRCifrU2X1WU_6qf/view?usp=sharing).

![Step1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step1_FR.png?raw=true "Step1") 

__2.__ Utilisez le bloc 🧩[Connexion au WiFi:( ) avec mot de passe:( )] et placez-le dans le bloc 🧩[On Start].

__3.__ Assurez-vous d'utiliser le nom Wi-Fi exact tel qu'il apparaît sur le M5Core2. Demandez les informations correctes à l'enseignant 🧑‍🏫.

![Step2](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step2_FR.png?raw=true "Step2")  

__4.__ Utilisez le bloc conditionnel logique __"si"__ pour vérifier si vous êtes connecté. Si vous êtes connecté, affichez un visage souriant 😃 sur le micro:bit avec le bloc 🧩[afficher texte].

__5.__ Ensuite, créez un autre bloc 🧩 pour vous déconnecter du réseau. Vous pouvez utiliser le bloc d'entrée 🧩[sur le logo appuye] pour cela et placer le bloc 🧩[Deconnexion du WiFi] à l'intérieur. Ajoutez également un bloc 🧩[montrer l'icone] après la déconnexion pour afficher un visage triste 🙁 après la déconnexion.

![Step3](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step3_FR.png?raw=true "Step3")

__6.__ Allumez le b.Board et établissez la communication entre le PC, le micro:bit et le b.Board.

![Step4](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step4_FR.png?raw=true "Step4")

__7.__ Téléchargez le code et vérifiez le code de connexion et de déconnexion avec le point d'accès Wi-Fi du module M5Core2.

## __À quoi s'attendre ?__
Lorsque les étudiants 🧑‍🎓 utilisent le bloc 🧩[Connexion au WiFi:( ) avec mot de passe:( )], une coche clignotante ✅ apparaîtra comme test d'initialisation, indiquant qu'ils sont connectés au point d'accès 📳. Si le micro
affiche une ❎, cela signifie que la connexion a échoué.

<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true" alt="Connected_gif" title="Si vous obtenez un ✅, vous êtes connecté au point d'accès" width="300" />

Les étudiants 🧑‍🎓 verront un visage souriant 😃 s'ils sont connectés.
![Connected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_FR.png?raw=true "Connected")

ou une face triste 🙁 s'ils ne le sont pas.
Students will see smile face if they are connected.
![Disconnected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Disconnected_FR.png?raw=true "Disconnected")

En appuyant sur le logo du Microbit les élèves se déconnecteront du système.
Pour se reconnecter, il est nécessaire de modifier le code - soyez ingénieux - ou de redémarrer la b.Board.

## Exemple de code

Vous pouvez télécharger le code pour cette activité depuis `https://www.brilliantlabs.ca/documents/cybersec/Networking_A.hex` le fichier sera dans l'historique de téléchargement récent, il suffit de le glisser-déposer dans un nouveau projet.

Ou utilisez cet exemple de code pour connecter la b.Board au point d'accès du module M5Core2 📳.

__*N'oubliez pas de configurer le nom correct du point d'accès. Coupe le son du PC pour écouter le son du b.Board.*__

```blocks
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    Cybersec.Disconnect()
    basic.showIcon(IconNames.Sad)
})
Cybersec.WifiConnect("Cyberville #?", "")
if (Cybersec.WiFi_Connected()) {
    basic.showIcon(IconNames.Happy)
}
```