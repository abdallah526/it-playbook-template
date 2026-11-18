---
description: >-
  This page explains the RED Tunnel Status Issue alert on the Splunk dashboard
  for the VPN tunnel between the head office and remote branches, its impact,
  and the steps to resolve it.
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

# RED Tunnel Status

### Overview

* **Purpose**: To address a RED VPN tunnel disconnection between the head office and remote branches, which disrupts inter-branch communication.
* **Trigger**: Activates when the RED tunnel is down (e.g., Branch B shows <mark style="color:red;">RED</mark> colored).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the RED tunnel status issue alert for oversight and guidance.
2. **Verify the Disconnection**
   * Confirm the RED tunnel status on the Splunk dashboard (e.g., Branch B shows <mark style="color:red;">RED</mark> colored).
3. **Check Internet Connectivity**
   * Verify if the internet is operational in both head office and Branch B branches.
   * If down in Branch B:the internet outage runbook
4. **Check Firewall Status**
   * Access Sophos Central to confirm if the firewalls in both head office and Branch B are online.
   * [Sophos Central Access](../../../endpoint-security/sophos-central/how-to-guides/firewall-management.md)
5. **Restart the RED Tunnel**
   * If the internet and firewalls are operational, restart the RED tunnel:
     * In Sophos Central, navigate to the VPN settings for both branches.
     * Restart the RED tunnel configuration.
   * Monitor Splunk to see if the tunnel is restored (e.g., Branch B devices show online).
6. **Monitor Post-Action**
   * After restarting, confirm the RED tunnel is operational via Splunk (e.g., Branch B shows <mark style="color:green;">Green</mark> Colored).

{% hint style="info" %}
RED tunnel issues can disrupt branch operations; resolve quickly.
{% endhint %}
