# Network Intrusion Detection System Using Snort

## Introduction
This project was created to learn how Snort works as a basic Network Intrusion Detection System (NIDS) using Ubuntu in VirtualBox.

## Features
- Installed and configured Snort
- Added custom ICMP detection rule
- Monitored network traffic
- Detected ping packets and generated alerts

## Tools Used
- Ubuntu
- Snort
- VirtualBox

## Commands Used

```bash
snort -V
sudo nano /etc/snort/rules/local.rules
sudo snort -A console -q -c /etc/snort/snort.conf -i enp0s3
```

## Custom Rule

```bash
alert icmp any any -> any any (msg:"Ping Detected"; sid:1000001; rev:1;)
```

## Result
Snort successfully detected ICMP ping traffic and generated alerts.

## Conclusion
This project helped me understand basic network monitoring and intrusion detection using Snort.
