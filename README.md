# Homemade US Drone Lab

A practical path from a **home-built drone under 0.5 lb** (with optional 3D-printed parts) to high-performance, **primarily US-electronics** platforms.

This repo is for legal hobby and civil UAS work only: recreational flying under 49 U.S.C. §44809, or civil operations under 14 CFR Part 107. It is not a weapons, munitions, or targeting guide.

**Repo:** https://github.com/silentio-cmdq/homemade-us-drone-lab

---

## Short version — where to start

1. **Pass TRUST** (free, required for all recreational flyers, any weight). Carry the certificate.
2. **Buy a radio and fly a sim** for 8–20 hours before a first outdoor flight (Radiomaster + Liftoff or Velocidrone).
3. **Build a 65–75 mm whoop or 2–3.5" toothpick** with a 3D-printed or injection-molded frame. Target **all-up weight under 227 g (0.5 lb)** so you stay under both your stated limit and the FAA 250 g recreational registration line.
4. **Weigh the finished aircraft** with battery, props, camera, and antenna. If it crosses 250 g, register it before outdoor flight.
5. After that airframe is boringly reliable, step up: 5" FPV with a US stack → Pixhawk/ARK PX4 autonomy → endurance / heavy-lift (registered, Remote ID, usually Part 107).

3D printing is optional on day one. Use it for frames, canopies, battery trays, antenna mounts, and crash replaceables. Do not print motor mounts that flex under load unless you know the material.

Full write-up:

- [docs/00-faa-and-safety.md](docs/00-faa-and-safety.md)
- [docs/01-start-here-sub-250g.md](docs/01-start-here-sub-250g.md)
- [docs/02-path-to-high-performance.md](docs/02-path-to-high-performance.md)
- [docs/03-us-electronics.md](docs/03-us-electronics.md)
- [docs/04-3d-printing.md](docs/04-3d-printing.md)

---

## Repo map

```
README.md
docs/                      # the path
setups/
  01-whoop-3dprint/        # indoor / backyard micro
  02-35inch-sub250/        # outdoor cine / light freestyle under 250 g
  03-5inch-fpv-us/         # US-stack 5" FPV
  04-pixhawk-px4-us/       # autonomous / mapping class
firmware/                  # Betaflight diffs, PX4 notes, radio profiles
cad/                       # print settings and CAD notes (drop STLs here)
```

Each setup folder has a BOM, assembly notes, and a firmware stub. Replace vendor part numbers as stock changes. Prefer US-made or NDAA/Blue UAS listed parts when they exist; document substitutions when they do not.

---

## Weight math that actually matters

| Label | Mass | Why it matters |
| --- | --- | --- |
| Your target | **0.50 lb = 226.8 g** | The limit you asked for |
| FAA recreational registration | **0.55 lb = 250 g** | Recreational aircraft at or below this, flown only for fun, need no FAA registration |
| Part 107 | any weight | Commercial / work flights register every aircraft |
| Remote ID | registered aircraft | If it must be registered, it generally must broadcast Remote ID outdoors |

Takeoff weight includes battery, props, camera, antenna, tape, and GoPro if you bolted one on. Weigh it. Do not guess.

TRUST is still required under the recreational exception even if the aircraft is 80 g.

---

## Recommended first purchase order

1. Radio: Radiomaster Pocket or Boxer (ELRS).
2. Simulator.
3. Lipo charger + fire-safe bag + kitchen scale (0.1 g).
4. 1S whoop kit **or** printed 75 mm frame + 0802/1102 motors + 1S AIO board.
5. Extra props, extra printed arms, extra canopy.
6. Then a 3.5" sub-250 outdoor quad.

Do not start on a 5" 6S freestyle quad. That is how people buy a second radio after the first one eats a tree.

---

## Legal and safety baseline

- Recreational: TRUST, community-based safety guidelines, VLOS, 400 ft AGL in Class G unless authorized, no careless operation, no airports / TFR / restricted airspace without authorization. Check B4UFLY / LAANC.
- Over 250 g recreational: register at [FAA DroneZone](https://faadronezone.faa.gov/), mark the number on the exterior, carry proof.
- Any work / compensation / business-benefit flight: Part 107 Remote Pilot Certificate + per-aircraft registration + Remote ID.
- Lithium batteries: charge in a bag, never unattended on a wood desk, retire puffed packs.
- First flights: empty park, props off for bench test, then props on with a spotter.

Official FAA pages change. Recheck [Recreational Flyers](https://www.faa.gov/uas/recreational_flyers) and [Register Your Drone](https://www.faa.gov/uas/getting_started/register_drone) before you fly a new airframe.

---

## Honest note on "US electronics"

A fully domestic bill of materials is still incomplete in 2026. Flight controllers, some ESCs, some motors, and some radios have real US options (ARK Electronics, Unusual Machines / Rotor Riot, Hoverfly, ModalAI, KDE Direct, and others). Cells, rare-earth magnets, many cameras, and most analog VTX chains still lean on non-US supply. This repo prefers US parts first, then documents the gap instead of pretending it does not exist.
