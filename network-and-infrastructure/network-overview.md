---
icon: network-wired
description: How the network is laid out across sites.
---

# Network Overview

## Address plan

Describe the rule you use, for example: one /24 per site, VLAN ID equals the third octet.

## Sites

| Site | Subnets | Firewall | Internet links |
| --- | --- | --- | --- |
| Head office | `10.0.10.0/24`, `10.0.20.0/24` | Model | Fiber + 4G backup |
| Branch A | `10.1.10.0/24` | Model | VDSL |

## How the sites connect

* Site-to-site tunnels between the head office and branches.
* Remote access VPN for staff working outside the office.

{% hint style="info" %}
If the playbook is shared outside the IT team, keep exact IP addresses in a restricted place and link to it from here.
{% endhint %}
