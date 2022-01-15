## Changes

**2201.0.2**
- fix: reverse thrust is too small and has no effect on the plane
- fix: add dummy interaction point for ground power unit.
- fix: prevent reference cruise torque bug disappear if RPMS are slightly above 1900
- fix: make a few iop controls movable: pressurization lever, heating and ventilation pulling knobs (They still do not impact the model though).
- fix: Changed the default look of Stby Alternator LED to make it more distinguashable between on and off states

**2201.0.1**
- Metal chip detection after prolonged engine overstress (You can disable/enable engine failures in the MSFS Assistance Options)
- sound warning about aircraft overstress
- New dynamic maximum torque calculation

**2201.0.0**
- Changed the electric bus configuration to comply with POH. 
- Cabin light connected directly to battery bus. 
- Battery switch disconnects battery bus instead of the battery itself
- Changes in the sound configuration
- fixes for default FLT configurations
- fix for a problem with External Power switch. it did not reconnect starter to battery when external power was disconnected
- Generator switch has been fixed. Right now it is possible to trip the main generator.
- Generator characteristics have been modified: Workaround for now to simulate lack of power during the startup.
- Fixed the panel emblem light knob
- increase the brightness of the stby alternator light.
- Fixed configuration of PFD and MFD - they properly initialize right now. Avionics 1 switch enables only PFD 1.
- Improved CAS Annunciations
- fix the battery load indication

**2112.1.5**
- Fixed wrong behaivor of the passenger cabin lights

**2112.1.4**
- Added Content Info

**2112.1.3**
- Power supply truck can be requested for external power supply

**2112.1.2**
- Activate Startup Screen for MFD

**2112.1.1**
- Removed yellow color range on the airspeed indicator
- Added License info

**2112.1**
- Tested version

**2112.0.3**
- Prop is now in Feather when starting in cold & dark

**2111.0.2**
- Fixed Center of Gravity, Forward and Aft Limit to be more accurate

**2111.0.1**
- Changed position of Condition lever depending on startup scenario (Fuel Valve will be closed when starting in cold & dark)
- Changed position of Alternator switch depending on startup scenario

**2112.0**
- New EIS dynamic function now also working with NXi
- Corrected BATT, GEN and ALT AMPS

**2111.1**
- Added some INOP switches

**2111.0**
- Update for SU7

**2110.0**
- Tested Release Version

**2110.0.beta1**
- New EIS function will work with stock G1000 (NXi not ready yet)
- Improved EIS for WorkingTitle NXi (Engine Page, System Page)

**2110.0.alpha2**
- EIS Update for WorkingTitle NXi

**2110.0.alpha1**
- Update for SU6

**2109.2**
- Fixed texture of standby torque gauge

**2109.1**
- Added and changed some Annunciation Messages
- More steering angle on higher speed
- Fixed: Oil temperature is always in the yellow position
- POIs do not popping in at far distances
- Some small improvments on flight characteristics
- Fixed: Standby torque does show the wrong value
- Fixed Standby Airspeed Indicator texture


**2108.4**
- Fixed compatibility issue on the Avionics with other Turboprops
- Separate Mod for users who want to play with the vanilla G1000 or WorkingTitle legacy G1000

**2108.3**
- Fixed Annunciation Messages
- Deleted WorkingTitle Fix (No longer needed)

**v2108.2**
- Updated WorkingTitle G1000 v0.4 / GX v0.1.0-dev10 Fix

**v2108.1**
- Updated Files for SU5

**v2107.1**
- Increased propeller moi
- added more texture fixes
- Added additional Voice Alert for Minimums
- Added additional Voice Alert when within 1000 feet of the target altitude set in the autopilot
- Corrected BATT, GEN and ALT AMPS on Engine/System Pages

**v2106.2**
- Going back to most of the Vanila Data cause performance is good since SU4
- Test

**v2106.1.beta.1**
- Clean and Compare Mod with original source
- Update WorkingTitle Fix
- Update WorkingTitle Engine Pages
- First Beta Version

**v2102.3**

- Drag scalars adjusted

**v2102.2**

Compatibility patch for MSFS update 1.13.16.0

- Flap lift/drag scalars adjusted

**v2102.1b**

Flight model/engine update addressing the following:

- Short field takeoff/landing distance
- Rate of climb flaps TO/APR
- Max rate of climb flaps UP
- Airspeed (takeoff, enroute climb, descent, landing approach)
- Cruise performance (fuel flow, airspeed)
- Ng idle behaviour (fuel flow, RPM)

**v2102.1**

- Oil temp adjusted (BubblyDruid56)
- ITT increased (still broken)
- Fuel controller adjusted
- Prop governor adjusted (less overrun)
- Spawn states revised (apron, runway, cruise) 
- Cockpit textures revised

**v2012.2**

- Max torque limit adjusted (max 2500 FT-LB) (TrentKama)
- Brake scalar increased (TrentKama)
- Stall warning type changed (TrentKama)
- Anti-ice Max Flow switch fixed (reversed)
- G1000 splash screen revised (PilotTrev)
- Prop/spinner textures revised

**v2012.1**

- Avionics and light improvements from https://github.com/SheepCreativeSoftware/msfs2020-C208-Improvment-Mod
- Cockpit, autopilot, engine and flight model fixes from https://github.com/Exp232/C208-MSFS2020-Fix

With the following changes:

- Mod files brought in line with the current stock C208B
- Propeller specs changed to match McCauley 4HFR34C778 (TrentKama)
- Max prop RPM reduced (max 1900)
- Reverse thrust range reduced
- Nosewheel steering angle increased (51.5 degrees)
- Yaw damper enabled
- Reversionary mode enabled
- Center and Left Flood dimming knobs swapped
- Stby torque gauge replaced
- Stby avionics power fixed
- Decal/Text textures revised
