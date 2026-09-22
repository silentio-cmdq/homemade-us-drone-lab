# Setup 04 — US autopilot class (PX4)

**Role:** waypoints, mapping, inspection, research. This is the start of "insane" in the engineering sense.

**Regulatory default:** Part 107 + registration + Remote ID for any mission that is not pure recreation.

## Brain

| Item | First choice | Why |
| --- | --- | --- |
| Flight controller | ARK Electronics ARKV6X or ARKV6S | US, Pixhawk bus, PX4 |
| Carrier / IO | Matching ARK carrier | Power rails and connectors you can document |
| ESC | ARK 4-in-1 or documented NDAA singles | Current sense you trust |
| GNSS | Dual GNSS + compass on masts | Heading and redundancy |
| Power module | Board the FC vendor supports | Voltage + current into PX4 |
| Companion (optional) | ARK Pi6X path or US-carrier compute | Offboard, CV, logging |
| Remote ID module | FCC-capable module that PX4/the airframe can host | Required once registered and outdoors |
| Frame | 7–10" quad or small endurance airframe | Printed fairings, carbon structure |
| Motors | KDE Direct or Hoverfly class | Documented industrial motors |

## Ground station

- QGroundControl on a laptop you actually take to the field.
- Parameter files live in `firmware/px4/` in this setup.
- One operator, one observer until you have a waiver story you can defend.
