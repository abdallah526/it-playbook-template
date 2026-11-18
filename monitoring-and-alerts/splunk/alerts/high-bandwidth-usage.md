---
description: >-
  Overview Purpose: To address excessive bandwidth consumption that can degrade
  network performance. Trigger: Activates when download traffic exceeds the
  warning limit.
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

# High Bandwidth Usage

### Overview

* **Purpose**: To address excessive bandwidth consumption that can degrade network performance.
* **Trigger**: Activates when download traffic exceeds the warning limit (e.g., Sophos 237 Mbit/s in Traffic In, above 190 Mbit/s).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT administrator or IT manager about the high bandwidth usage alert for oversight and guidance.
2. **Identify the Source**
   * Check the **Live Bandwidth Monitor** section on the Splunk dashboard to find the employee consuming high bandwidth (e.g., downloading or streaming high-quality video).
   * [Splunk Dashboard Overview](../dashboard.md)
3. **Verify Authorization**
   * Confirm if the employee is permitted to use high bandwidth based on their role or company policy.
4. **Check Firewall Rules**
   * Identify the firewall rule allowing this traffic via Sophos Firewall.
   * See ([Sophos Log Viewer](../../../network-and-infrastructure/sophos-firewall/how-to-guides/use-log-viewer.md)).
5. **Take Action**
   * If unauthorized, restrict the employee’s bandwidth or block the activity through the firewall rule in Sophos firewall after obtaining approval from the IT admin or IT Manager.

{% hint style="info" %}
Regularly monitor bandwidth to prevent network slowdowns.
{% endhint %}
