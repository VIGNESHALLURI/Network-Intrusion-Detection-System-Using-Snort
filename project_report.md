# Project Report

## Project Title

Network Intrusion Detection System Using Snort

## Introduction

I created this project to learn how Snort works as a Network Intrusion Detection System (NIDS). The project was done on Ubuntu using VirtualBox. Snort was configured to monitor network traffic and detect ICMP ping packets using a custom rule.

## Objective

The main aim of this project was to understand basic intrusion detection concepts and monitor ping traffic in real time using Snort.

## Tools Used

* Ubuntu Linux
* Snort
* VirtualBox

## Project Explanation

First, Ubuntu was installed inside VirtualBox. After setting up the environment, Snort IDS was installed and configured properly. A custom ICMP detection rule was added in the local.rules file to detect ping packets.

After configuration, Snort was started in console mode to monitor network traffic. When ping packets were generated, Snort displayed alert messages successfully in the terminal.

The following command was used to run Snort:

```bash
sudo snort -A console -q -c /etc/snort/snort.conf -i enp0s3
```

When ping packets were generated, Snort successfully displayed alert messages in the terminal.

## Result

The project successfully detected ICMP ping traffic and generated alerts in real time using Snort.

## Conclusion

This project helped me improve my understanding of Linux commands, basic networking, and intrusion detection systems. I also learned how custom Snort rules work for monitoring network traffic.
