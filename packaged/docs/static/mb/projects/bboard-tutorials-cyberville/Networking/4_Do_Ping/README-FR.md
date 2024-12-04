
---
# ~avatar
_Veuillez lire attentivement l'activité et suivre les étapes fournies. Dans la section Exemple de Code, vous pourrez_ 📝 **Modifier** _le code exemple ou le_ ⬇️ **télécharger** _sur votre __b.Board__._  
N'oubliez pas de changer la langue dans ⚙️ `More...` > 🌎 `Languaje` > `Français` dans le coin supérieur droit.
# ~
---

# 4_PINGUER

Maintenant que le réseau __Cyberville__ est opérationnel et que tout le monde a un rôle, il est temps de découvrir s'il y a quelqu'un de spécial sur le réseau. Pour cela, nous allons utiliser la commande "__ping__."

Un __"ping"__ est un programme Internet simple qui vous permet de tester et de vérifier si une adresse __IP__ particulière existe et peut accepter des requêtes dans le réseau __Cyberville__. C'est vraiment facile à utiliser ! Un autre avantage du __ping__ est qu'il vous indique si une autre carte essaie de vous joindre et si cela fonctionne correctement. Utilisons la commande __"ping"__ pour découvrir si d'autres rôles sont présents dans le réseau __Cyberville__ !

## Activité
Vérifions rapidement si le point d'accès 📳 M5 Module est disponible. Il suffit de faire un __Ping__, et nous le saurons en un rien de temps ! Il a une adresse IP par défaut pratique de 192.168.4.1, idéale pour commencer avec la commande PING !
Ce serait vraiment amusant de partager nos cartes d'identité et de découvrir à qui nos camarades de classe sont connectés ! N'oubliez pas de configurer les adresses IP de vos amis dans le bloc 🧩 ``||Effectuez un PING vers l'IP("")||``, et assurez-vous d'être connecté au bon point d'accès 📳.
Vous obtiendrez un 😊 visage souriant si votre rôle de demande est disponible sur le réseau, et un 😔 visage triste si ce n'est pas le cas.

## Exemple de code
You can download the .hex file for this activity by clicking [__⬇️ Here__](https://www.brilliantlabs.ca/documents/cybersec/Networking_D.hex). 
Once downloaded, either drag and drop it into a new project, or click the **📝 Edit** icon in the programming language modes to modify it in the 🧩 Blocks editor.
![IconEdit](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Passwords/2_Seq_to_Access/IconEdit.png?raw=true "IconEdit")

_**`N'oubliez pas de configurer le nom et le mot de passe corrects pour le point d'accès. Coupez le son du PC pour écouter le son de la b.Board.`**_

Ou utilisez cet exemple de code pour __pinguer__ vos amis.

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```