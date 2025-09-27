# Capteur GSR

Le GSR peut être utilisé pour mesurer l'activité électrodermale (EDA) du corps humain, également connue sous le nom de réponse galvanique de la peau (GSR).
L'EDA est une mesure courante de l'activité du système nerveux autonome. La conductance cutanée n'est pas contrôlée consciemment, elle est contrôlée de manière autonome par l'activité sympathique et les états cognitifs et émotionnels à un niveau subconscient. Par conséquent, la résistance électrique de la peau offre un aperçu direct de la régulation émotionnelle autonome.

## Exemple de code

```blocks
let gsr = GSR_Sensor.createGSRReader(BoardID.zero, ClickID.A)
basic.showIcon(IconNames.Heart)
basic.forever(function () {
    serial.writeValue(« GSR », gsr.getGSR())
})
```