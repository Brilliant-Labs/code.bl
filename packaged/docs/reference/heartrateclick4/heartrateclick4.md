# Clickboard HeartRate_Click4

HeartRate_Click4 is a complete pulse oximetry - SpO2- and heart-rate.
This pulse oximeter measures the oxygen saturation in one’s blood, or more precisely, the percentage of hemoglobin molecules in blood that is saturated with oxygen (in a healthy adult, readings go from 94% to 100%).

## Code Example

```blocks
let heart = HeartRate_Click_4.createHeartRateSensor(BoardID.zero, ClickID.A)
basic.showIcon(IconNames.Heart)
basic.forever(function () {
    serial.writeValue("HeartRate", heart.getHeartRate())
    serial.writeValue("Oximeter", heart.getSpO2())
})
```