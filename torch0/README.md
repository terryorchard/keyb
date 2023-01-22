# torch0
 First custom hand-wired keyboard

Firmware here: [torch0 qmk firmware and keymap](https://github.com/terryorchard/qmk_firmware/tree/master/keyboards/wizrad/torch0)

# Parts
* Elite-Pi MCU
* Kailh Choc Pink low-profile switches
* MBK Legends keycaps
* 1N4148 Diodes
* 16 Gauge copper wire
* Assorted heat shrink
* Whatever servo wire I had laying around
* A bunch of 1.75 PLA filament
* EC11 encoder cut down for a lower profile
* Hours of my life

# Tools
* TS101 Soldering Iron with B2 and KU tips
* 63-37 Tin Lead Rosin Core Solder Wire
* Straight and 45° Tweezers
* Helping Hands
* Leatherman
* Hot glue gun
* Dremel
* Persistence

# Why this?
The initial inspiration for this build was the Alice layout, but a columnar-staggered, Kailh low-profile, 40% remix with some extra ergonomic tweaks inspired by the 6x3 Corne. A big reason was to avoid doing a split for my first project so I could get my head around wiring and firmware and prove to myself I can actually make a board that works.

I talked my dad into getting a [Keychron Q10](https://www.keychron.com/products/keychron-q10-alice-layout-qmk-custom-mechanical-keyboard) as their first (and second) ergonomic and got to try it out, but I didn't like the row stagger or double B keys so I had a good feeling of what I was going for, so I got out a piece of paper and mapped out where I wanted my rows and columns, especially the outer two columns.

For the hand-wired side of things I took a lot from [Joe Scotto](https://github.com/joe-scotto) builds and videos. Basically, just watching [How to Build a Handwired Keyboard](https://www.youtube.com/watch?v=hjml-K-pV4E) half a dozen times was all I really needed.

# How'd it go?
After putting my sketch into more concrete numbers with [the keyboard layout editor](http://www.keyboard-layout-editor.com/) and getting a baseline layout with [the case and plate builder](http://builder.swillkb.com/) I spent a few hours in Fusion 360 tweaking the spacing for choc switches (with MBK caps) and had to split the switch plate in half with a kinda aesthetic join to fit it on my Ender 3 V2 220mm x 220mm print bed. I did the plates and "case" separately to make soldering easier.

The major pain was soldering columns and especially rows to the socket legs -- it got much easier once I had shorter exposed wires and only one wire per-leg rather than trying to join both row halves at the socket. The copper was actually super easy to work with my Leatherman, and soldering wasn't a problem at 350°F with a chisel tip. I eventually went back and used copper to link the rows of the two halves and just bridged those 4 to the pins rather than running 8 wires and if I built this again I would do that from the very start. It'd be a little more tedious but absolutely worth it.

The only other thing I struggled with was mapping the pins in QMK. Since I'm using an Elite-Pi I have to use the prefix `GPx` for all the pins... but that was not clear in any documentation I could find, but the QMK Discord got me up and running and after making that change I was set to go.

# What next?
The last thing I've added is an encoder that I wired into column 4 row 3 and used two remaining GP0 and GP1 pins for the A and B encoder inputs. To get away with just one encoder I have it programmed to scroll by default, and on number / symbol layers it becomes volume control and I use it a TON. As a bonus I have pressing set to turn on a layer that uses home row mods and disables the outer columns to test out a 3x5_2 layout, which I'm thinking will be my next build.

To really call this "done" I'm planning to add an RGB LED to change colour with the layers and a cut acrylic bottom plate so I can still see the wiring but have it be a bit more sturdy and safe from conductive debris.

# Where the magic happens
![Alt text](images/workbench.jpg?raw=true "Workbench")

# Gallery

This is the 3D CAD of the first version that I printed and built. If I were to rebuild this I would add a hole for the encoder and slots for the sockets so I wouldn't have to drill and dremel them in. Lesson learned.
![Alt text](images/CAD_v0.jpg?raw=true "3D CAD")


The completed build after I first got it all working.
![Alt text](images/FinishedBuild.jpeg?raw=true "Complete Build")


Current state of the board with an added encoder.
![Alt text](images/NewEncoder.jpg?raw=true "Complete Build")


How the encoder is mounted and wired. Flattened out the pins and ran servo wire to the matrix and A | B | ground pins.
![Alt text](images/Wiring03.jpg?raw=true "Complete Build")


How the wiring started, using 16 gauge copper wire for the rows and columns, with diodes for each row connection.
![Alt text](images/Wiring00.jpeg?raw=true "Copper Rows/Columns")

Initial wiring for all 4 rows; three for alphas and one for thumbs and later encoder.
![Alt text](images/Wiring01.jpeg?raw=true "Row Wiring")

Completed wiring with all 12 columns and the rest of the minimal "case". Messy, but functional!
![Alt text](images/Wiring02.jpeg?raw=true "Complete Wiring")