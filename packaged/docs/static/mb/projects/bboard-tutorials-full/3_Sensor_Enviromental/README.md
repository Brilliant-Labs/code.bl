# 📒 b.Board Tutorial Clickboards:

# `SENSOR`

- [IR Sense 3](#ir-sense-3)
- [Noise](#noise)
- [Temp Log 2](#temp-log-2)
- [Thermo 6](#thermo-6) 
- [Weather](#weather) 
---
## IR Sense 3
![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/IRpic.png?raw=true "A magician's assistant")

## Description

This thermal imaging sensor can
detect environmental heat
changes up to 1m (100cm) away, even
through glass. Also, this sensor
can be used to detect humans as
they approach the area where the
sensor is located.

![IR SENSE 3 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-sense-3/ir-sense-3-click.jpg?raw=true "IR SENSE 3 Click")

## Code Example

This example has the IR SENSE 3 Click plugged into to MikroBus #1 on the b.Board

```blocks
let IR_Sense_32 = IR_Sense_3.createIR_Sense(BoardID.zero, ClickID.A)
basic.forever(function () {
    if (IR_Sense_32.isHumanDetected()) {
        basic.showIcon(IconNames.StickFigure)
    } else {
        basic.showIcon(IconNames.No)
    }
})
```

## Project Idea

THE INVISIBLE TRIP WIRE

Detect someone approaching from one meter
away. Use this click to activate your design
or set an alarm. This is great for projects
that draw a lot of power and can be activated
when being observed and de-activated when
the room is empty. Play a noise when someone
approaches for a good scare!

![Magic](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/ir-distance/magicianGif.gif?raw=true "A magician's assistant")
---
##### [🔙 Back Menu](#sensor) 
---
---
## Noise
![Noise](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/noise/noise.png?raw=true "Noise")

## Description

Enables you to set a noise
detection threshold for alarm
systems, environmental
monitoring or data logging. Need
to monitor the volume of your
voice? No problem. Strap some
neopixels to your project and
have them light up to the noise
level of your voice.

![Noise](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/noise/noise-click.jpg?raw=true "Noise Click")

## Code Example

This example has the Noise Click plugged into to MikroBus #1 on the b.Board.

Just add your Noise Click blocks and code some motors, screens, lights, or other outputs to react to the Noise Click's input!


![Noise](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/noise/noise-code-gif.gif?raw=true "Noise Click")

The noise click will help you measure how much noise (db) is in the area. You can then use the noise level as an input to control actuators, and other outputs. 

Select ||Noise|| category blocks 

```blocks
let strip = neopixel.create(DigitalPin.P1, 30, NeoPixelMode.RGB)
basic.forever(function () {
    strip.showBarGraph(Noise.getNoiseLevel(clickBoardID.one), 1024)
})
```

## Project Idea

SLEEPOVER NOISE MONITOR

Keep noise levels to a minimum, and
you and your sleepover pals out of
trouble, by coding your own noise
level threshold. Keep an eye on noise
levels by adding some neopixels into
the mix. Code your neopixels to alert
you if you are nearing your threshold
by flashing different colours.

![Noise](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/noise/noise-gif.gif?raw=true "Let's Keep things noisy")
---
##### [🔙 Back Menu](#sensor) 
---
## Temp Log 2
![Temp Log 2](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/temp-log-2/hotday.jpg?raw=true "Temp Log 2")

## Description

Ambient temperature sensor with
the ability to store and log data.
This sensor can sense
temperatures from -55°C to
125°C. This sensor would be great
to monitor and plot the
temperature changes over time
in your next project.

![Temp Log 2 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/temp-log-2/temp-log-2-click.jpg?raw=true "Temp Log 2 Click")

## Code Example

This example has the Temp Log 2 Click plugged into to MikroBus #1 on the b.Board. 

We will place the Temp Log 2 Click's value in an "IF / ELSE Statement" which we've nested inside a "Forever Loop". If the temperature is more than 25 degrees Celcius then we will display a message sharing that it is hot!  You could also use this to trigger an IoT action or notification if you have a WiFi_BLE Click or trigger a fan if you have a DC Motor Click.  

```blocks
basic.forever(function () {
    if (Temp_Log_2.readTemperatureC(clickBoardID.one) > 25) {
        basic.showString("It's hot in here! Let's turn on a fan :)")
    } else {
        basic.showString("Nice and Comfy")
    }
})
```

## Project Idea

HOT DOG ALARM

Make sure your pet is
comfortable with the windows
down in your car. Keep tabs on
the temperature with the Temp
Log 2. This click can send an
alert to you when your pet’s
comfort level could be at risk.


![Temp Log 2](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/temp-log-2/hotdaygif.gif?raw=true "Let's Keep things cool")
---
##### [🔙 Back Menu](#sensor) 
---
## Thermo 6
![Thermo 6 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/thermo-6/ice.jpg?raw=true "Thermo 6 click")

## Description

This board shares most of the
functionality with the other
temperature sensors, with one
exception: it is super tiny! This
temperature sensor would be
great should your project require
descretion.

![Thermo 6 Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/thermo-6/thermo-6-click.jpg?raw=true "Thermo 6 Click")

## Code Example

This example has the Thermo 6 Click plugged into to MikroBus #1 on the b.Board. 

We will place the Thermo 6 click value in an "IF /ELSE Statement" which we've nested inside a "Forever Loop".  We compare the value and if it is under 5 degrees Celcius then we trigger the "Brrrr!" message and remind ourselves to grab a jacket before going outside.

```blocks
let Thermo_62 = Thermo_6.createThermo_6(BoardID.zero, ClickID.A)
basic.forever(function () {
    if (Thermo_62.getTemp(Thermo_6.TempUnits.C) < 5) {
        basic.showString("Brrrr!  It's Cold! Grab your jacket!")
    } else {
        basic.showString("Warm and Cozy!")
    }
})

```

## Project Idea

THE AUTOMATIC SNOW JACKET DETECTOR

Never be chilly again with the Automatic
Snow Jacket Detector! Let this sensor stay
outside and pair it with a Wifi Click to
inform you of the temperature while you
stay toasty warm inside. The Wifi click
can be coded to turn on a lamp on your
chest of drawers to indicate that it is
cold, and remind you to grab that
jacket before you leave.


![Cold Gif](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/thermo-6/cold.gif?raw=true "It's Cold!")
---
##### [🔙 Back Menu](#sensor) 
---
## Weather
![Weather Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/weather/ice.jpg?raw=true "Weather click")

## Description

This board shares most of the
functionality with the other
temperature sensors, with one
exception: it detects humidity and pressure!.

![Weather Click](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/weather/weather-click.jpg?raw=true "Weather Click")

## Code Example

This example has the Weather Click plugged into to MikroBus #1 on the b.Board. 

We will place the weather click value in a "Button Pressed event".  Pressing A, B or both, a message with measure of Temperature, Humidity or Pressure will be displayed.

```blocks
let Weather2: Weather.Weather = null
Weather2 = Weather.createWeather(BoardID.zero, ClickID.A)
input.onButtonPressed(Button.A, function () {
    basic.clearScreen()
    basic.showString("" + (Weather2.temperature(Weather.Weather_T.T_C)))
})
input.onButtonPressed(Button.B, function () {
    basic.clearScreen()
    basic.showString("" + (Weather2.humidity()))
})
input.onButtonPressed(Button.AB, function () {
    basic.clearScreen()
    basic.showString("" + (Weather2.pressure(Weather.Weather_P.Pa)))
})

```

## Project Idea

WEATHER STATION

Help to monitor the climate, Let this sensor stay
outside and pair it with a Wifi Click to
inform you of the temperature, pressure and humidity. The Wifi click
can be coded to send this information.


![Cold Gif](https://github.com/Brilliant-Labs/bboard-tutorials-v3/blob/master/weather/cold.gif?raw=true "It's Cold!")
---
##### [🔙 Back Menu](#sensor) 
---