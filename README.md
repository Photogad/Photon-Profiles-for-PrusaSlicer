# Photon-Profiles-for-PrusaSlicer
Finely tuned Photon™ profiles for PrusaSlicer. Highly optimized for MK3S Bondtech BMG Extruder with Mosquito hot end, but should work fine on a stock MK3S printer.
NOTE: These profiles are in Beta stage and a work in progress. Some profiles may be missing features listed below.

# Features
 - Profiles tuned for a wide-range of nozzle sizes (0.15mm, 0.20mm, 0.25mm, 0.40mm, 0.50mm, 0.60mm, 0.80mm, 1mm)
 - Profiles tuned for different materials (PLA, PETG, PC, FLEX, etc)
 - Profiles tuned for a wide variety of filament brands with extensive testing for best temperature and extrusion multiplier. 
 - Multiple profiles based on your printing goals (Quality, Speed, More Speed, Strength, etc).

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
