
#1_CONNEXION

Il est temps de se connecter au Wi-Fi de __Cyberville__. __Cyberville__ est une représentation futuriste vraiment cool développée par les incroyables équipes de Brilliant Labs. Dans cette Cyberville, tous les clients ou b.Boards sont connectés au réseau Wi-Fi de Cyberville. Le service Wi-Fi de __Cyberville__ est fourni par le module M5Core2, qui créera le point d'accès Wi-Fi 📳 appelé __Cyberville #?__. Connectons-nous pour appartenir à __Cyberville!__.

## Description de l'activité
Les __*🧑‍🎓 élèves*__ doivent être capables de se connecter au point d'accès Wi-Fi de Cyberville créé par l'enseignant 🧑‍🏫 __*professeur*__.

*Commençons !*

## __🧑‍🏫 Enseignants :__
Pour établir le point d'accès 📳 nécessaire, il est essentiel d'utiliser le module M5Core2, car cela facilitera la configuration requise. L'activité __Networking_BL_FR__, qui se trouve dans le module M5Core2, doit être sélectionnée et chargée.
Il est important de fournir aux élèves le nom et le numéro du point d'accès qui a été créé.
Il peut être utile de partager votre adresse MAC 🆔 et votre adresse IP 📮 générées par le module M5Core2 avec les élèves, car cela leur donnera une représentation visuelle du format.

### Nom du point d'accès - Numéro de Cyberville
Notez que __nous n'utiliserons pas de mot de passe__ pour cette activité, car le numéro de Cyberville changera à chaque redémarrage du M5Core2.
![CybervilleNumb](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/CybervilleNumb.png?raw=true "Cyberville Number for Access Point")

## __🧑‍🎓 Élèves :__
__1.__ Créez un nouveau projet en utilisant le Microbit
V2, en vous assurant d'utiliser une __b.Board V.1.4__, et nommez-le Networking_A.

![Step1](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step1.png?raw=true "Step1") 

__2.__ Utilisez le bloc Connect to WiFi:( ) with Password:( ) et placez-le à l'intérieur du bloc On Start.

__3.__ Assurez-vous d'utiliser exactement le même nom de Wi-Fi tel qu'il apparaît sur le M5Core2. Demandez les bonnes informations à l'enseignant 🧑‍🏫.

![Step2](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step2.png?raw=true "Step2")  

__4.__ Créez un bloc conditionnel logique __si__ pour savoir quand vous êtes connecté. Utilisez une petite face souriante pour l'afficher sur le Microbit.

__5.__ Créez un autre bloc pour vous déconnecter du réseau. Vous pouvez utiliser *sur le logo appuyé*.

![Step3](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step3.png?raw=true "Step3")

__6.__ Allumez la b.Board et établissez la communication entre le PC, le Microbit
et la b.Board.

![Step4](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Step4.png?raw=true "Step4")

__7.__ Téléchargez le code et vérifiez le code de connexion et de déconnexion avec le point d'accès Wi-Fi du module M5Core2.

## __À quoi s'attendre ?__
Si vous obtenez un ✅, vous êtes connecté au point d'accès 📳.

<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true" alt="Connected_gif" title="Si vous obtenez un ✅, vous êtes connecté au point d'accès" width="300" />

Les élèves 🧑‍🎓 verront une face souriante 😃 s'ils sont connectés.
![Connected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected.png?raw=true "Connected")

ou une face triste 🙁 s'ils ne le sont pas.
Students will see smile face if they are connected.
![Disconnected](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Disconnected.png?raw=true "Disconnected")

En appuyant sur le logo du Microbit les élèves se déconnecteront du système.
Pour se reconnecter, il est nécessaire de modifier le code - soyez ingénieux - ou de redémarrer la b.Board.

## Exemple de code
Vous pouvez télécharger le code pour cette activité depuis `https://www.brilliantlabs.ca/documents/cybersec/Networking_A.hex`, le fichier sera dans l'historique de téléchargement récent, il suffit de le glisser-déposer dans un nouveau projet.

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