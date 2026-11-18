---
description: >-
  This page explains the UPS Alerts on the Splunk dashboard for the UPS-01
  UPS in the head office, its impact, and the steps to address an electrical
  cut causing the UPS to switch to battery power.
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

# UPS Alerts

### Overview

* **Purpose**: To address a UPS switching to battery power due to an input power problem, ensuring minimal downtime for critical systems.
* **Trigger**: Activates when the UPS (e.g., UPS-01) detects an input power issue and switches to battery (e.g., IPs 172.20.31.4 for Floor 2, 172.20.31.5 for Floor 1).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the UPS alert for oversight and guidance.
2. **Verify the Alert**
   * Confirm the UPS alert on the Splunk dashboard (e.g., UPS-01 on battery power, IPs 172.20.31.4 and 172.20.31.5).
3. **Check Power Status**
   * Verify if there’s an electric outage in the head office affecting the UPS.
   * [Electric Outage at a Branch](../../../incidents-and-troubleshooting/electric-outage-at-a-branch.md).
4. **Monitor UPS Runtime**
   * Check the remaining runtime on the UPS units (e.g., 10h 49m for Floor 1, 2h 40m for Floor 2).
   * Instruct employees to shut down non-essential devices to extend UPS runtime.
5. **Monitor Post-Action**
   * Once power is restored, confirm the UPS switches back to AC power via Splunk (e.g., voltage returns to 227-228 V AC).
   * [Splunk Quick Start](../dashboard.md)

{% hint style="info" %}
UPS alerts indicate power issues that can lead to downtime; act quickly to conserve battery.
{% endhint %}
