# 3_Rôles.

Pour compléter cette activité, tu dois acquérir un rôle dans Cyberville afin de la protéger contre les cyberattaques.

## Activité :
### Prendre un rôle dans Cyberville

*Commençons !*

__1.__ Remplis ta carte d'identité __Cyberville__ avec les noms, adresses MAC 🆔 et adresses IP 📮.

__2.__ Acquiers une identité en choisissant un rôle au sein de __Cyberville__.

__3.__ Développe un code où ton icône est toujours affichée sur l'écran du Microbit pour indiquer que tu es connecté au Wi-Fi dans __Cyberville__.

__4.__ Programme le Microbit pour jouer un son ou démarrer une mélodie (tu peux la trouver dans les blocs musique) si tu n'es pas connecté à __Cyberville__.

Rappelle-toi, ton rôle dans __Cyberville__ peut être l'une des entités importantes suivantes :
![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "Rol")

Voici à quoi cela pourrait ressembler pour quelqu'un qui choisit __WATER__ et est connecté.

![Step10](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Step10.png?raw=true "Step10")

Une fois que chaque b.Board dans la classe est reliée à __Cyberville__ et qu'un rôle lui est attribué, c'est le moment amusant ! Ton enseignant va simuler une __Cyberattaque__ en désactivant le module M5, qui est le fournisseur Wi-Fi de __Cyberville__. Cela déconnectera tous les appareils dans __Cyberville__, créant une situation de chaos et une chute générale du réseau de __Cyberville__ !

## Exemple de code

Tu peux télécharger le code pour cette activité depuis `https://www.brilliantlabs.ca/documents/cybersec/Networking_C.hex`. Le fichier sera dans l'historique des téléchargements récents, il suffit de le glisser-déposer dans un nouveau projet.

Ou utilise cet exemple de code pour savoir si tu as un __rôle actif 👤__ dans __Cyberville__.

__*N'oublie pas de configurer le nom correct du point d'accès. Coupe le son du PC pour écouter le son du b.Board.*__

Voici un exemple de code pour configurer ton rôle 👤 :

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString(Cybersec.getMACaddressbBoard())
})
input.onButtonPressed(Button.B, function () {
    basic.showString(Cybersec.getIPaddressbBoard())
})
Cybersec.WifiConnect("Cyberville #?", "")
basic.forever(function () {
    if (Cybersec.WiFi_Connected()) {
        basic.showIcon(IconNames.Umbrella)
    } else {
        soundExpression.sad.play()
        basic.showIcon(IconNames.Sad)
    }
})
```
