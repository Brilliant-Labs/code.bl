# 6_FORCE DU SIGNAL

Salut ! Nous sommes sûrs que vous serez vraiment intéressé de savoir que l'emplacement de votre point d'accès Wi-Fi 📳 dans votre maison est super important pour la cybersécurité !

Dans cette activité, nous allons avoir une petite discussion sur la force du signal Wi-Fi. L'indicateur de force du signal reçu, ou __RSSI__, est une petite mesure pratique qui vous montre à quel point le signal que vous recevez est fort. Nous avons de bonnes nouvelles pour vous ! Notre b.Board dispose d'un module radio et d'un bloc pour lire la puissance générée par le point d'accès M5Core2 📳. Juste un petit rappel : RSSI est indiqué par une unité négative appelée dBm. Plus le nombre est élevé, meilleur est le signal ! Mais comment cela est-il lié à la cybersécurité ? À cause du point d'accès 📳 dans notre maison, nous pouvons être plus ou moins vulnérables pour nos __*données précieuses*__.

Voyons comment cela fonctionne, et n'oubliez pas de répondre au dernier test !

Nous sommes très heureux de partager certains des avantages incroyables de placer votre point d'accès au bon endroit !

__1.__ Réduction des fuites de signal 🙉 Lorsque votre point d'accès est au centre de votre maison, le signal Wi-Fi a moins de chances de s'étendre à l'extérieur, gardant vos informations privées en sécurité. C'est formidable car cela aide à empêcher les personnes que vous ne connaissez pas, comme vos voisins ou même des personnes mal intentionnées, de détecter et d'essayer d'accéder à votre réseau.

__2.__ Nous voulons tous garder nos maisons sûres et sécurisées, n'est-ce pas ? Eh bien, une façon de le faire est de contenir le signal à l'intérieur de votre maison. Cela aide à limiter les opportunités pour les attaquants 🙊 d'exploiter les vulnérabilités, comme tenter de pénétrer dans votre réseau Wi-Fi en utilisant des attaques par force brute sur le mot de passe.

__3.__ Un autre grand avantage est que vous pouvez contrôler l'accès 🙈 à votre réseau domestique. En centralisant le point d'accès, vous pouvez décider quelles zones de votre maison disposent de signaux Wi-Fi plus forts. Cela vous aide à décider stratégiquement où les appareils se connectent et qui a accès. Cela est particulièrement important lorsqu'il s'agit de sécuriser vos appareils IoT, qui pourraient être plus vulnérables aux attaques.

__4.__ Un autre grand avantage d'un point d'accès situé au centre 🐵 est qu'il facilite la surveillance de l'ensemble de votre réseau pour détecter toute activité suspecte. Cela est dû au fait qu'il peut suivre les connexions sur toute la zone de couverture de manière plus efficace.

__5.__ Gestion sécurisée des réseaux invités 🔧🐒 En plaçant votre point d'accès à un endroit central, vous pouvez facilement gérer vos réseaux invités en toute confiance. Ainsi, vos invités peuvent rester connectés dans une zone contrôlée de votre maison, tandis que vous pouvez vous détendre en sachant qu'ils n'accéderont à aucune partie sensible de votre réseau interne.

## Activité  

### 🧑‍🏫  __*Enseignants*__
Il incombe au personnel enseignant de fournir aux élèves un point d'accès 📳 en utilisant le module M5Core2 pour cette activité. L'activité de mise en réseau est le choix le plus approprié, car elle nécessite uniquement la création d'un point d'accès 📳.
Il est également nécessaire de partager avec les élèves les informations suivantes concernant __RSSI__ et la force du signal.
<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/6_Signal_Strength/RSSI.png?raw=true" alt="RSSI" title="RSSI" width="450" /> 
Pour déterminer la force du signal dans __Cyberville__,  l'enseignant 🧑‍🏫 doit sortir de la salle de classe ou s'éloigner des b.Boards.
Les élèves 🧑‍🎓 liront la force du signal en fonction de leur code et de la position de l'enseignant avec le M5Core2.

### 🧑‍🎓 __*Étudiants*__
__1.__ Connectez-vous au point d'accès Wi-Fi M5Core2 📳. L'enseignant doit fournir le nom du point d'accès et le mot de passe. Utilisez le bloc Connecter au WiFi. N'oubliez pas que cela devrait ressembler à ceci (✅ sur l'écran b.Board):
![Connected_gif](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/1_Connecting/Connected_gif.gif?raw=true "Connected_gif")  

Si vous obtenez un petit __x__ (❎ sur l'écran b.Board), vous __N'êtes PAS__ connecté.

__2.__ Utilisez un bloc *sur le bouton A pressé*, et à l'intérieur, ajoutez un bloc *montrer chaîne ()*.

__3.__ Trouvez le bloc *Obtenir la force du signal* dans les blocs de cybersécurité, et utilisez-le pour remplacer le mot *bonjour!* dans le bloc Montrer la Chaîne.

__4.__ Obtenez le niveau __RSSI__ et vérifiez la force du signal selon l'emplacement du point d'accès 📳, tirez vos propres conclusions sur le meilleur endroit pour obtenir un signal fort.

__5.__ Disons que c'est votre maison... Où placerez-vous votre point d'accès 📳 pour protéger vos __données précieuses__? [Télécharger](https://drive.google.com/file/d/1LNoaNRcknDB6Oy8KqP0S8L2PaEW8EaEH/view?usp=sharing), et imprimez les plans.

<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/6_Signal_Strength/House1.png?raw=true" alt="House1" title="House1" width="450" />

<img src="https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/ValuableData/6_Signal_Strength/House2.png?raw=true" alt="House2" title="House2" width="450" />

## Exemple de code

Vous pouvez télécharger le code pour cette activité à partir de `https://brilliantlabs.ca/documents/cybersec/RSSI.hex` Le fichier sera dans l'historique des téléchargements récents, il vous suffit de le glisser et de le déposer dans un nouveau projet.

Ou utilisez ce code comme exemple pour obtenir la puissance __RSSI__.

Assurez-vous toujours que vous êtes connecté au bon réseau __Cyberville__ avant d'essayer un nouveau code.

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString(Cybersec.getSignalStrength())
})
Cybersec.WifiConnect("Cyberville #2", "")
```