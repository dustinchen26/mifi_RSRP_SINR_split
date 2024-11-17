# Parse_RSRP_draw

online tool => https://dustinchen26.github.io/mifi_RSRP_SINR

## Example
```
【How to use】
step0. Set the UE time correctly. ex:
date -s "2024-08-20 09:03:50"
step1. MobaXterm Session -> SSH -> Termnial settings -> Select "Log terminal output to": _DesktopDir_
step2. ssh into mifi. ex: 10.205.164.22
step3. "Mifi" use below command to run 10 times
watch -n 1 'echo "$(date "+%Y-%m-%d %H:%M:%S")"; atcli at+cesqdbm'
step4. paste the _DesktopDir_ output file content below to parse

【Input】
~ # watch -n 1 'echo "$(date "+%Y-%m-%d %H:%M:%S")"; atcli at+cesqdbm'
Every 1s: echo "$(date "+%Y-%m-%d %H:%M:%S")"; atcli at+cesqdbm                                                                                                                        2024-11-13 12:37:23
2024-11-13 12:37:23
at+cesqdbm
+CESQDBM:
SYSTEM:NR5G-SA
Band 79
NR5G: RSRQ -11 dB, RSRP -74 dBm, SINR 33 dB
OK

Every 1s: echo "$(date "+%Y-%m-%d %H:%M:%S")"; atcli at+cesqdbm                                                                                                                        2024-11-13 12:37:24
2024-11-13 12:37:24
at+cesqdbm
+CESQDBM:
SYSTEM:NR5G-SA
Band 79
NR5G: RSRQ -11 dB, RSRP -73 dBm, SINR 34 dB


【Output】

```
