# Setup 03 assembly

1. Square the frame. Bent arms go in the scrap box, not in the sky.
2. Soft-mount the Brave F7. Plug the harness if you are using the solderless path; still inspect every connector.
3. Flash Betaflight 4.5.1+ to `RRIOT_F722` (or the current published target). Do not flash an older major.
4. ESC protocol: DShot300 or DShot600 as the Brave 55A manual specifies. Bidirectional DShot on if you want RPM filtering.
5. ELRS on a free UART. GPS on a free UART if installed. Do not share those UARTs with the VTX unless the board docs say you can.
6. Set motor poles correctly or RPM filter will lie.
7. Bench hover, then a field with no people. Rates go up only after the motors track.

## Switch layout (suggested)

- SA: ARM
- SB: ANGLE / HORIZON / ACRO
- SC: BEEPER
- SD: FLIP OVER AFTER CRASH
- SE: GPS RESCUE if GPS is installed and tested
