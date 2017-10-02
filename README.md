# OpenC64MegaDrivePadAdapter

OpenC64MegaDrivePadAdapter is an Open Hardware adapter that allows the safe connection of a Sega Mega Drive (known as *Genesis* in the US) controller to a Commodore 64 computer.

![Board](https://github.com/SukkoPera/OpenC64MegaDrivePadAdapter/raw/master/doc/render-top.png)

### Summary
Despite being compatible at the physical level (i.e.: they use the same DB-9 connectors), Sega Mega Drive controllers are slightly different from the *Atari-style joysticks* (which the C64 uses) at the electrical level. These differences usually manifest themselves in the fact that certain keyboard keys are not responsive when a Sega Mega Drive pad is connected to a C64 computer, but the CIA chip may also get harmed as a result.

To make a long story short, Sega Mega Drive controllers keep the button lines at a logical high level when not pressed, while the C64 expects them to be left floating.

Since I think that the Sega Mega Drive controller is one of the best joypads which ever saw the light, I developed this simple adapter board, which is supposed to sit inbetween the C64 and the controller. You should be able to keep it plugged into the computer and then connect the controller to it, but you can also use a joystick extension cord (widely available), if that makes it easier.

### Configuration
The board is based on the circuit that was originally published in [issue #5 of Commodore world](https://www.scribd.com/document/8945979/Commodore-World-Issue-05) back in 1994, with a few improvements that will allow an easier gameplay with certain titles.

You have three configuration jumpers that you can use to customize how the C64 interprets button presses on the controller.

In fact, since most joysticks back in the day only had a single fire button, it was usually used for *firing*, whatever that meant. *Jumping* was usually done with the UP direction of the joystick, which is quite annoying on a joypad.

This is why OpenC64MegaDrivePadAdapter allows you to repurpose the B or C key to jumping, leaving the other button for firing, all at your choice.

It also allows to use C as the second fire button, which is only supported by a few titles. You can even swap B and C, if you prefer.

Configuration is done through the jumpers on the board, and should be pretty self-explanatory. There are only two rules which you will have to remember:
1. **ALWAYS TURN YOUR C64 OFF BEFORE MOVING THE CONFIGURATION JUMPERS.**
2. **NEVER EVER KEEP MORE THAN ONE JUMPER ON THE SAME HORIZONTAL LINE.**

If you don't follow the rules, **you will probably cause permanent damage to your C64 and/or controller**, so **please be careful**, you have been warned.

The default configuration maps B to button 1, C to button 2 and UP to UP. If you play Giana Sisters, you will probably want to use the C button for jumping, so just do the following:
1. Turn OFF your C64.
2. Remove the UP/UP jumper and store it in a safe place.
3. Move the C column jumper to the UP row.
4. Turn on your C64, load the game and enjoy!

### License
OpenC64MegaDrivePadAdapter is Open Hardware.
