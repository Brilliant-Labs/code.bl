# Clickboard HeartRate_Click4

HeartRate_Click4 est un oxymètre de pouls complet - SpO2 - et un cardiofréquencemètre.
Cet oxymètre de pouls mesure la saturation en oxygène dans le sang, ou plus précisément, le pourcentage de molécules d'hémoglobine dans le sang qui sont saturées en oxygène (chez un adulte en bonne santé, les valeurs vont de 94 % à 100 %).

## Exemple de code

```blocks
let heart = HeartRate_Click_4.createHeartRateSensor(BoardID.zero, ClickID.A)
basic.showIcon(IconNames.Heart)
basic.forever(function () {
    serial.writeValue("HeartRate", heart.getHeartRate())
    serial.writeValue("Oximeter", heart.getSpO2())
})
```