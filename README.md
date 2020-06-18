# EDR_SinkHole

## What's This About?

With everything going on with COVID-19 situation, a lof of organizational employees are using their endpoints outside of the safe perimeter of the organization.
But, DNS are still an issue in today's world:

We found out that by creating a DNS Sinkhole in the LAN's DNS server, and blocking specific addresses (mainly single ones per EDR), it it possible to remove visibility on the machine in both telemetry and remote control processes.

Basically, machines will not be able to be remote controlled and no telemetry will be uploaded to the EDR's servers, potentially allowing attackers to start and launch attacks on the machine without the organizaion knowing.

It is important to mention that this method does not affect the functionality and usability of the EDR on the machine, but it will be helpful to kill the communications as part of the first step to achieving full EDR Evasion.

This simple and stupid method is quite easy to employ, with threats schenarios going from a Rogue Wifi or a compromised DNS server.


## Which EDR's Affected?
1. Microsoft's Windows Defender ATP
2. Carbon Black
3. Endgame?
4. SentinelOne?
5. Crowdstrike?
6. F-Secure?
7. Varonis?
