---
description: >-
  This guide outlines the steps to handle an electric outage at a branch,
  covering scenarios in Branch A, other branches, and head office.
icon: plug-circle-xmark
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

# Electric Outage at a Branch

### Steps

1. **Branch A Outage**
   * If power is out in Branch A, server racks will stay operational via the UPS.
   * Monitor UPS runtime and wait for power restoration.
2. **other branches Outage**
   * For other branches, there’s no immediate solution; wait for power to return.
3. **Head Office Outage**
   * Identify the outage via employee reports from the head office or Splunk alerts/dashboard.
   * Handle based on the scenario:
     * **Full Company Outage**:
       * All critical devices will run on the UPS units.
       * Instruct employees to shut down non-essential devices to extend UPS runtime.
     * **Partial Outage (One Floor/Side)**:
       * From the electrical panel in the server room, lower the breaker for the affected floor or section completely.
       * This shifts the load to the working power source.


{% hint style="info" %}
Monitor UPS levels closely during outages. Document outage details and UPS performance in the team documentation for future improvements. Ensure employees know how to power down non-critical devices safely.
{% endhint %}
