---
description: >-
  How to open the inventory tool (PDQ Inventory in this example), filter devices
  and export reports.
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

# Using the Inventory Tool

### Overview

* **Purpose**: The inventory tool scans Windows devices and keeps their hardware and software details, so you can filter and report on them.
* **Location**: Write where the tool is installed (for example, a management VM) and how the team reaches it.

### Steps

1.  **Open the inventory tool**

    * Connect to the machine where the tool is installed (for example, through your remote support tool).
    * Open PDQ Inventory from the desktop or the Start menu.

    <div align="left"><figure><img src="../../.gitbook/assets/image (282).png" alt="" width="563"><figcaption></figcaption></figure></div>
2.  **Browse devices**

    * In the left sidebar, under **All Computers**, open the collections you need, for example by RAM size, Windows version or CPU generation.

    <div align="left"><figure><img src="../../.gitbook/assets/image (283).png" alt=""><figcaption></figcaption></figure></div>
3.  **Apply filters and view devices**

    * Click a collection (e.g., **RAM 16 GB**) to list the matching devices.
    * Useful columns:
      * **Name**: Device name (e.g., PC036).
      * **Online**: Status (e.g., Online, N/A).
      * **Memory**: Total RAM (e.g., 16 GB).
      * **Model**: Device model (e.g., OptiPlex 3050).
      * **Serial Number**: The vendor serial or service tag.
      * **OS**: Operating system (e.g., Windows 11).
    * If a device shows "The network path was not found", it is probably offline; check its connection.
4.  **Generate reports**

    * In the toolbar, click **New Report**.
    * Pick the fields to include (e.g., OS, Memory, Model).
    * Click **Run Report**, then export it as CSV or PDF from **File** > **Export**.

{% hint style="info" %}
Make sure the machine that runs the inventory tool is powered on. Use collections to find devices that need updates or upgrades (e.g., low RAM), and keep exported reports in the team documentation.
{% endhint %}
