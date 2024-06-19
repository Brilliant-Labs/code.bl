# Measure:  MAKE IT MEASURE MAGNETIC FIELD

![Mkt_Measure_Magnetic_Field-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/8_Measure/Measure3/Mkt_Measure_Magnetic_Field-EN.png?raw=true "Mkt_Measure_Magnetic_Field-EN")

![Mkt_Measure_Magnetic_Field-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/8_Measure/Measure3/Mkt_Measure_Magnetic_Field-EN.png?raw=true "Mkt_Measure_Magnetic_Field-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT MEASURE MAGNETIC FIELD using the b.Board

```blocks

basic.forever(function () {
BLiXel.showBarGraph(input.magneticForce(Dimension.Strength), 1000)
})

```