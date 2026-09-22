# Start here: homemade drone under 0.5 lb

Goal: one flying quad you built, weighed, and can repair after a crash, without needing FAA registration for recreational flights.

## Pick one of two day-one airframes

### Option A — 65–75 mm whoop (best first aircraft)

- Indoor and calm backyard only.
- 1S, 0802 or 1102 motors, 31–40 mm props, AIO flight controller (FC + ESC + often RX on one board).
- Frame: buy a molded whoop frame **or** print one in PETG / TPU.
- Typical AUW: 25–45 g. Trivially under 0.5 lb.
- Why start here: crashes are cheap, parts are small, you learn binding, rates, props, and battery discipline without launching a 600 g knife.

See [setups/01-whoop-3dprint](../setups/01-whoop-3dprint).

### Option B — 2" to 3.5" toothpick / light cine (first outdoor aircraft)

- 2–4S, 1103–1407 motors, analog or lightweight HD.
- Hybrid frame: carbon plates + 3D-printed canopy, camera mount, and battery tray, **or** a fully printed 3 / 3.5" frame if you keep AUW honest.
- Budget the scale from the first screw. A naked 3.5" can sit at 180–230 g. A GoPro-class camera usually blows the 227 g cap.
- Fly this only after the whoop is easy.

See [setups/02-35inch-sub250](../setups/02-35inch-sub250).

Do not start with a 5" 6S freestyle quad.

## Skills before solder

1. TRUST certificate printed or on your phone.
2. Radio bound to a sim. Mode 2 unless you already fly something else.
3. Know what failsafe means and how to set it.
4. Know how to read a 1S voltage: 4.20 full, 3.50 land now, never store at 4.20.

## Tools

- Temperature-controlled iron, 60/40 or lead-free you can actually use, flux, 60/40 wick.
- Hex drivers: 1.5, 2.0 mm plus whoop-size bits (M1.4 / M2).
- Kitchen scale, 0.1 g.
- Smoke stopper or a current-limited bench PSU for first power-up.
- 3D printer if you want printed frames (Bambu / Prusa class is plenty).

## Electronics for the starter whoop

True US-made 1S AIO boards are scarce. Be honest on the BOM:

- Frame: printed at home (US) or molded whoop frame.
- AIO FC: hobby 1S AIO (often imported). Note the origin on the build card.
- Motors: 0802/1102; US micro motors are limited — document source.
- RX: ExpressLRS 2.4 GHz (some US assembly options exist; many modules are mixed).
- Battery: 1S 300–550 mAh. Cells are rarely US-made.
- Props: Gemfan / HQ 31 mm or 40 mm.

The point of build 01 is **process**, not a Blue UAS scorecard. Move the US-content fight to builds 03 and 04.

## Assembly order

1. Print or buy the frame. Deburr holes. Test-fit motors and AIO dry.
2. Mount motors. Check rotation later in Betaflight; do not glue threadlocker into windings.
3. Mount AIO on soft mounts if the frame has them.
4. Solder motors (or plug if the AIO is connectorized). Strain-relieve every wire.
5. Bind RX. Flash current Betaflight target. Set UART map from the board silkscreen, not from memory.
6. Motor direction + props off. Then props on, smoke stopper, short hover.
7. Weigh AUW. Write it on the battery tray.

## First flight profile

- Angle mode, low rates, indoor or waist-high grass.
- Land at 3.5 V/cell.
- After crash: check motor bells for grinding, inspect solder joints, reprint the broken arm the same evening.

When you can fly a packed figure-8 without thinking about the sticks, open [docs/02-path-to-high-performance.md](02-path-to-high-performance.md).
