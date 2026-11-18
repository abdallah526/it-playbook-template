---
icon: monitor-waveform
description: Zabbix monitors the network devices and links in every branch.
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
  anchors:
    visible: true
---

# Zabbix

### Overview

Zabbix is the team's network monitoring system. It watches the devices and connections in all branches, from the head office to every branch, and raises a problem when something stops responding.

### Where it runs

* **Location**: head office.
* **Server**: an Ubuntu server, with Zabbix deployed through Coolify.

### When to use it

* To check whether a branch, firewall or device is up before you start troubleshooting.
* Alongside [Splunk alerts](splunk/alerts/README.md) and [PRTG](prtg/README.md), when an alert fires and you need to see what else is affected.

{% hint style="info" %}
Ask your team lead for the Zabbix address and an account during your first week.
{% endhint %}
