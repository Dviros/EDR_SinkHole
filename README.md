# EDR_SinkHole

## What's This About?

With everything going on with COVID-19 situation, a lof of organizational employees are using their endpoints outside of the safe perimeter of the organization.
But, DNS are still an issue in today's world:
We found out that by creating a DNS Sinkhole in the LAN's DNS server, and blocking specific addresses (mainly single ones per EDR), it it possible to remove visibility on the machine.

This simple and stupid method is quite easy to employ, either by a Rogue Wifi or a compromised DNS server.
