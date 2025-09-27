# GSR Sensor

GSR can be used to measure the electrodermal activity (EDA) of the human body, also known as the galvanic skin response (GSR).
EDA is a common measure of autonomic nervous system activity. Skin conductance is not under conscious control, it is autonomously controlled by the sympathetic activity and cognitive and emotional states on a subconscious level. Therefore, the skin electric resistance offers direct insights into autonomous emotional regulation.

## Code Example

```blocks
let gsr = GSR_Sensor.createGSRReader(BoardID.zero, ClickID.A)
basic.showIcon(IconNames.Heart)
basic.forever(function () {
    serial.writeValue("GSR", gsr.getGSR())
})
```