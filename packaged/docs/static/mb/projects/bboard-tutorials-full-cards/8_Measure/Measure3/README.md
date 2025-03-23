# Measure:  MAKE IT MEASURE MAGNETIC FIELD

![Mkt_Measure_Magnetic_Field-EN](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cards/8_Measure/Measure3/Mkt_Measure_Magnetic_Field-EN.png?raw=true "Mkt_Measure_Magnetic_Field-EN")

## Code Example

Example MAKE IT MEASURE MAGNETIC FIELD using the b.Board

```blocks

basic.forever(function () {
BLiXel.showBarGraph(input.magneticForce(Dimension.Strength), 1000)
})

```