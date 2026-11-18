---
description: >-
  This page explains the PBX VPN Connection alert on the Splunk dashboard for
  the RED tunnel between the head office firewall and Branch A PBX branch
  firewall (VoIP PBX server), its impact, and the s
layout:
  width: wide
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: false
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

# PBX VPN Connection

### Overview

* **Purpose**: To address a RED tunnel disconnection that disrupts VoIP communication (PBX server) between head office and Branch A.
* **Trigger**: Activates when the RED tunnel between the head office firewall and Branch A PBX branch firewall is down.


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the PBX VPN connection alert for oversight and guidance.
2. **Verify the Disconnection**
   * Confirm the tunnel status on the Splunk dashboard (e.g., Branch A PBX disconnected).
3. **Check Internet Connectivity**
   * Verify if the internet is operational in Branch A.
   * If down, follow: the internet outage runbook
4. **Check PBX Server Status**
   * If the internet is up, check if the PBX server in Branch A is operational.
   * See[ PBX Server is Down](../../../incidents-and-troubleshooting/pbx-server-is-down.md)
5. **Restart the RED Tunnel**
   * If both internet and PBX server are operational, restart the Branch A RED connection on the head office firewall. See [Restart RED Connection](../../../network-and-infrastructure/sophos-firewall/how-to-guides/restart-red-connection.md).
6. **Monitor Post-Action**
   * After restarting, confirm the RED tunnel is restored via Splunk.

{% hint style="info" %}
RED tunnel disconnections can disrupt VoIP services; resolve quickly.
{% endhint %}
