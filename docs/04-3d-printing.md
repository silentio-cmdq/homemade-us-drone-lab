# 3D-printed parts for homemade drones

Print what takes impacts and changes shape. Buy or machine what takes continuous motor torque.

## What to print

**Good print jobs**

- Whoop frames (65–75 mm)
- Canopies and camera pods
- Battery trays and straps anchors
- Antenna mounts and TPU bumper corners
- GoPro / lite-camera wedges
- Motor guards / ducts on cinewhoops
- Bench fixtures, prop gauges, soldering jigs

**Print only with eyes open**

- Full 3" / 3.5" frames: possible, common, and heavier/softer than 3K carbon. Stay in the sub-250 g budget with thin walls and no hero ducts.
- 5" arms: TPU or nylon-CF can work as crash replaceables. A printed 5" arm is not a race arm.

**Do not print as primary structure**

- Motor bells, prop hubs, high-current ESC mounting that needs heat sinking through metal, anything that must hold a folding prop bolt on a 2 kg lift quad unless you have tested that exact part.

## Materials

| Material | Use | Notes |
| --- | --- | --- |
| PETG | Whoop frames, trays | 3–4 walls, 0.16–0.20 mm layers. Tough enough for micro impacts |
| TPU 95A | Bumpers, ducts, battery pads, 5" corner bumpers | Slow print, great crash survival |
| PLA+ | Prototypes only | Brittle in sun and after a few outdoor packs |
| PA-CF / PC-CF | Outdoor 2.5–3.5" printed frames | Stiffer, needs dry filament and a competent hotend |
| ABS/ASA | Canopies in sun | Warp risk; enclosure helps |

Whoop starting recipe: PETG, 0.16 mm, 3 walls, 30–40% gyroid, no supports if the STL is printed-in-place, 8–15 g frame target.

## Design rules that keep aircraft in the air

- Motor holes: match the real motor pattern (M1.4 / M2) and leave a boss thick enough that a stripped hole can be heat-set later.
- FC patterns: 25.5 mm whoop AIO, 20×20 micro, 30.5×30.5 standard stack. Model the rubber grommet, not just the hole.
- Wire paths: leave a chamfered slot so motor wires do not saw the arm.
- Battery: center of mass near the FC. Top-mount 1S on a whoop is usually calmer than a sloppy belly strap.
- Ducts (whoop / cine): inner diameter must clear the prop + a crash margin. A pretty duct that rubs a prop is a heat gun.

CAD: Onshape or Fusion is enough. Keep STEP + STL in `cad/` once you own a design. Do not commit 200 MB of slicer projects.

## Crash loop

Print two frames on day one. When you break one, reprint that night and fly tomorrow. That loop is the actual advantage of a printed micro, not saving $8 versus a molded whoop frame.

## Mass discipline

Weigh every printed part. Write grams in the filename: `whoop75_frame_petg_11g.stl` is more useful than `final_final2.stl`.
