# 4_Pinging

Now that the __Cyberville__ network is up and running and everyone's roles are filled, it's time to find out if there's someone special in the network. To do that, we're going to use the command "__ping__."

A __"ping"__ is a simple Internet program that lets you test and verify if a particular destination __IP__ address exists and can accept requests in the __Cyberville__ network. It's really easy to use! Another great thing about __ping__ is that it lets you know if another board is trying to reach you and that it's working properly.
Let's use the __"ping"__ command to find out if other roles are in the __Cyberville__ network! 

## Activity
Let's quickly check if the Access Point 📳 M5Core2 Module is available doing __Ping__. It has a handy default IP address 📮 of 192.168.4.1, which is perfect for getting started! 
It would be fun to share our ID cards and find out who our classmates are connected to. 


## Code Example

You can download the code for this activity from `https://www.brilliantlabs.ca/documents/cybersec/Networking_D.hex` the file will be in Recent Download History, just drag and drop it into a new project.  

Or use this code example to __pinging__ your friends.

__*Please do not forget to set up the correct name for the access point. Mute the PC sound to listen the b.Board sound.*__

```blocks
input.onButtonPressed(Button.A, function () {
    Cybersec.PingbBfrend("192.168.4.1")
})
Cybersec.WifiConnect("Cyberville #?", "")
```