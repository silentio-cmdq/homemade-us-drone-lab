# ExpressLRS radio notes

- Unique bind phrase per aircraft, stored off-repo.
- 2.4 GHz for whoops and short-range 5". 900 MHz only if you understand antennas, duty cycle, and the fact that long range is how people lose visual line of sight.
- Dynamic power on. Telemetry on so the TX can shout at you before the pack dies.
- Failsafe on the aircraft is DROP unless a PX4 mission profile has a tested land/RTL and you are flying that stack.
