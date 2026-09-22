# PX4 notes for Setup 04

- Build PX4 from a tagged release, not a random `main` commit you cannot name next month.
- Board: use the ARK-supported PX4 target for ARKV6X / ARKV6S (confirm on current ARK + PX4 docs).
- Keep `params.params` exports in this folder, one file per airframe revision.
- Airframe mixers and startup files belong here once they exist.

Minimum parameters to set on purpose:

- Battery cell count and empty/full voltages
- CBRK_IO_SAFETY only with a reason written next to it
- COM_RC_LOSS_T and failsafe action
- GF_ACTION and a fence that is smaller than the field
- EKF2 GNSS and magnetometer enables that match the hardware you actually installed
