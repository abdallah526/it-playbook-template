---
icon: network-wired
description: How the network is laid out across sites.
---

# Network Overview

## Address plan

Describe the rule you use, for example: one /16 per site (`172.20.0.0/16` for the head office, `172.21.0.0/16` for Branch A), and the VLAN ID is the third octet.

## Sites

| Site | Subnets | Firewall | Internet links |
| --- | --- | --- | --- |
| Head office | `172.20.11.0/24`, `172.20.21.0/24` | Model | Fiber + 4G backup |
| Branch A | `172.21.11.0/24` | Model | VDSL |

## How the sites connect

* Site-to-site tunnels between the head office and branches.
* Remote access VPN for staff working outside the office.

{% hint style="info" %}
If the playbook is shared outside the IT team, keep exact IP addresses in a restricted place and link to it from here.
{% endhint %}
