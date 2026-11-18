---
description: >-
  This page explains the DC1 Server CPU Usage is High Alert on the Splunk
  dashboard, its impact, and the steps to resolve it.
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

# Server CPU Load

### Overview

* **Purpose**: To address high CPU usage on the DC1 server, which can lead to performance degradation or system failure.
* **Trigger**: Activates when CPU usage exceeds the error limit (e.g., 78% total usage, above 75%).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the high CPU usage alert for oversight and guidance.
2. **Identify the Cause**
   * Use the inventory or monitoring tool to check which processes or services are consuming high CPU on the DC1 server.
   * [Device Inventory](../../device-inventory/using-the-inventory-tool.md)
3. **Access the Server**
   * Connect to the DC1 server via TeamViewer or direct access to investigate.
4. **Analyze and Mitigate**
   * Open Task Manager or Resource Monitor on the DC1 server to identify high-CPU processes (e.g., specific applications, and services).
   * If non-critical, stop or restart the process/service.
   * If critical, optimize the process or allocate more resources (e.g., increase CPU allocation in ESXi if virtualized).
5. **Monitor Post-Action**
   * After mitigation, monitor CPU usage via Task Manager to ensure it drops below the error limit (75%).

{% hint style="info" %}
High CPU usage can indicate resource bottlenecks or misconfigurations. If the issue persists, consider upgrading server resources or redistributing workloads.
{% endhint %}
