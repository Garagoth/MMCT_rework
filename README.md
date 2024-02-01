This is a copy of yobeefjerky MMCT Cosmoteer mod.

### Changes compared to original

- Cables only connect with sides to each other.
- Cables and substations must be touching to connect as well.
- Substations can power everything in their radius, except for cables which have to be touching substations to exchange power.
- Capacitors can connect to cables and substations and push power to them, but then again, must be touching sides to work.
- Capacitors no longer exchange power between each other, subject to change in future maybe.
- Only wireless transfer is from substations (area around or line in front).

With heat the same, however I did tweak turbines a bit. Going with original values (and lowering some), now it is possible to:
- One core can produce heat to power 3 turbines fully loaded (previously impossible due to how heat was distributed)
- Each turbine can support 2.67 transformers, meaning third transformer will drain turbine, and this will provide 64 bat/sec (24/sec for each transformer).
- Thermal junction has more bandwidth to be able to push heat from core to 3 separate pipes and turbines at the end

### Problems

- This system is broken by loops in power grid.
  
  ![mmct_rework_powergrid_loops](https://github.com/Garagoth/MMCT_rework/assets/916161/f8458fa1-8a7b-4e44-a61e-afbe80b3331e)
- Loops of all kinds are possible, but they all divert power from where it needs to go. Eventually grid should saturate and power should flow where it is needed, but do not count on this to be efficient.
  
  ![mmct_rework_fun_loop](https://github.com/Garagoth/MMCT_rework/assets/916161/0288b7b9-7587-483a-9bdc-4ccab2afe695)


### Various Fixes

- Fixed larger hyperdrives to not be power black holes.
- Added stats to most parts

