# wizergo
My third hand-wired keyboard design and build: split ergonomic 36-key + two encoder layout with GX16 4-pin aviator connector between halves.

[Build timelapse video!](https://youtu.be/iHv_8P2sFnQ)

[Typing sound test video!](https://youtu.be/g8DxL-B8DD8)

Firmware here: [wizergo qmk firmware and keymap](https://github.com/terryorchard/qmk_firmware/tree/master/keyboards/wizrad/wizergo)

# Parts
* Elite-Pi MCU (RP2040)
* Cherry MX Brown switches
* Amazon "FC Gaming" PBT DSA keycaps
* 1N4148 Diodes
* 16 Gauge copper wire
* 22 gauge enameled copper wire
* 2x12 pin mill-max sockets & pins
* GX16 4-pin aviator connectors
* Brass heat-set threaded inserts
* Metric M2.5 screws 
* Assorted heat shrink
* 7g adhesive weheel weights (3 per side)
* 1.75mm Hatchbox PLA filament
* EC11 encoders
* Hours of my life

# Tools
* Fusion 360
* Ender 3 V2 + Cura
* Pinecil Soldering Iron with B2 and KU tips
* 60-40 Tin Lead Rosin Core Solder Wire
* Hot glue gun
* CA glue
* Straight and 45° tweezers
* Reverse grip tweezers
* Helping Hands
* Leatherman
* Dremel
* Persistence

# Why this?
My first project was a [monoblock split 40-key alice-like layout](https://github.com/terryorchard/keyb/tree/main/torch0) with one encoder, just to get a sense of wiring and programming, and that gave me the confidence to do my own split build. This is what I came up with. My daily driver for the last ~5 years has been a Kinesis Advantage 2 and then 360 Pro, so I took some inspiration from them, Dactyl/Manuform, and 5-column Corne, plus one encoder per-side. The final inspiration was [Manna Harbour's Miryoku layout](https://github.com/manna-harbour/miryoku), I've seen a lot of people on Reddit reference it and I was really intrigued by the idea of homerow mods. All that together locked me in to a (heavily) modified 3x5+3 keymap based on my preferences and existing muscle memory from my Lily58 and Corne layouts.

My second project was [a few numpads](https://github.com/terryorchard/keyb/tree/main/torchnum) with only "hard" wiring, all copper, no soft wires, and I loved the process, results, and aesthetic so I went for that again with this build. I also love the dual encoders on my Corne and Lily58, but I did find giving up the third thumb button on my Corne only really worked with modifiers on the 6th column, so I wanted 5 columns, 3 thumb keys, and one encoder per-half. Because it has tenting and some column scoop I had plenty of vertical room on the back to work with, so I wired in a low-profile choc switch as a reset button, because why not, and used the rest of the room for a ridiculous alternative to TRS / TRRS with a 4-pin GX16 aviator connector to link the halves.

Because it has a kind of chunkier, more industrial aesthetic rather than smooth curves I think the aviator connector was a great choice, and I honestly just carry it around by the cable since it's so solidly connected to the case. The "downside" is that I have to make custom F-F cables, but the upside is that I get to make custom cables.

# How'd it go?
I have some experience with Fusion 360 but am very much so an amateur hobbyist so this really stretched my abilities, the CAD was definitely one of the most challenging projects I have ever done. I ended up building a single key switch holder, made 3 copies of that for a column and tilted the top and bottom towards the center and merged them together for a single column, then cloned that 9 times to make the full keyboard. Then it was just a matter of staggering columns horizontally and vertically to make the alpha key's switch plate, merge the 2 groups of 5 columns, then tenting the two halves.

After that it was just a super time consuming process of creating a footprint outline, extruding walls, then a ton of tedious splitting and rejoining solids so it would line up with the column angles, with a tilted platform for the thumb keys, and leaving room for the controller. The cutouts for the reset switch, aviator connector, and sections for weights were straightforward subtractions that I test printed to check tolerances. After 3(?) rough prototype prints I went all in and did the final prints with 100% infill and 0.12mm layer height, which took ~36 hours per-half. While I was waiting for that I also designed some printable encoder knobs, and ran through some prototypes to get something that both fit well and felt good, I'm very happy with the "knurled" mid sized knobs I landed on (STLs for D-post EC11 encoders are freely available in 3D files folder).

The wiring was not overly difficult after the last two projects, just a slow and steady, zen process of straighten, bend, check fit, bend, fit, solder. And once again I used sendcutsend to get some custom cut 3mm clear acrylic bottom plates with cutouts for my wizrad cat logo to protect the wiring, show off the wiring, and add a little extra weight to the bottom. The bulk of the weight is in the print, the switches, and the car wheel balancing weights I stuck in, but the plates do help it feel a bit more substantial and "finished".

In the spirit of honesty, writing the firmware was a real pain in the ass. I'm glad my first project was just one controller rather than split. I learned a lot from that, but had to lean heavily on the SplitKB Aurora QMK firmware files, Discord, Reddit, and Google to hack together stable firmware this time. I won't go into detail, it was just rough and took a lot of hours, but I did it and have happily been using the board as my main daily driver for the last month or so.

Praise be 5-column layouts and homerow mods.

# What next?
Now that I've done monoblock, split, and numpads all with MX keys, the next level is choc low-profile switches, hotswap sockets, and bluetooth. Stay tuned...

# Where the magic happens
![Alt text](images/workbench.jpg?raw=true "Workbench")

# Gallery

**Fusion 360 screenshot of the CAD.**
![CAD 1](images/CAD1.png?raw=true)

**Finished build.**
![Alt text](images/wizergo(5).jpg?raw=true)

**Backside aviator connectors and reset switches.**
![Alt text](images/wizergo(7).jpg?raw=true)

**Closeup of the copper wiring.**
![Alt text](images/wizergo(4).jpg?raw=true)

**Symmetrically wired halves and acrylic bottom plates.**
![Alt text](images/wizergo(8).jpg?raw=true)

**Ergo tent and scoop plus rad wizard cat engraving.**
![Alt text](images/wizergo(1).jpg?raw=true)

**Fusion 360 renders just for fun.**
![CAD 1](images/CAD2.png?raw=true)
![CAD 1](images/CAD3.png?raw=true)
