# suricata-no-philips-metrics

Blocks Philips hue devices from sending metrics

Philips devices are not just using you speecified DNS-Server. They are also trying to connect to googles DNS-Server. These rules allow you to block specific domains, which are related to diagnostics and metric collection. Fell free to some domains and to create a pull request.

## OPNsense

Place the file 'philips.rules' in '/usr/local/etc/suricata/rules/' and reload suricata / Intrusion Detection
