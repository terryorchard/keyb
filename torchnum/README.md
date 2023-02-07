# torchnum
My second hand-wired "keyboard" design and build: a unique numpad / macropad layout with one encoder and one addressable RGB LED.

Firmware here: [torchnum qmk firmware and keymap](https://github.com/terryorchard/qmk_firmware/tree/master/keyboards/wizrad/torchnum)

# Parts
* Elite-Pi MCU / Sea-Picro EXT V1.0
* Cherry MX Brown switches
* Misc Aliexpress / Amazon keycaps
* 1N4148 Diodes
* 16 Gauge copper wire
* 22 gauge enameled copper wire
* 2x12 pin mill-max sockets & pins
* Assorted heat shrink
* 1.75mm PLA filament
* EC11 encoder
* Hours of my life

# Tools
* Fusion 360
* Ender 3 V2
* Pinecil Soldering Iron with B2 and KU tips
* 60-40 Tin Lead Rosin Core Solder Wire
* CA glue
* Straight and 45° tweezers
* Reverse grip tweezers
* Helping Hands
* Leatherman
* Dremel
* Persistence

# Why this?
Since making the switch to tenkeyless keyboards many years ago, myself and my dad in particular have been missing our numpads for data entry and symbols with alt codes. On top of that we both do af fair bit of repetitive typing that could be moved to macros, so I decided to have a go at making a number + macro pad and ended up making three: a rough one to learn from, one for me, and one for my old man.

I have some extra encoders lying around and find them very useful so I threw those in, and put in a single RGB LED for layer indication. I also had seen some copper-only builds floating around that looked awesome, so I wanted a project I could try to do with no soft wires without being overly ambitious.

# How'd it go?
The layout was pretty simple, just a 4x5 grid with the bottom right key moved up to the encoder push button. I decided not to go with a standard numpad layout, with the large + and 0 keys just so it'd look more unique and have a few extra keys open for programming. The initial CAD was very very simple, but I spent some extra time on the MCU area with hotswap socket slots and a little holder for the encoder.

I printed it top-side down in PLA with standard supports everywhere to allow for the MCU cradle and wizard cat logo, at 50mm/s and 0.12mm layer height for detail and tight tolerances. I also went with 100% infill for a little extra weight and durability, although it was definitely overkill the extra print time and filament was worth it, although I think it would be perfectly functional printed faster with 0.2mm layers and much less infill.

The wiring being all copper was a major goal from the start, and was easily my favorite part of the build. I just straightened the wire with a drill + pliers, roughly figured out how much length I'd need for a run, then bend with pliers, test placement, bend, and repeat until it looked like a good fit. Then it was just a matter of heat shrink for cross overs, tweezers, and patience to get everything soldered in place without any shorts.

I'm really happy with how it came together; using copper wire was a lot more work, but not overly difficult and WAY more aesthetically pleasing IMO. After working with it for a bit it's quite relaxing and satisfying. I used 16AWG for everything except the LED, which got 22AWG since the pads are so small.

The last thing to really finish it up was the 3mm acrylic bottom plate with a new "logo" for my designs from sendcutsend. Very affordable service, and the extra plate lets me see the wiring but keeps it protected from being moved or shorted, and makes the whole thing feel really premium and complete while adding a touch of extra weight.

# What next?
The last thing I need to get figured out is the single RGB LED layer indication. It seems like it "should" be really easy but I just can't get it working after many, many attempts. I'll circle back and update this readme when I finally figure it out. Overall I consider this one a big success and don't plan on doing any revisions or additions besides refining my keymap and other QMK stuff.

# Where the magic happens
![Alt text](images/workbench.jpg?raw=true "Workbench")

# Gallery

**These are all three that I made; the skeleton of the first one I drilled and dremeled, my second glow in the dark build, and the final red one for my dad.**
![Alt text](images/torchnum(7).jpg?raw=true "All together now")

**Close up of the front of the build.**
![Alt text](images/torchnum(1).jpg?raw=true)

**The bottom ft. acrylic plate.**
![Alt text](images/torchnum(2).jpg?raw=true)

**Closeup of the copper wiring.**
![Alt text](images/torchnum(3).jpg?raw=true)

**Very aesthetically different set of builds.**
![Alt text](images/torchnum(4).jpg?raw=true)

**Functionally exactly the same: same pinout, VERY similar wiring, and the same components (with the exception of the MCU).**
![Alt text](images/torchnum(5).jpg?raw=true)

**One more group photo of the three prints.**
![Alt text](images/torchnum(6).jpg?raw=true)
