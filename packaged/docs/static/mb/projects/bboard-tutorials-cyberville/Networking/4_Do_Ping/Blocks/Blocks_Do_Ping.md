# Do Ping Tutorial for blocks

## Let

Let's do a quick Ping to the Access Point, the M5Core2 Module. It has a default IP address of 192.168.4.1, which is great for getting started!

Tell everyone who you are, your role, as well your MAC and IP address, show them your Cyberville ID Card

![ID](https://github.com/Brilliant-Labs/code.bl/blob/code_alpha/packaged/docs/static/mb/projects/bboard-tutorials-cyberville/Networking/2_MAC_IP/ID.png?raw=true "ID")

## Step 1

Place the ``||basic:show string||`` block in the ``||basic:forever||`` block to repeat it. Change the text to your name.

```blocks
basic.forever(() => {
    basic.showString("MICRO");
});
```

## Step 2

Look at the simulator and make sure it shows your name on the screen.

## Step 3

Place more ``||basic:show string||`` blocks to create your own story.

```blocks
basic.forever(() => {
    basic.showString("MICRO");
    basic.showString("<3<3<3");
})
```

## Step 4

If you have a @boardname@ connected, click ``|Download|`` to transfer your code and watch your name scroll!
