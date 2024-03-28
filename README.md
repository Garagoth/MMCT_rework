This is a modified version of [yobeefjerky's MMCT Cosmoteer mod](https://steamcommunity.com/sharedfiles/filedetails/?id=2885124288).
Uses art assets and ideas from original mod, with permission from original author.
Published as [Steam Workshop item](https://steamcommunity.com/sharedfiles/filedetails/?id=3170178280).

### Changes compared to original

- Cables only connect with sides to each other.
- Cables and substations must be touching to connect as well.
- Substations can power everything in their radius, except for cables which have to be touching substations to exchange power.
- Capacitors can connect to cables and substations and push power to them, but then again, must be touching sides to work.
- Capacitors exhange power with all power_storage parts.
- Only wireless transfer is from substations (area around or line in front).
- Added tech tree unlocks

With heat the same, however I did tweak turbines a bit. Going with original values (and lowering some), now it is possible to:
- One core can produce heat to power 3 turbines fully loaded (previously impossible due to how heat was distributed)
- Each turbine can support 2.67 transformers, meaning third transformer will drain turbine, and this will provide 64 bat/sec (24/sec for each transformer).
- Thermal junction has more bandwidth to be able to push heat from core to 3 separate pipes and turbines at the end

### Problems

- This system is broken by loops in power grid.
  To make it efficient, please make sure that there are no loops in cables (including most trivial case of four cables in a square)
  and no substation is in range of another substation (with some exceptions that can be found by experimentation).
  
  ![mmct_rework_powergrid_loops](https://github.com/Garagoth/MMCT_rework/assets/916161/f8458fa1-8a7b-4e44-a61e-afbe80b3331e)
- Loops of all kinds are possible, but they all divert power from where it needs to go. Eventually grid should saturate and power should flow where it is needed, but do not count on this to be efficient.
  
  ![mmct_rework_fun_loop](https://github.com/Garagoth/MMCT_rework/assets/916161/0288b7b9-7587-483a-9bdc-4ccab2afe695)


### Various Fixes

- Fixed larger hyperdrives to not be power black holes.
- Added stats to most parts

### New parts

- One way connector - acts as a diode AND a power pump, can suck power from capacitors and storages or feed power to parts in front of it.


