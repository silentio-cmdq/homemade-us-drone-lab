# Full path: starter whoop to high-performance US-electronics aircraft

"Insane" here means high thrust-to-weight, clean video, long endurance, or autonomy — not a weaponized airframe.

## Stage 0 — paper and thumbs (week 0)

- TRUST.
- Radio + sim.
- Read [docs/00-faa-and-safety.md](00-faa-and-safety.md).
- Buy a scale and a charger. These two tools prevent more grief than any carbon plate.

## Stage 1 — micro you can crash (weeks 1–4)

**Airframe:** 65–75 mm whoop, printed or molded.  
**Mass:** 25–45 g.  
**Firmware:** Betaflight on an AIO.  
**Win condition:** bind, hover, punch-out indoors, repair a broken arm in one evening.

Folder: `setups/01-whoop-3dprint`

## Stage 2 — first outdoor quad under 0.5 lb (weeks 4–10)

**Airframe:** 2" to 3.5" toothpick or light cinewhoop. Carbon + printed parts preferred.  
**Mass budget:** ≤ 220 g AUW with analog or a true lite HD system. No full GoPro if you want to keep 0.5 lb.  
**Firmware:** Betaflight or a lightweight INAV build if you want GPS rescue later (GPS will eat the mass budget).  
**Win condition:** pack a picnic-table flight, come home with footage, still weigh under 227 g.

Folder: `setups/02-35inch-sub250`

Register the moment a camera or GPS pushes you over 250 g. Add Remote ID if required.

## Stage 3 — 5" FPV with a US stack (months 3–8)

**Airframe:** 5" freestyle or cinematic, carbon frame, printed TPU ducts / camera protection.  
**Mass:** typically 450–750 g. This is a registered aircraft.  
**US-leaning stack examples:**
- FC: Rotor Riot Brave F7 (Unusual Machines, Orlando) or ARK FPV / ARKV6X class boards (ARK Electronics, Utah).
- ESC: Rotor Riot Brave 55A, ARK 4-in-1, Triumph / other NDAA-listed ESCs when in stock.
- Motors: Unusual Machines Brave series, KDE Direct (industrial), Hoverfly Elements where the size fits.
- Radio: Radiomaster with ELRS; keep the module documented.

**Firmware:** Betaflight 4.5+ on Brave F7 (check current target), or PX4 on ARK boards if you want an autopilot path instead of stick freestyle.

**Win condition:** tuned 5" that survives a pack of packs, blackbox you can actually read, failsafe that drops motors instead of fly-away.

Folder: `setups/03-5inch-fpv-us`

Get the Part 107 certificate during this stage if any flight is for work. Do it anyway if you want airspace flexibility.

## Stage 4 — autopilot class (months 6–18)

**Airframe:** 7–10" or small VTOL / quadplane if you have the bench time.  
**Brain:** ARK Electronics Pixhawk-bus boards (ARKV6X, ARK Pi6X, ARKV6S) running **PX4** or ArduPilot.  
**Why this is the "insane" step:** waypoints, geofence, log analysis, payload power rails, RTK GPS, companion computer (US options around NVIDIA / Qualcomm compute on a US carrier).  
**Compliance:** registered, Remote ID, Part 107 for almost every interesting mission.

Folder: `setups/04-pixhawk-px4-us`

## Stage 5 — endurance and heavy lift (year 2+)

This is systems engineering, not a shopping list.

- Power: 8S–12S capable US ESCs, documented motors (KDE, Hoverfly, USA Drone Motors class vendors), packs you can name the cell source of.
- Airframe: carbon / aluminum / printed nylon-CF hybrid. Print fixtures and fairings, machine the spars.
- Avionics: redundant IMU boards from ARK, dual GPS/compass, power module with current sense you trust.
- Software: PX4 airframe file in this repo, CI on parameter sets, bench-test scripts.
- Ops: written checklist, pack log, maintenance log, insurance if you fly near other people’s property.

Stay under 55 lb unless you want a completely different FAA process.

## Skills that compound

| Stage | Skill you must keep |
| --- | --- |
| 1 | Solder, Betaflight dump, pack care |
| 2 | Weight budget, antenna placement, tuning without copy-paste PID |
| 3 | Blackbox, notch filters, US supply chain reading |
| 4 | PX4 airframes, QGroundControl, geofence, log review |
| 5 | Power budgets, thermal, reliability, ops manuals |

## Suggested spend (order of magnitude, 2026 hobby prices)

- Stage 1: $150–300 plus radio/sim if you do not own them.
- Stage 2: $250–500.
- Stage 3 US-leaning: $700–1500.
- Stage 4: $2k–8k depending on sensors.
- Stage 5: do not start without a mission and a notebook.
