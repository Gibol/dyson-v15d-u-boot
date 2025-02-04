
## The story
It begins on an aucion site where I became the owner of broken Dyson Submarine wet roller head.
It came full of water in the electronic's compartment, because a plastic tube feeding the water broke.
Fortunatelly this time hot glue on the PCB happend to be usefull and protected the circuit from water damage (mostly), so I was able to fix it

Dyson Submarine mop accessory is not working on old Dyson vacuums, it works only with the new v15s which, according to the Dyson website is exactly the same as v15 but with different software :clownface:

Not being able to update the software is a nice excuse untill there is a connected version of dyson vacuum (perhaps v16 or gen6) and a subscription based service - then vacuums will receive weekly updates at a low price of $19 per month.

I'm not sure if there is any communication between the vacuum and the submarine accessory because I own a very old (v15) dyson model and quite frankly I coudn't be bother to check after I discovered that connecting power to submarine head is enough to make it do it's job.

So, if the only requirement is to power the roller head and there is no way to make it work with actual functioning Dyson vaccum, the only logical way was to make new (non sucking) dumb dyson vacuum model

# (not)Dyson V15d U-Boot
<img src="whole.jpg" alt="U-Boot" height="600" />

## Parts
Basically you will only need two parts:
- Broken dyson vacuum body or spare parts. In my case I've used DC62 (V6) body (with battery) and part of v7 dustbin which connects to the wand (wand itself is also necessary!). V6 wand connector is different, will not work, you need V7 or newer.
- Step-up DC-DC converter with decent caps on input and output able to handle input voltage of your dyson battery and over 3A of current (mine is rated for 5 or 6 Amps and has 470uF caps built in, see photos)

<img src="parts.jpg" alt="U-Boot" height="600" /> <img src="dry_fit.jpg" alt="U-Boot" height="600" />

## Setting up the DC-DC converter
Dyson sumbarine head is rated for 16.2V 45W.
Set the DC-DC converter voltage to 16.5-16.8V to compensate for voltage drops.
If your DC-DC converter has current limiting capabilities set it to maximum, we don't need to limit the current.

## Battery
If your battery is dead or if you want to prevent the invitable death of you dyson battery, I recommend flashing alternative firmware to it: https://github.com/tinfever/FU-Dyson-BMS
This is not necessary if your battery is operational.

## Connecting junk together
I've used heatgun to shape the wand attachement to fit inside the v6 body (removing some insides of the body was necessary),  I've drowned it in hot glue to the point that it's not going anywhere and became almost a solid block.
But you do you, release your creativity and try to use whatever is available or suitable for you.
In terms of electrical connections - connect the trigger wires to the input terminal of the DC-DC converter and wand connector to the output (WHITE is -, BLACK is +)
Additionally for visual effects I've added two white LEDs connected in series with 1K resistor to illuminate the MAX button at the back of the V6 body and I also drowned it with hot glue just to be safe!

<img src="dcdc.jpg" alt="U-Boot" height="600" /> <img src="guts.jpg" alt="U-Boot" height="600" />




It works and it even looks okay!

<img src="assembled.jpg" alt="U-Boot" height="600" /> <img src="side.jpg" alt="U-Boot" height="600" />

Video (Youtube):

[![VIDEO](http://img.youtube.com/vi/fbeCS-oXFKM/0.jpg)](http://www.youtube.com/watch?v=fbeCS-oXFKM "Video")


