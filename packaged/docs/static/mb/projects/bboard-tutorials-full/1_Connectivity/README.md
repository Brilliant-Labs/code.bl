# 📒 b.Board Tutorial Clickboards:

# `CONNECTIVITY`

- [NFC](#nfc) 
- [WiFi ble](#wifi-ble) 
---
## NFC
![NFC](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/nfc/nfc.jpg?raw=true "NFC")

## Description

This NFC enabled ClickBoardTM
can store simple information
such as text or a website. Use
your bBoard to write directly to
this board and then encourage
users with a NFC reader on their
mobile device to find and scan.

![NFC](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/nfc/nfc-click.jpg?raw=true "NFC Click")

## Code Example

This example has the Touchpad Click plugged into to MikroBus #1 on the b.Board.

Just add your Touchpad blocks and code some motors, screens, lights, or other outputs to react to the Touchpad Click's input!

Locate the NFC block

```blocks
let NFC_Tag = NFC_Tag_2.createNFC_Tag(BoardID.zero, ClickID.A)
basic.forever(function () {
   NFC_Tag.setURI("http://www.brilliantlabs.ca")
})

```

## Project Idea

MAGIC COMMUNICATION

Do you need to embed
information in a subtle way?
Write some text to this
ClickBoardTM and embed the
board itself without a bBoard in
your project. Tell users to scan
and your information will be
revealed.

![Noise](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/nfc/nfc-gif.gif?raw=true "Let's Keep things noisy")
---
##### [🔙 Back Menu](#connectivity) 
---
## WiFi ble
![Wifi BLE](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/wifi-ble/wifilogo.jpg?raw=true "Wifi BLE")

## Description

Want to wirelessly control your
project? This WiFi BLE board will
allow you to connect via either of
these popular wireless
communication protocols. 

With the WIFI BLE Click you can connect to a variety of online services including IFTTT, Adafruit.io, MQTT, and even secure Web Sockets!


![WiFi_BLE](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/wifi-ble/wifi-ble-click.jpg?raw=true "WiFi_BLE Click")

## Code Example

This example has the Touchpad Click plugged into to MikroBus #1 on the b.Board.

Just add your Touchpad blocks and code some motors, screens, lights, or other outputs to react to the Touchpad Click's input!

Locate the WiFi_BLE blocks

![WiFi_BLE](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/wifi-ble/wifi-ble-code-gif.gif?raw=true "WiFi_BLE Click")

The WiFi BLE is the perfect click to connect your latest inventions to the internet or send data to a cloud service!


Select || WiFi BLE || category blocks 

```blocks
input.onButtonPressed(Button.A, function () {
    WiFi_BLE.publishAdafruitMQTT("StayBrilliant/feeds/test", input.temperature(), clickBoardID.one)
})
WiFi_BLE.WifiConnect("Enter SSID Here", "Enter PW Here", clickBoardID.one)
basic.pause(100)
basic.showIcon(IconNames.Yes)
```

## Project Idea

CREATE YOUR OWN IoT

In a world with hundreds of
thousands of IoT devices, how
will your smart device be
different? Will it light-up? Will
it make sound? Will it control a
motor from around the world?
The choice is yours!


![Wifi-ble](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/wifi-ble/wifi-click-gif.gif?raw=true "Let's Keep things Connected")
---
##### [🔙 Back Menu](#connectivity) 
---
