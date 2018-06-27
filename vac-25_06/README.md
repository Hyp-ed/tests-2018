# Vacuum chamber testing on 25/06

## Tests performed and data collected
1. Idle BBB CPU temperature during evacuation
    * BMS data in `evacuation.txt`, `evacuation2.txt`, `evacuation3.txt`
    * BBB and RPi CPU temperatures in `temp-log-evacuation.csv`
2. Full load BBB CPU temperature under vacuum
    * BMS data in `vacuum_cpu.txt`
    * BBB and RPi CPU temperatures in `temp-log-cpu.csv`
3. BMS load test under vacuum
    * BMS data in `vacuum_bms.txt`
    * BBB and RPi CPU temperatures in `temp-log-bms.csv`

## Data format
All the `.txt` files contain timestamped proxi, IMU, and BMS data in a human-readable format. Only `bms0` is relevant (all the other
sensors were disconnected). The `.csv` files have 3 columns - timestamp, BBB CPU temperature in degC, and RPi CPU temperature in degC.
The absolute values of the timestamps are irrelevant since the clocks on both BBB and RPi were out of sync with real time and one another.
