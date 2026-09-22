# Primarily US electronics

Use this as a living vendor map. Stock and Blue UAS listing status change. Verify origin and listing before a procurement that depends on NDAA language.

## What "US" can mean

1. Designed, assembled, and tested in the United States.
2. NDAA-compliant / Blue UAS Framework listed (supply-chain rules, not a patriotism sticker).
3. Final assembly in the US on imported subcomponents.

This repo labels parts as **US-made**, **NDAA/Blue listed**, or **imported / mixed**. Do not mix those words.

## Flight controllers

| Part | Maker / site | Notes |
| --- | --- | --- |
| Rotor Riot Brave F7 | Unusual Machines / Rotor Riot, Orlando, FL | FPV, Betaflight target `RRIOT_F722`, ~8 g, 30×30 mount, Blue UAS listed at introduction |
| ARKV6X / ARKV6S | ARK Electronics, Salt Lake City, UT | Pixhawk Autopilot Bus, PX4, NDAA-focused |
| ARK FPV | ARK Electronics | FPV-oriented ARK board with payload power |
| ARK Pi6X / Pi6X Flow | ARK Electronics | Compute + FC path |
| Holybro Pixhawk 6X | Mixed; widely used reference | Not a US-origin board; useful as a pin-compatible stand-in while you wait on ARK stock |

Brave F7 is the realistic first US FPV FC. ARK boards are the realistic first US autopilot FC.

## ESCs

| Part | Maker | Notes |
| --- | --- | --- |
| Rotor Riot Brave 55A 4-in-1 | Unusual Machines | Paired with Brave F7, Blue UAS listed |
| ARK 4-in-1 ESC | ARK Electronics | 3–8S class, NDAA-focused |
| Triumph NDAA ESC series | Triumph Manufacturing | AM32, single and 4-in-1 |
| ModalAI ESC series | ModalAI | VOXL ecosystem, US manufactured |
| Hoverfly Elements ESC | Hoverfly | Defense / commercial lean |

Hobby 1S AIO ESCs for whoops remain mostly imported. Do not stall Stage 1 waiting for a US 1S AIO.

## Motors

| Part | Maker | Notes |
| --- | --- | --- |
| Brave series 2207 / 2807 / 3220 | Unusual Machines | FPV sizes, US manufacturing push, rare-earth magnet provenance still a watch item |
| KDE Direct | US industrial motors | Excellent documentation, heavier and costlier, good on Stage 4–5 |
| Hoverfly Elements motors | Hoverfly | Commercial / defense |
| USA Drone Motors | Southern California (emerging) | Watch for ag / heavy-lift sizes |

Micro 0802/1102 whoop motors: imported is still the default. Print the frame in the US and move on.

## Compute, radios, GNSS, video

- **Companion computers:** US carriers around Raspberry Pi CM / NVIDIA / Qualcomm modules exist; the module origin is mixed. ARK Pi6X is the cleanest FC+compute story in this list.
- **Radios:** Radiomaster (TX16S, Boxer, Pocket) is the practical hobby standard. ExpressLRS firmware is open. Treat the radio as mixed-origin unless a specific US module is on the bench.
- **GNSS:** Septentrio-class receivers show up on higher-end US integrators; u-blox modules are common and mixed-origin. Dual GPS + compass is the Stage 4 baseline.
- **Video:** analog VTX and most lite HD cameras are the thinnest US category. Budget imported video on Stages 1–2. For later stages, document the camera serial and do not pretend it is domestic if it is not.
- **Batteries:** cells are the structural weakness of any "US drone" claim. Buy quality packs, store them correctly, and write the cell brand on the build card.

## Firmware that matches the hardware

- Brave F7: Betaflight 4.5.1+ on target `RRIOT_F722` (confirm current target notes before flash).
- ARK Pixhawk-bus: PX4 first. ArduPilot if you already live in that world.
- ESCs: BLHeli_32 or AM32 as specified by the vendor. Do not cross-flash "because a forum said so."
- Radios: ExpressLRS current release. Bind phrase in a password manager, not on a sticky note on the pack.

## Procurement habit

Every setup folder has a `BOM.md`. For each line record:

- manufacturer
- country of assembly if known
- firmware target
- mass in grams
- date bought
- replacement URL or SKU

That table is how a hobby bench becomes an engineering bench.
