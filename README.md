# Cessna 208B Improvement Mod for Microsoft Flight Simulator

A community mod for the Cessna 208B Grand Caravan, which aims to fix many of the issues present in the stock version.
Feel free to contribute to this mod! Create an issue or fork and create a pull request!  
Disscution about this mod, takes place in the [official forum](https://forums.flightsimulator.com/t/c208b-grand-caravan-ex-mods-general/322172?u=magrainaone)

**Based on Sim version 1.21.18.0 (SU7)**

***Engine and Flight Model***
- Corrected Different Values according to POH
- Reverse thrust is stregthened and has noticible effect on the plane
- 4 minutes of engine overstress (operating above max torque limit) cause CAS message about metal chips in the oil and increase probability of the engine failure.
The average time of engine failure after metal chips appearance is 100 minutes. The event is random so you may not experience engine failure if you are gentle with throttle.
If the engine is kept overstressed the probability of the engine failure increases. Each second of keeping the engine above the torque limit decreases the expected enigne failure time by 8 second.  
You can disable/enable engine failures in the MSFS Assistance Options.

***Ground Handling***
- More control while taxiing
- Tighter turning circle

***Electric System***
- Electric system of Cessna has been modified to reflect the real aircraft configuration. The battery is connected to an always-hot battery bus. The Master Battery Switch disconnects the battery bus from the main power distribution bus of the aircraft.
- Interior cabin lights are connected directly to the battery bus and are powered independently of the master battery switch position. Pilot is able to switch on the cabin lights and there should be enough ambient light in the cockpit to operate without a torch.
- Cessna is equipped with combined started-generator unit. The unit works in starter mode if the engine is below 46% Ng, and in generator mode for Ng above 46%. The generator is connected to the power distribution bus of the aircraft through a contactor. The gen switch allows disconnecting the generator's contactor if required by emergency procedure or to check the operation of standby alternator during the runup.
- Startup switch allows initiation of the engine startup procedure. Start switch operates only if engine is below 46% Ng, if engine operates above 46% starter switch does not interact with any aircraft systems. Putting it to start position powers engine igniters, disconnects the generator contractor and powers the engine starter. Starter is disabled automatically when the engine reaches 46% Ng. After reaching stable engine opreation pilot can put the starter switch to off position. It disables ignition system and connects the generator contractor.
- Starter is one of the most power demanding component on the aricraft. The battery provides the power to start the engine in most real scenarios. The current drawn by the starter depend on the external teamperature. For temperatures below -20C the starter takes 3500W while above 20C the consuption drops to 2500W. The minimum voltage required to run starter is 24V.
- The Mod improves the battery, generator and stby alternator current indications on PFD/MFD. The negative value of the battery current indicates that battery is discharging. Positive battery current means the battery is charging. The charging current is dependent on the battery current capacity. The inicated charging current decreases to zero with the battery reaching full capacity. However, for simplicity the charging time is not adeqate and is usually much shorter.
- All knobs used to regulate the light intensity also impact the light current consumption. The dimmer the light the less current is drawn from battery or generators.

***Systems & Avionics***
- Works with Stock G1000 and WT G1000 NXi Avionics
- Added CAS annunciations, Systems Page, improved engine readouts, fuel indication
- Cruize torque bug does not longer disappear for RPMS slightly above 1900 
- Reversionary Mode Enabled
- Additional Voice Alerts
- Autopilot and instrument fixes
- Yaw Damper Working
- More accurate start up

***Miscellaneous***
- Improved lighting and textures
- All panel potentiometers work
- Added some inoperative Switches
- Fixed Cabin lights

Based on the work of [C208-MSFS2020-Fix](https://github.com/Exp232/C208-MSFS2020-Fix), [msfs2020-C208-Improvment-Mod](https://github.com/SheepCreativeSoftware/msfs2020-C208-Improvment-Mod) and [dgtlanlg/C208B-mod](https://github.com/dgtlanlg/C208B-mod)

Thanks to everyone who has contributed, and to PilotTrev for sharing his knowledge and first hand experience.

----

## Known Issues and Limitations
- Some Voice Alerts won't work with NXi (Is not implemented by WT yet)
- Fuel consumption is not zero when engine isn't started (Bug by Asobo)
- Not compatible (not tested) with other mods which modify the C208 Grand Caravan EX

----

## Compatibility
- **Working Title's G1000 NXi**  rev 0.10.1 (recommended mod available on Sim Marketplace)

***Important Note:*** Please note that this mod has not been tested with the legacy freeware WT G1000. It is officially at end-of-life and will not be updated. Users should either use stock G1000 sim avionics or download Working Title Simulations G1000 NXi from the Marketplace.

----

## Download

***[Latest Release v2201.3](https://github.com/SheepCreativeSoftware/msfs2020-C208-Improvment-Mod/releases/latest)***

### How to install

1. Delete any previous versions.
2. Extract the Zip Archive
3. Copy the "C208B-mod" folder into the Community Folder.

----

## License
Microsoft Flight Simulator © Microsoft Corporation.  
Cessna 208B Grand Caravan EX Improvement Mod was created under Microsoft's "[Game Content Usage Rules](https://www.xbox.com/en-US/developers/rules)" using assets from Microsoft Flight Simulator and it is not endorsed by or affiliated with Microsoft.
