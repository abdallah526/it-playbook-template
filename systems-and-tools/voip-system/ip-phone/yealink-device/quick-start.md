---
description: >-
  An overview to help you get started with the Yealink IP phones, highlighting
  its key features and guiding you to detailed instructions for setup and
  management.
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

# Quick Start

### Overview

The Yealink IP Phone is an enterprise-grade IP phone designed for efficient communication in business environments. It supports Power over Ethernet (PoE) in some models, VLAN configurations, and hotdesking for flexible user access. In the head office, these phones are configured on VLAN 21 (IP range: 172.20.21.0/24) and integrated with SIP servers for VoIP functionality. This section provides guidance on powering on, configuring settings, adjusting time, logging in, resetting the device, enabling dual headset support for shadowing, etc.

### Key Features

* **Power Options**: Supports PoE or a power adapter depending on the model.
* **Network Configuration**: Operates on VLAN 21 with DHCP for IP assignment.
* **SIP Integration**: Connects to SIP servers for VoIP calls (e.g., 172.20.31.10:5060).
* **Hotdesking**: Allows flexible user login via the Message button.
* **Dual Headset Support**: Enables simultaneous use of two headsets for shadowing.
* **Time Synchronization**: Uses NTP servers for accurate date and time.

### Next Steps

* Refer to [Power On](how-to-guide/power-on.md) to get the device started.
* Explore How-To Guides for detailed instructions on tasks like configuring settings, adjusting date and time, or enabling dual headset support.
* For advanced configurations, ensure your network is set up for VLAN 21 (IP range: 172.20.21.0/24) and the SIP server is accessible.

{% hint style="info" %}
Verify VLAN 21 configuration on your switch and ensure the SIP server is reachable. Visit Yealink’s support page (`https://support.yealink.com`) for firmware updates or additional resources.
{% endhint %}
