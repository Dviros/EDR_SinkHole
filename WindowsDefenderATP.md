![Screenshot of WDATP Live Response](https://raw.githubusercontent.com/Dviros/EDR_SinkHole/master/Screens/WDATP.png)

Blocking the following will disrupt telemetry upload and Remote Investigation (limited remote shell), but will allow the machine to appear as "Online":

```
winatp-gw-neu.microsoft.com

eu-v20.events.data.microsoft.com

wdatpprd-eu.securitycenter.windows.com

winatpservicehealth.securitycenter.windows.com



*.events.data.microsoft.com

wdatpprd-*.securitycenter.windows.com

winatp*.microsoft.com
```
