# Correction des couleurs BLiXel

Certains modules BLiXel sur certaines cartes b.Board affichent les couleurs de façon mélangée à cause d’une erreur du fabricant.  
Ce bloc corrige le problème pour que les couleurs **rouge, vert et bleu** s’affichent correctement.

---

## Comment l’utiliser

1. Glissez le bloc **BLiXel corriger les couleurs** dans votre programme.  
2. Placez-le dans `au démarrage` pour que la correction soit appliquée dès le lancement.  
3. Ensuite, toutes les couleurs BLiXel seront affichées correctement.

---

## Exemple

```blocks
input.onButtonPressed(Button.A, function () {
    BLiXel.showColour(0xff0000)
})
BLiXel.blixelColourCorrection()
basic.forever(function () {
	
})
```