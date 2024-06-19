# MAKE IT ROLL USING A REMOTE vehicule code

![Mkt_Roll_Vehicule_Code-EN](https://github.com/Brilliant-Labs/bboard-tutorials-cards/blob/master/5_Move/Move3/Mkt_Roll_Vehicule_Code-EN.png?raw=true "AMkt_Roll_Vehicule_Code-EN")

![Mkt_Roll_Vehicule_Code-EN](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/bboard-tutorials-cards/5_Move/Move3/Mkt_Roll_Vehicule_Code-EN?raw=true "Mkt_Roll_Vehicule_Code-EN")

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Code Example

Example MAKE IT ROLL USING A REMOTE vehicule code using the b.Board

```blocks

radio.onReceivedNumber(function (receivedNumber) {
if (receivedNumber == 1) {
bBoard_Motor.motorLeftDuty(50)
bBoard_Motor.motorRightDuty(100)
} else if (receivedNumber == 2) {
bBoard_Motor.motorLeftDuty(100)
bBoard_Motor.motorRightDuty(50)
} else if (receivedNumber == 3) {
bBoard_Motor.motorDuty(100)
} else if (receivedNumber == 4) {
bBoard_Motor.motorDuty(-100)
} else {

}
})
radio.setGroup(1)

```