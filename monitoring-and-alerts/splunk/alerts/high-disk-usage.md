---
description: >-
  This page explains the High Disk Usage Server alert on the Splunk dashboard,
  its impact, and the steps to resolve low disk space on servers like DC1 (Drive
  E:).
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

# High Disk Usage

### Overview

* **Purpose**: To address low disk space on a server, which can cause performance issues or system failures.
* **Trigger**: Activates when free disk space falls below the warning limit (e.g., 24% free space on Drive E: of DC1, below 25%).


### Steps to Resolve

1. **Notify IT Admin or IT Manager**
   * Immediately inform the IT Admin or IT Manager about the high disk usage alert for oversight and guidance.
2. **Verify Disk Space**
   * Confirm the alert on the Splunk dashboard, noting the affected server and drive (e.g., DC1, Drive E:).
3. **Access the Server**
   * Connect to the affected server (e.g., DC1) via TeamViewer or direct access to investigate.
4. **Analyze Disk Usage**
   * On the server, open File Explorer and navigate to the affected drive (e.g., Drive E:).
   * Use tools like Disk Cleanup or TreeSize to identify large files, logs, or unnecessary data consuming space.
5. **Free Up Space**
   * Delete or move non-critical files (e.g., old logs, temporary files) to another drive or external storage.
   * If critical data, consider archiving or expanding storage capacity.
6. **Monitor Post-Action**
   * After freeing up space, monitor the disk usage via Splunk to ensure free space is above the warning limit (25%).

{% hint style="info" %}
Low disk space can lead to system crashes; address it promptly. If the issue recurs, plan for additional storage or better data management policies.
{% endhint %}
