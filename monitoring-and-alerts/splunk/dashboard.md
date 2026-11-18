---
description: >-
  This guide explains the key components of the Splunk dashboard used for
  monitoring IT operations across branches, including head office and Branch A.
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

# Dashboard


### Dashboard Components

1. **Head Office Gateway (Fiber & VDSL Router)**
   * Displays latency (e.g., 34 ms, 38 ms) and current bandwidth usage (e.g., 19 Mbit/s down, 2.98 Mbit/s up) for Fiber and VDSL routers.
2. **Remote Access VPN Users**
   * Shows current VPN live users (e.g., jsmith), failed logins (e.g., 0), and successful logins (e.g., 6).
3. **Malware and IPS (Sophos - head office)**
   * Tracks malware events and IPS events in head office.
4. **PBX Downtime (head office to Branch A)**
   * Monitors PBX disconnects (e.g., 0), daily downtime (e.g., 00:00:00), and weekly downtime (e.g., 00:00:21).
5. **Domain User Failed Logins**
   * Displays failed login attempts on domain users (e.g., 18 failed logins).
6. **Live Bandwidth Monitor (head office Employees)**
   * Tracks bandwidth usage per employee in head office (e.g., 0.38 mb/s down, 32.52 mb/s up for an employee).
7. **Switch Logins (head office)**
   * Shows failed (e.g., 0) and successful (e.g., 19) logins on switches in head office.
8. **UPS Data (head office)**
   * Monitors UPS status: runtime (e.g., 10h 49m for Floor 1), load (e.g., 11.2 A), capacity (e.g., 25%), voltage (e.g., 230 V AC), and temperature (e.g., 28°C).
9. **Red Connection Status (Between Branches)**
   * Displays latency (e.g., 101 ms for Branch C) and online device count (e.g., 2/4 in Branch D) across branches.
10. **Online Users and Devices (head office)**
    * Shows total online users (e.g., 73) and devices (e.g., 102) in head office.

{% hint style="info" %}
Use this dashboard to quickly identify issues (e.g., high latency, failed logins). Cross-check with PRTG for deeper network insights.
{% endhint %}
