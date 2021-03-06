# Photon™ Profiles for PrusaSlicer
Finely tuned Photon™ profiles for PrusaSlicer. Highly optimized for MK3S Bondtech BMG Extruder and Mosquito hot-end (non-magnum) with MMU2S installed, but should work fine on a stock MK3S printer.

NOTE: These profiles are in Beta stage and a work in progress. Some profiles may be missing features listed below.

# Features
 - Profiles tuned for a wide-range of nozzle sizes (0.15mm, 0.20mm, 0.25mm, 0.40mm, 0.50mm, 0.60mm, 0.80mm, 1mm)
 - Profiles tuned for different materials (PLA, PETG, PC, FLEX, etc)
 - Profiles tuned for a wide variety of filament brands with extensive testing for best temperature, extrusion multiplier, and fan speed. 
 - Multiple profiles based on your printing goals (Quality, Speed, More Speed, Strength, etc).
 - Enhanced start GCODE for better purge line than the Prusa purge line. The purge line now does not bump into itself, and prints faster, and is easier to peel off the sheet when using PETG.
 - Only shows the correct matching print profiles based on the printer profile that is activated.

# Profile Naming System

**SEXY**

*For the best looking prints. 
Looks as good as the stock Prusa quality settings, but prints even faster!*

**LIGHT SPEED**

*For much faster prints, with a small loss of detail on the X and Y axis. Do not use this if your print has a lot of small or fine features on the top or bottom, such as small embossed or raised lettering. Good for mechanical prints where quality does not matter.*

How it works: 
I've increased the line widths by a large amount, but to a percentage that the nozzle can handle. I've also lowered the infill amount a little bit, and increased the printing speeds.

**LUDICROUS SPEED**

*For even faster prints, with the same loss of detail above, but also a taller layer height which means a loss of detail on the Z axis. Do not use this if your print has a lot of small or fine features anywhere on the print, such as small embossed or raised lettering. Even better for mechanical prints where quality does not matter.*

How it works: 
Like the LIGHT SPEED profile, I've increased the line widths by a large amount, but to a percentage that the nozzle can handle. I've also lowered the infill even more and increased the printing speeds. Lastly, I've increased the layer height to the maximum amount that the nozzle can safely handle.

**STRONG**

*For mechanical prints where quality does not matter, but strength and print speed does.*

How it works: 
I've taken the LIGHT SPEED profile and increased the infill amount, as well as the number of perimeters, and top and bottom shell thickness. I also recommend for strong parts to temporarily alter your filament profile to increase nozzle temperature by 10c, which helps to increase layer adhesion and therefore print strength. Unfortunately I cannot set up PrusaSlicer to do this automatically via preset profiles.

**There are also other small tweaks here and there to increase speed on the faster profiles, but I will not bother to list them all.**

# Example print times

For a 3D Benchy @ 300% scale with a 0.40mm nozzle using PLA:

- Prusa Quality Profile: 15 hours, 24 minutes.
- Prusa Speed Profile: 12 hours, 27 minutes.
- Photon SEXY Profile: 14 hours, 7 minutes.
- Photon LIGHTSPEED profile: 9 hours, 3 minutes.
- Photon LUDICROUS SPEED profile: 6 hours, 19 minutes.
- Photon STRONG profile: 12 hours, 40 minutes.

You can see the SEXY profile prints faster than the Prusa quality profile by about 7%.

The LIGHTSPEED profile prints faster than the Prusa speed profile by about 25%.

The LUDICROUS SPEED profile prints faster than the Prusa speed profile by about 50%.


TODO: Add photos.

# Will this work on a stock MK3S printer that doesn't have a Bondtech Extruder and Mosquito hot end, or a printer with no MMU2S installed?

The print profiles should work fine, but you may need to alter the printer profiles and filament profiles and save them. Here's what you should change:
- Retraction in the printer profiles. My retraction settings should still work fine on a stock MK3S, however you may get slightly better results if you run a [Retraction Calibration](retractioncalibration.com) test print and determine your own values.
- Max Volumetric Flow in the filament profiles. I've determined the maximum volumetric flow with the BMG/Mosquito setup is about 17.6 mm3/s with PLA and 17.2 mm3/s with PETG, but I set it in the Photon profiles to be 17 for safety. On a stock MK3S (E3D) hot end, you want to set this to 15 for PLA and 8 for PETG. The max volumetric flow rate "caps" your print speeds to not print faster than your hot-end can push plastic out. If you do not change this setting for a stock MK3S, you may have underextrusion issues sometimes on certain prints.
- Fan speed in the filament profiles. I have these optimized for the [LDO BLOWER FAN](https://www.printedsolid.com/collections/prusa/products/ldo-5015-5v-blower-fan-df5015h05s) which is more powerful than the stock fan (I highly recommend getting one for best bridging and overhangs!). You can [RUN YOUR OWN FAN SPEED TEST](https://www.prusaprinters.org/prints/58001-ultimate-fan-speed-test) to determine the best values if you are using the stock fan, or simply set all the fan speeds to 100% for PLA like the Prusa defaults.

- Profile names. They are named "BMG-M" denoting BMG extruder and Mosquito hot end. You may want to change the names and re-save each profile if this bothers you. To do it quickly, you can use a program in windows to find+replace "BMG-M" in the folder and change it to "MK3S" or whatever you want to call it.

# Includes Prusa MK3S 3D Model and Ultistik™ Textured Sheet Preview
If you don't want these, simply delete the "bed images" folder.

[Bed Model](https://github.com/Photogad/Photon-Profiles-for-PrusaSlicer/blob/main/docs/Bed.png)


