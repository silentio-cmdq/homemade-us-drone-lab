# Setup 01 — 75 mm 3D-printed whoop

**Role:** first homemade aircraft. Indoor / calm backyard. Recreational, no FAA registration if AUW stays under 250 g (it will).

**Target AUW:** 28–40 g with a 1S 450 mAh pack.

## Frame

- Printed 75 mm whoop, 25.5 mm AIO pattern, 40 mm props.
- Material: PETG or TPU 95A.
- Print settings: see `../../docs/04-3d-printing.md`.
- Mass target: 8–14 g.
- Bring a spare frame in the lipo bag.

Placeholder STLs live in `../../cad/whoop75/` once you drop files there. Until then, use a known 75 mm print-in-place whoop and record the source URL on the build card.

## Electronics (typical hobby 1S AIO class)

Document origin. These lines are usually mixed/imported at whoop size.

| Qty | Item | Spec | Est. mass |
| --- | --- | --- | --- |
| 1 | AIO FC | 1S, 5A, 25.5 mm, SPI ELRS or UART ELRS | 4–6 g |
| 4 | Motors | 0802 or 1102, 18000–26000 Kv class matched to 40 mm props | 2–3 g each |
| 4 | Props | 40 mm, several colors so you can see damage | — |
| 1 | Camera | 1/2" whoop cam or AIO cam | 2–4 g |
| 1 | VTX | often on the AIO; otherwise 25–100 mW whoop VTX | included or 1–2 g |
| 1 | Antenna | short 5.8 dipole or printed mount + whip | 1 g |
| 1 | Battery | 1S 300–550 mAh BT2.0 / PH2.0 | 8–15 g |
| — | Hardware | M1.4 screws, canopy, soft mounts | 2 g |

## Radio

- Radiomaster Pocket or Boxer, ExpressLFS 2.4 GHz.
- Bind phrase unique to this aircraft.

## Tools specific to this build

- M1.4 driver.
- Smoke stopper on first plug-in.
- Scale.

## Build card (copy to issues)

- Date built:
- AUW with pack X:
- Betaflight target:
- Bind phrase location:
- Failsafe: drop / no pulse
- Notes:
