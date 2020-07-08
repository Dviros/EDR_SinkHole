# EDR_SinkHole

## What's This About?

With everything going on with COVID-19 situation, a lof of organizational employees are using their endpoints outside of the safe perimeters of the organization.
But DNS are still an issue in today's world:

We found out that by creating a DNS Sinkhole in the LAN's DNS server (a method reserved for fighting Ransomewares) and blocking specific addresses (mainly single ones per EDR), it is possible to remove visibility on the machine in both telemetry and remote control processes.

Simply put, machines will not be able to communicate back to the EDR's servers, as no telemetry will be uploaded and no remote controls will be available, potentially exposing the machines to attackers, allowing them to start and launch attacks on the machine without the organization’s knowledge.

This can be done without editing the machine's "host" file as it involves a highly privilege action, which is highly noticeable.

It is important to mention that this method does not affect the functionality and usability of the EDR on the machine, but it will be helpful to disrupt the communications as part of the first step to achieving full EDR Evasion:
A triggered EDR alert will not be uploaded and communicated back!

This simple and stupid method is quite easy to employ, with threats scenarios going from a Rogue Wifi or a compromised DNS server.


## Which EDR's Affected?
1. Microsoft's Windows Defender ATP
2. Carbon Black
3. SentinelOne - Not so much

### To be Checked:
1. Elastic Endpoint (Endgame)?
2. Crowdstrike?
3. F-Secure?
4. Varonis?
5. CORTEX (palo alto)?
6. CyberReason?
7. Tenium?
8. TrendMicro?
9. McAffee ATP?

## Recommendations
EDR vendors should offer their customers a list of dynamically changed telemetry gateways, ranging across the world, in order to try and communicate back in any case of network tampering.

These dynamic gateways should use masked and hard to identify addresses to make it harder for attackers to distrupt communications.

Implementing communications disruption detection mechanism, that will be triggered once a disruption was identified.
