---
description: >-
  This page explains the Server RAM Usage alert on the Splunk dashboard for the
  servers, its impact, and the steps to resolve high RAM usage.
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

# Server RAM Usage

### Overview

* **Purpose**: To address excessive RAM usage on the servers like WDS-WSUS, which can lead to performance issues or system slowdowns.
* **Trigger**: Activates when available memory falls below the warning limit (e.g., 12% available memory on WDS-WSUS, below 15%).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the high RAM usage alert for oversight and guidance.
2. **Verify RAM Usage**
   * Confirm the alert on the Splunk dashboard, noting the affected server (e.g., WDS-WSUS, 12% available memory).
3. **Access the Server**
   * Connect to the WDS-WSUS server via TeamViewer or direct access to investigate.
4. **Analyze RAM Usage**
   * Open Task Manager or Resource Monitor on the WDS-WSUS server to identify processes consuming high RAM (e.g., WSUS services, updates, or other applications).
   * Check for memory leaks or unnecessary processes.
5. **Mitigate High Usage**
   * Stop or restart non-critical processes consuming excessive RAM (e.g., pause WSUS sync if active).
   * If critical, optimize the process (e.g., adjust WSUS settings) or allocate more RAM in ESXi if the server is virtualized.
6.  **Monitor Post-Action**

    * After mitigation, monitor RAM usage via Splunk to ensure available memory rises above the warning limit (15%).



{% hint style="info" %}
High RAM usage can slow down critical services like WSUS; address promptly. If the issue persists, consider upgrading RAM or optimizing server workloads.
{% endhint %}
