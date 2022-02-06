# OPNsense

## OPNsense Cron job


Place the file `philips.rules` in `/usr/local/etc/suricata/rules/` and reload suricata / Intrusion Detection

You can also place the following code in your crontab by using `crontab -e`:

```shell
wget https://raw.githubusercontent.com/janwiesemann/suricata-no-philips-metrics/main/philips.rules -O /usr/local/etc/suricata/rules/philips.rules && /usr/local/opnsense/scripts/suricata/installRules.py && pkill -USR2 suricata

```
