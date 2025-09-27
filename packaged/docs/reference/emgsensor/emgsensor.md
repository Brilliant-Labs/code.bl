# EMG_Sensor

Electromyography, or EMG, is a diagnostic technique for measuring the electrical activity of muscles. It is often used to diagnose the health of these muscles and the neurons that control them. These neurons are called motor neurons. They transmit electrical signals, and the muscles contract when this happens.

## Code Example

```blocks
let emg = EMG_Sensor.createEMGReader(BoardID.zero, ClickID.A)
basic.showIcon(IconNames.Heart)
basic.forever(function () {
    serial.writeValue("EMG", emg.readEMG())
})
```