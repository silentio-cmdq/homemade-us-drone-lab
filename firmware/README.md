# Firmware lab

Per-setup firmware lives next to the aircraft:

- `setups/01-whoop-3dprint/firmware/` — Betaflight whoop starter
- `setups/02-35inch-sub250/firmware/` — add a dump when that airframe exists
- `setups/03-5inch-fpv-us/firmware/` — Brave F7 / Betaflight
- `setups/04-pixhawk-px4-us/firmware/` — PX4 params and airframe notes

## Rules for this folder

1. Never commit bind phrases, Wi-Fi passwords, or cloud API keys.
2. Commit `diff all` / QGC param exports with a date and AUW in the filename.
3. Flash official released firmware. Record the version in the commit message.
4. Props off for every first boot after a flash.
