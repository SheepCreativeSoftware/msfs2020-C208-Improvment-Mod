# Cessna 208B Improvement Mod for Microsoft Flight Simulator

A community mod for the Cessna 208B Grand Caravan, which aims to fix many of the issues present in the stock version.

***Engine and Flight Model***  
Higher thrust and greater braking force, allowing for short field ops.  
Improved flight characteristics, more realistic climb, increased drag on approach and less float on landing.  
More accurate cruise performance.

***Ground Handling***    
More control while taxiing.  
Tighter turning circle.  
More realistic idle behaviour, lower fuel burn.

***Systems & Avionics***  
Added CAS annunciations, Systems Page, improved engine readouts.   
Autopilot and instrument fixes.  
More accurate start up.

***Miscellaneous***  
Improved lighting and textures.

Based on the work of [C208-MSFS2020-Fix](https://github.com/Exp232/C208-MSFS2020-Fix) and [msfs2020-C208-Improvment-Mod](https://github.com/SheepCreativeSoftware/msfs2020-C208-Improvment-Mod)

Thanks to everyone who has contributed, and to PilotTrev for sharing his knowledge and first hand experience.

----

## Issues and Limitations

- Beta mode ~~and prop feathering are~~ nonfunctional **(Prop feathering fixed)**
- ~~The propeller generates zero drag/has no affect on torque~~ **(I think I fixed this by boosting prop MOI by some amount, MS's values seemed absurdly low)**
- Torque increases with altitude
- ITT effectively decreases with altitude

***Propeller*** - Beta mode is completely nonfunctional, blade pitch jumps from the minimum stop to reverse with no control between.  ~~Feathering is possible, but the behaviour is so bugged that it's practically useless. The prop itself lacks any physics, produces no drag and has no affect on torque.~~

***Climb Performance*** - With ITT being broken, it's not possible to use it as a metric when tuning climb performance, neither is the *Maximum Torque for Climb* chart of much use. Instead, I referenced the *Maximum RoC* and *RoC - Takeoff Flap Setting* tables, crosschecked with *Time, Fuel, and Distance*, to find a somewhat acceptable balance where climb performance is not overly excessive at minimum weight, but still allows for max RoC at max weight. I haven't accounted for the reduction in airspeed when flying through clouds.

***Cruise Performance*** - Due to the torque/prop issues, cruise performance and fuel flow can only be tuned correctly for a specific set of conditions, outside of which, engine behaviour and performance varies. For this purpose I used ISA conditions, 8807 pounds and 1750 RPM.

***Flight Model (WIP)*** - The flight model is the result of adapting the POH to the above issues and the limited control the config files provide. Not only are turboprops poorly simulated but the inaccuracies are all over the place, meaning the phases of flight are often at odds with each other. With this in mind, I've attempted to average out behaviour at all stages of operation, rather than perfecting any one aspect at the expense of another.

As mentioned above, the flight model has been tuned using ISA conditions, a climb/cruise/landing weight of 7300-8807/8807/8500 pounds, a cruise RPM of 1750 and the inertial separator normal; live weather behaviour will vary but should still show an improvement over the previous model.

A few notes from my testing so far:

- *Taxi* -  To compensate for the lack of beta, thrust in the beta range has been further reduced to make taxiing more manageable.
- *Takeoff* - For the most part, normal and short field takeoff procedures can be followed as you'd expect - maximum takeoff torque, takeoff distance and RoC with flaps TO/APR closely match the POH. Flaps UP takeoff ground roll is shorter than it should be.
- *Climb* - The thrust to drag ratio favours the accuracy of cruise over climb performance. As a consequence, at lower weight, climb performance is higher than it should be, and requires a reduced power setting. At maximum weight, required power/torque will be higher than expected. Time, fuel and distance are correct as long as VS/KIAS are kept in check.
- *Cruise* - Cruise performance is fairly accurate to 12,000 ft (1750 RPM), above which, torque and fuel flow remain accurate to 18,000 ft, while airspeed falls below expected numbers; to compensate, prop RPM can be increased without affecting torque. Above 18,000 ft, power must be increased and consequently fuel flow will be higher than expected.
- *Descent, approach and landing* - Drag has been increased and the relationship between Ng and the power lever adjusted in an attempt to simulate propeller drag as you bring it back towards idle.

----

## Compatibility

***Sim version*** - v1.13.16.0

***WT G1000 version*** - v0.3.7, v0.4 beta

## Required

***[Working Title's G1000 v0.3.7](https://github.com/Working-Title-MSFS-Mods/fspackages/releases/tag/g1000-v0.3.7)***


----

## Download

***[Latest Release v2106.1](https://github.com/SheepCreativeSoftware/msfs2020-C208-Improvment-Mod/releases/tag/v2106.1.beta.1)***

## How to install

1. Delete any previous versions.
2. Copy the C208B-mod folder into the Community Folder.

***WT G1000 v0.3.7*** - To enable annunciations you will need to replace the following file with the one included with this mod (wt-g1000-0.3.4-fix):
*workingtitle-g1000\html_ui\WorkingTitle\Pages\VCockpit\Instruments\NavSystems\SharedCommonPFD_MFD.js*
