# Setup 04 assembly and first autotune discipline

1. Mount the FC with vibration isolation. Arrow forward. No foam that turns to jelly in heat.
2. Calibrate power module on a known load before you trust current-based battery percent.
3. Compass / GNSS up and away from ESCs and video.
4. Load a close PX4 airframe, then create `ROMFS/px4fmu_common/init.d/airframes/XXXX_homemade_us` when you own the mix.
5. Bench: sensor check, actuator test with props off, failsafe to terminate or land — pick one and test it.
6. First flight is a manual hover in Stabilized, then Position over a huge empty field, then a 20 m square waypoint.
7. Geofence on from flight two.
8. After every flight: download the ulog, glance at vibration and clipping before you pack the car.

Do not copy a military concept of operations into this folder. Civil mapping and inspection only.
