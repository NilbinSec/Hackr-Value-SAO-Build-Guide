# Hackr-Value-SAO-Build-Guide

Welcome to the build guide for NilbinSec's first badge, made for DefCon 30! This is a fairly simple, straightforward build, but it may be challenging for those inexperienced with SMD soldering. This guide does offer step by step instructions, but feel free to look up a video or guide for some extra tips!


### Tools needed
* Soldering iron with a small tip
* Solder
* Fine point tweezers
### Optional Tools
* Third hand tool
* Solder sucker (in case of mistakes)
* Hot glue gun and glue sticks (for better light dispersal)
* A multimeter or source of 3.3V and wires (for testing)
### Parts List
* Hackr Value PCB
* 2 SMD Resistors
* 5 SMD LEDs
* 1 SAO connector


## Prep

Wet the sponge, set temp on soldering iron, and plug it in to heat it up. Prop up PCB to prepare for soldering (we’ll be using a third hand). Lay out the 5 LEDs, 2 resistors, and SAO connector from the packaging (don’t lose them, pull ‘em out 1 by 1 if needed).



## Attaching Resistors



Start by soldering the two resistors. Orientation doesn’t matter here, but we did black side up. Place a drop of solder on one pad for the resistor. Make sure you’re heating both the solder and the pad so that the solder will stick. Take the resistor in tweezers, and, using the tweezers, place and hold the resistor. It should be on the drop of solder and correctly placed. With the other hand, take the soldering iron and reheat the solder to hold the resistor in place. Then solder the other side of the resistor in place, again heating both the pad and the resistor.

![SMD - Resistor](https://user-images.githubusercontent.com/85370905/183690429-bb17f8b1-4607-40a3-85a3-315729e5a008.jpg)


Mistakes happen! If too much solder is placed, you can use a solder sucker to suck up the excess solder and recover. You can correct any placement errors using tweezers and the soldering iron. 

![Sucker](https://user-images.githubusercontent.com/85370905/183690503-748f8503-4f88-4e9f-9f8c-cc6ac2ec50c1.jpg)

Repeat this process for the second resistor. 

![Resistors](https://user-images.githubusercontent.com/85370905/183690997-2f93cf28-5155-42dd-be98-5d4ee334e97e.jpg)


## Attaching LEDS

Next we need to solder on the LEDs. We’ll use essentially the same process, placing a drop of solder on the heated pad, then using tweezers to hold the LED in place while the solder is reheated by the iron, then soldering the other side in place.

Current will flow through LEDs in only one direction! Make sure the side with the green line (the cathode) MUST be on the closed end of the box on the silkscreen. Getting one of these wrong could burn out the other LEDs quickly, and getting more than one wrong could prevent the badge from doing anything at all. If you’re worried, you can use a multimeter to check the flow of current for each LED after soldering.

### Note! For best light dispersion turn the LEDs 90 degrees to face inwards towards the center of the badge! This is different from the depiction in the images. 
 ![LED](https://user-images.githubusercontent.com/85370905/183690574-3685cd4f-dbc2-4304-863e-293f27b02181.jpg)


Repeat the process for each of the five LEDs.
### Note! For best light dispersion turn the LEDs 90 degrees to face inwards towards the center of the badge! This is different from the depiction in the images.
## Testing

Before you attach the SAO connector, now is a good time to double check that everything is working as expected. There are several valid ways to do this, including using a multimeter to check that the connections are functioning and applying voltage to the entire badge.

If you do apply voltage at this point, use the VCC and GND holes for the SAO connector. Do not apply voltage to LEDs individually, as this could burn them out without the proper resistance. You can apply voltage with two wires and two AA batteries (or any other pair of batteries that are 1.5V each) to create a circuit that runs 3V through the badge. We found using two AA batteries to be a somewhat cumbersome job, so we used our Flipper Zero to run 3.3V through the badge instead.

![Testing](https://user-images.githubusercontent.com/85370905/183690641-b4d09ab2-24f4-482a-9c1c-2fc7210081f2.jpg)


## Attaching the SAO connector

Now for some classic through-hole soldering! Insert the SAO connector into the side of the PCB with the silkscreen, making sure to match the notch on the connector with the gap in the outline. The pins should stick out of the side that says “Hackr Value”. Prop these up so they can’t move while you’re soldering (a third hand is good for this).

![SAO Connected](https://user-images.githubusercontent.com/85370905/183690714-f6de2115-c2e1-4b26-98d4-f704c1d857f4.jpg)


Solder the pins to the PCB. If you’re having trouble keeping the connector flush with the board, try soldering one pin any way you can, then re-heating the solder momentarily while you push them together. After that first pin is soldered, it will hold the connector in place for the other five pins.

![SAO - Solder](https://user-images.githubusercontent.com/85370905/183690786-18024da4-4547-4920-83fd-3848186b623f.jpg)


## Hot Glue Light Tunnel

Finally, we applied hot glue to the back of the SCB, creating an outline of the wrench that goes along the five LCDs before filling it in. This isn't strictly necessary for board function, but does make it look a little nicer when powered on. 

![Hot Glue Outline](https://user-images.githubusercontent.com/85370905/183690814-b1e81fef-fc36-4484-a2a1-752c00c43488.jpg)


And you've done it! We hope you enjoyed building our first badge and look forward to releasing more in the future!
