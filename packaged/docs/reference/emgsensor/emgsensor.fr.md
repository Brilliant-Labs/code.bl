# Capteur EMG

L'électromyographie, ou EMG, est une technique diagnostique permettant de mesurer l'activité électrique des muscles. Elle est souvent utilisée pour diagnostiquer la santé de ces muscles et des neurones qui les contrôlent. Ces neurones sont appelés neurones moteurs. Ils transmettent des signaux électriques, ce qui provoque la contraction des muscles.

## Exemple de code
```blocks
let emg = EMG_Sensor.createEMGReader(BoardID.zero, ClickID.A)
basic.showIcon(IconNames.Heart)
basic.forever(function () {
    serial.writeValue("EMG", emg.readEMG())
})
```