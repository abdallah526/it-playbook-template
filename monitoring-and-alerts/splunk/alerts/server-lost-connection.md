---
description: >-
  This page explains the Server Lost Connection alert on the Splunk dashboard,
  its impact, and the steps to resolve it for servers like DC1, DC2, WDS, or
  others.
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

# Server Lost Connection

### Overview

* **Purpose**: To address a server outage (e.g., DC1, DC2, WDS) that disrupts services due to a lost connection.
* **Trigger**: Activates when a server request times out (e.g., ICMP error #11010, as seen with DC2).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the server lost connection alert for oversight and guidance.
2. **Verify Server Status**
   * Check the Splunk dashboard alert to confirm which server is down (e.g., DC2, DC1, WDS).
3. **Ping the Server**
   * Perform a ping test to the affected server from the branch’s firewall and an employee’s device.
   * See [Ping From Gateway](../../../network-and-infrastructure/sophos-firewall/how-to-guides/ping-from-gateway.md)
4. **Analyze Ping Results**
   * **If ping fails**: The server may be offline; coordinate with the IT Admin to check the server’s hardware or power status (e.g., during an outage).
   * **If ping succeeds**: The issue may be that the cable of the Ethernet port may be corrupted, which would cause a random lost connection or a need to change.
5. **Monitor and Resolve**
   * After taking action, monitor the server status via Ping to confirm it’s back online.
   *

{% hint style="info" %}
Act quickly to restore server connectivity. If the issue recurs, investigate potential hardware or network issues.
{% endhint %}
