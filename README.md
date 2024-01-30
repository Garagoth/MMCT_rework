This is a copy of yobeefyerky MMCT Cosmoteer mod.

### Chanes compared to original

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

### Fixes

- Fixed larger hyperdrives to not be power black holes.
- Added stats to most parts

