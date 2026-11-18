---
description: >-
  This page explains the Switch Lost Connection alert on the Splunk dashboard
  for any switch in the network, its impact, and the steps to resolve it.
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

# Switch Lost Connection

### Overview

* **Purpose**: To address a connection loss to any switch in the network, which can disrupt connectivity for devices connected to it.
* **Trigger**: Activates when a switch becomes unreachable (e.g., ICMP error #11003).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the switch lost connection alert for oversight and guidance.
2. **Verify the Alert**
   * Confirm the connection loss on the Splunk dashboard, identifying the affected switch (e.g., by IP or name).
3. **Check Power and Hardware**
   * Verify if there’s an electric outage affecting the switch.
   * If no power issue, ensure the switch is powered on and cables (e.g., Ethernet, power) are securely connected.
4. **Ping the Switch**
   * Perform a ping test to the affected switch from the branch’s firewall or an employee’s device to confirm connectivity.
5. **Restart the Switch**
   * If the ping fails, restart the switch:
     * Unplug the switch, wait 30 seconds, then plug it back in.
6. **Check Network Configuration**
   * If the switch is still unreachable, verify the network configuration:
     * Check for recent changes in VLANs, IP settings, or firewall rules that might block the switch.
7. **Monitor Post-Action**
   * After taking action, confirm the switch is reachable via Splunk (e.g., ping succeeds, devices reconnect).

{% hint style="info" %}
Switch outages can disrupt local network access; resolve quickly. If frequent, investigate hardware health or network configuration issues.
{% endhint %}
