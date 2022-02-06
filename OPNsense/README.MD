# OPNsense

## OPNsense Cron job

### Easy

Run the following Command:

```shell
wget https://raw.githubusercontent.com/janwiesemann/suricata-no-philips-metrics/main/OPNsense/actions_updateSuricataPhilipsRules.conf -O /usr/local/opnsense/service/conf/actions.d/actions_updateSuricataPhilipsRules.conf
```

afterward you can create a cron job under `System` -> `Settings` -> `Cron`


### Advanced

Place the file `philips.rules` in `/usr/local/etc/suricata/rules/` and reload suricata / Intrusion Detection.
