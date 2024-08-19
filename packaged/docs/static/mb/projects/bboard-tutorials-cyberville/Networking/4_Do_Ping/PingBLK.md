# Pinging Tutorial for Blocks

*Let´s start*

Let's do a quick __ping__ to the Access Point 📳, the M5Core2 Module. It has a default IP address 📮 of 192.168.4.1, which is great for getting started!

Tell everyone who you are, your role, as well your MAC and IP address, show them your Cyberville ID Card. 

Blocks

![Role](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/3_Role/Rol.png?raw=true "ID")


## Step 1

Place a ``||input:on button pressed||`` block to run code when button **A** is pressed.

```blocks
input.onButtonPressed(Button.A, () => { 
});
```

## Step 2

Place a ``||basic:show leds||`` block inside ``||input:on button pressed||`` to display a smiley on the screen. Press the **A** button in the simulator to see the smiley.

```blocks
Cybersec.wifi_connect("Cyberville #1", "")

input.on_button_pressed(Button.A, on_button_pressed_a)

input.onButtonPressed(Button.A, () => { 
    basic.showLeds(`
        # # . # #
        # # . # #
        . . . . .
        # . . . #
        . # # # .`
        );
});
```

## Step 3

Add ``||input:on button pressed||`` and ``||basic:show leds||`` blocks to display a frowny when button **B** is pressed.

```blocks
input.onButtonPressed(Button.B, () => { 
    basic.showLeds(`
        # # . # #
        # # . # #
        . . . . .
        . # # # .
        # . . . #`
        );
});
```

## Step 4

Add a secret mode that happens when **A** and **B** are pressed together. For this case, add multiple ``||basic:show leds||`` blocks to create an animation.

```blocks
input.onButtonPressed(Button.AB, () => {
    basic.showLeds(`
        . . . . .
        # . # . .
        . . . . .
        # . . . #
        . # # # .
        `)
    basic.showLeds(`
        . . . . .
        . . # . #
        . . . . .
        # . . . #
        . # # # .
        `)    
})
```

## Step 5

If you have a @boardname@, connect it to USB and click ``|Download|`` to transfer your code. Press button **A** on your @boardname@. Try button **B** and then **A** and **B** together.

## Step 6

Nice! Now go and show it off to your friends!

