
---
# ~avatar
_Veuillez lire attentivement l'activité et suivre les étapes fournies. Dans la section Exemple de Code, vous pourrez_ 📝 **Modifier** _le code exemple ou le_ ⬇️ **télécharger** _sur votre __b.Board__._  
N'oubliez pas de changer la langue dans ⚙️ `More...` > 🌎 `Languaje` > `Français` dans le coin supérieur droit.
# ~
---

# 3_Rôles

Dans cette activité, vous prendrez un rôle à Cyberville afin de pouvoir la protéger des cyberattaques.

## Activité :
### Prendre un rôle dans Cyberville

*Commençons !*

__1.__ Remplis ta carte d'identité __Cyberville__ avec les noms, adresses MAC 🆔 et adresses IP 📮.

__2.__ Acquiers une identité en choisissant un rôle au sein de __Cyberville__.

__3.__ Programmez le micro:bit pour que votre icône soit toujours affichée sur l'écran du micro
afin d'indiquer que vous êtes connecté au réseau Wi-Fi __Cyberville__.

__4.__ Programmez le micro:bit pour qu'il joue un son ou une mélodie (vous pouvez le trouver dans les blocs de musique) si vous n'êtes pas connecté au réseau Wi-Fi __Cyberville__.

Veuillez choisir l'un des rôles suivants dans __Cyberville__:
![Rol](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol_FR.png?raw=true "Rol")

Par exemple, si vous choisissez __💧 EAU__ et que vous êtes connecté au réseau Wi-Fi, alors votre micro:bit devrait ressembler à ceci :

![Step10](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Step10_FR.png?raw=true "Step10")

Une fois que chaque __b.Board__ dans la classe est reliée à __Cyberville__ et qu'un rôle lui est attribué, c'est le moment amusant ! Ton enseignant va simuler une __Cyberattaque__ en désactivant le module M5, qui est le fournisseur Wi-Fi de __Cyberville__. Cela déconnectera tous les appareils dans __Cyberville__, créant une situation de chaos au sein du réseau __Cyberville__!

## Exemple de code
Vous pouvez télécharger le fichier .hex pour cette activité en cliquant sur [__⬇️ Ici__](https://www.brilliantlabs.ca/documents/cybersec/Networking_C.hex).
Une fois téléchargé, glissez-déposez-le dans un nouveau projet, ou cliquez sur l'icône **📝 Modifier** dans les modes de langage de programmation pour le modifier dans l'éditeur 🧩 Blocks.
![IconeModifier](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit_FR.png?raw=true "IconeModifier")

_**`N'oubliez pas de configurer le nom et le mot de passe corrects pour le point d'accès. Coupez le son du PC pour écouter le son de la b.Board.`**_

Ou utilise cet exemple de code pour savoir si tu as un __rôle actif 👤__ dans __Cyberville__.

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