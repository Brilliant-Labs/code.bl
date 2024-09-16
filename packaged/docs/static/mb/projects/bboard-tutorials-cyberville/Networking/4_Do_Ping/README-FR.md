# 4_Pinguer

Maintenant que le réseau __Cyberville__ est opérationnel et que tout le monde a un rôle, il est temps de découvrir s'il y a quelqu'un de spécial sur le réseau. Pour cela, nous allons utiliser la commande "__ping__."

Un __"ping"__ est un programme Internet simple qui vous permet de tester et de vérifier si une adresse __IP__ particulière existe et peut accepter des requêtes dans le réseau __Cyberville__. C'est vraiment facile à utiliser ! Un autre avantage du __ping__ est qu'il vous indique si une autre carte essaie de vous joindre et si cela fonctionne correctement. Utilisons la commande __"ping"__ pour découvrir si d'autres rôles sont présents dans le réseau __Cyberville__ !

## Activité
Vérifions rapidement si le point d'accès 📳 du module M5Core2 est disponible en faisant un __Ping__. Il a une adresse IP 📮 par défaut pratique de 192.168.4.1, parfaite pour commencer !
Il serait amusant d'échanger nos cartes d'identité et de découvrir à qui nos camarades de classe sont liés. 

## Exemple de code
Vous pouvez télécharger le code pour cette activité depuis `https://www.brilliantlabs.ca/documents/cybersec/Networking_D.hex`. Le fichier sera dans l'historique des téléchargements récents, il suffit de le glisser et déposer dans un nouveau projet.

Ou utilisez cet exemple de code pour __pinguer__ vos amis.

__*N'oubliez pas de configurer correctement le nom du point d'accès. Coupez le son du PC pour écouter le son du b.Board.*__

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```