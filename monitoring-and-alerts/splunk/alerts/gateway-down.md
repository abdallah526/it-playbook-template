---
description: >-
  This page explains the Gateway Down alert on the Splunk dashboard for gateways
  in the head office (e.g., Fiber, VDSL router, 4G router), its impact, and the
  steps to resolve it.
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

# Gateway down

### Overview

* **Purpose**: To address a gateway outage (e.g., Fiber, VDSL router, 4G router) in the head office that disrupts internet connectivity.
* **Trigger**: Activates when the internet connection for a gateway (e.g., the fiber router) is down


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the gateway down alert for oversight and guidance.
2. **Verify the Outage**
   * Confirm the gateway outage on the Splunk dashboard.
3. **Check Power and Hardware**
   * Verify if there’s an electric outage in the head office affecting the gateway.
   * If no power issue, ensure the gateway (e.g., Fiber, VDSL router, 4G router) is powered on and cables are securely connected.
4. **Verify Bill Payments**
   * Check if the landline and internet bills for the head office are paid and there are no billing issues.
   * Coordinate with ISP (e.g., the ISP) to confirm payment status.
5. **Restart the Gateway**
   * IT staff in the head office (or remotely by the IT team) should restart the affected gateway:
     * Unplug the gateway (e.g., Fiber, VDSL router, 4G router), wait 30 seconds, then plug it back in.
   * Monitor Splunk to see if connectivity is restored.
6. **Contact ISP if Unresolved**
   * If the gateway remains down.
   * Contact the ISP (e.g., the ISP), submit a formal complaint, and obtain a complaint number.
   * Follow up with the ISP using the complaint number until resolved.
7. **Monitor Post-Action**
   * After resolution, confirm the gateway is back online via Splunk.

{% hint style="info" %}
Gateway outages can disrupt branch operations; act quickly. Ensure only IT staff handle router restarts to avoid errors.
{% endhint %}
