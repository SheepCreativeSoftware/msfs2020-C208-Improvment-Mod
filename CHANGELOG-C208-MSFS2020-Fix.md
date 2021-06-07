## Changelog [C208-MSFS2020-Fix](https://github.com/Exp232/C208-MSFS2020-Fix)

***Changelog v0.4.3***

- Added [Uwajimaya's light mod](https://uwajimaya.github.io/FS2020/). Thanks to Uwajimaya and D33pfield for the help.

***Changelog v0.4.2:***

- PFD horizon default is back to synthetic vision on so those who don't have Working Title's G1000 mod installed can use it as well. (but I strongly recommend you download the mod, it's great!).
- Corrected some wrong textures in the de-ice system. "FLUD CONTROL" changed to "FLUID CONTROL" and "HORN" changed to "NORM".

***Changelog v0.4.1:***

- Fixed some bugs to make it compatible with the [Working-Title G1000 mod](https://github.com/Working-Title-MSFS-Mods/fspackages) and the [msfs_pfd_color_modification](https://github.com/guifarias31/msfs_pfd_color_modification).
- The PFD will start with the Synthetic Vision off by default now (download the Working-Title G1000 mod to be able to change it).
- Autopilot tuned (It's less abrupt now).
- Flight model tuned.

***Changelog v0.4.0:***

- DELETE THE PREVIOUS VERSION OF THE MOD AND THEN INSTALL THIS ONE.
- The mod should work well with the latest version of MSFS.
- The Ng text indicator in the G1000 MFD now displays unit by unit (before it displayed every 10%).
- Now you have to actually move the condition lever close to the LOW IDLE position in order to get fuel flow during start.
- Ng, ITT and TRQ values during start tuned.
- Fuel consumption: this is a problem that has been very hard to deal with. As you may know, in the previous version of MSFS the available TRQ actually increased in higher flight levels, which is to say the least, a bit odd. This seems to be fixed in this new patch, so I reworked the consumption modifications I had made, and corrected the power (or brake) specific fuel consumption of the engine. In my test flights I had a little lower fuel consumption than the predicted in the POH. It seems acceptable to me for now.
- PFD Screens during start: In the normal start procedures you should turn the avionics 1 switch on, which should bring the left PFD on in reversionary mode (with the engine parameters in the left). After engine start you should switch on the avionics 2 and then the MFD and right PFD should turn on and the left PFD should go back to normal mode. However it looks like there's no working reversionary mode in the MSFS G1000 yet, so there's not much I can do about it for now. After the update the avionics 1 (without my mod) would turn on both PFD screens but not the MFD, which would turn on only after the avionics 2 switch was turned on. So, in order to make everyone able to at least follow the correct flight procedures I changed it back to the way it was - Avionics 1 switch turns right PFD and MFD on and Avionics 2 switch turns left PFD on. This way you can have the engine parameters indicators during start and only turn the avionics 2 on after start.
- Engine power tuned.
- Reverse power tuned.
- Ng to TRQ table tuned.

***Changelog v0.3.4:***

- Yaw damper is now functional thanks to D33pfield.

***Changelog v0.3.3:***

- Fixed a bug with ITT/Torque during takeoff.

***Changelog v0.3.2:***

- Adjusted the fuel consumption that was too high. Now it's closer to what it should be at least in the altitudes and settings I've tested, please let me know if you find any problems, I'm still trying to understand how to adjust the fuel parameters.
- The prop doesn't start in the feathered angle anymore when the plane is off at the ramp. The blade angle changing even when the engine is shutdown is unrealistic, so I decided not to change this until I can find a way to properly simulate the propeller governor/feathering.
- Adjusted the values of Torque, Ng, ITT and FF during engine start to match the values of the real plane. Not the exact same values but I think it's pretty close. Thanks to Trevor for all the information and feedback he is providing.


***Changelog v0.3.1:***

- Idle power tuned, the plane now shouldn't start moving so easily when you release the brakes.
- Engine power tuned.
- Fuel consumption tuned.
- Flight Model tuned.
- Now when you start a flight with the plane in the "cold and dark" state the condition lever is in the CUTOFF position intead of the HIGH IDLE position.
- When you start the flight with the plane in "cold and dark" the propeller is feathered* (read note below) as it should be, but instead of slowly moving to the right angle during engine start as the oil pressure builds up, it just moves when you move the prop lever to max before start, even when the engine is off (this is a problem that will try to solve later, but it might require some custom coding to work the way it should).
- Increased the range that the prop lever control the prop rpm in an attempt to get it to feather, and now you can reduce it to around 200 RPM. This is still a work in progress.
- Got the reverse thrust working. It might be overpowered or underpowered though, I'll adjust it in the next updates, but now it works :-).

* The prop still won't feather. I can get it to move to an angle that is close to what the feather angle should be but it still doesn't feather, the only thing you can do is reduce a lot the RPM. I'll keep trying to improve this.

Some other things to keep in mind:
- The beta range (before the reverse) doesn't really do anything now.
- Fuel consumption and climb/cruise power seem to be working the way they should according to the POH I use as reference, but if you notice any abnormalities or bugs please feel free to open an issue or contact me.

***Changelog v0.3:***

- Engine performance tuned.
- Fuel consumption tuned.
- Flight model changes: I tried to tweak the flight model to increase the drag generated from the flaps, mainly when using full flaps.
- Corrected Ng values at idle power with condition lever at high idle and low idle.
- Stall speeds corrected.
- Propeller angles corrected in the engines.cfg file but the propeller won't feather at all.
- Now you can install it the right way via the "Community" folder (I think it's working).


***Changelog v0.2:***

- Climb/cruise speeds corrected.
- Elevator trim actuation is now much more smooth than it was before.
- Engine Power tuned (the plane might feel a little overpowered, but I'm still fine tuning the power output).
- Fuel consumption tuned (now it's closer to what it should be, I'll try to improve it).
- AP FD GA angle reduced.
- Idle Ng corrected.

***Changelog v0.1:***

- Improved the Ng% -> Torque ratio so it delivers more torque with less Ng%, which resulted in a small gain of performance.

- Improved the Fuel Flow of the aircraft. I'm still doing test flights and as of now it consumes around 100 lbs of fuel less than it should in a flight as per the tables available in the POH. Will try to improve this.

- With this mod, I was able to make a flight following the power settings available in the POH and had a performance close to what it should be. I was able to keep the torque within the limits of the POH while maintaining the desired cruise airspeed. The ITT is still lower than it should be (it doens't limit your torque, you actually can go all the way up to around 2000 lbs/ft of torque and keep the ITT in the green, which shouldn't happen according to the POH).