SentinelOne's reporting URI's are really tricky:
By setting up an agent on a client, the installation process requires having a Site Key (Base64 encoded license, containing the reporting URI):

```
{"url": "https://(continent)-(ce1, unclear at this point)-(random number).sentinelone.net", "site_key": "16 digit license key"}
```

So this config will report to the following AWS server, also containing the management dashboard:

```
nlb-(continent and ce1)-(random number)-(omitted, xxxxxxxxxxxxxxxx).elb.eu-central-1.amazonaws.com
```

Blocking rule can be considered as:

```
nlb-*-*-*.elb.*.amazonaws.com
```


Agents will fallback to try and communicate back directly to the AWS machine hostname. Complete AWS block is possible and may needed if there's no prior knowledge on the target's EDR solution.
