---
description: >-
  An overview to help you get started with softphones on various platforms,
  guiding you to detailed instructions for setup and configuration.
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

Softphones are software-based phone applications that allow users to make and receive VoIP calls using devices like Windows PCs, Android phones, iPhones, and macOS systems. This section provides guidance on configuring softphones for platforms like MicroSIP (Windows), SessionTalk SIP Softphone (iPhone), and others, integrating with your VoIP system (e.g., PBX, FreePBX, 3CX). Softphones can be used both inside and outside the company network, with OpenVPN required for external access.

### Key Features

* **Cross-Platform Support**: Configure softphones on Windows, Android, iPhone, and macOS.
* **SIP Integration**: Connect to SIP servers (e.g., 172.20.31.10:5060) for VoIP calls.
* **External Access**: Use OpenVPN with a VPN file for secure access outside the company network.
* **User-Friendly Setup**: Easy configuration with SIP account details provided by your IT admin.

### Next Steps

* Choose your platform (Windows - MicroSIP, Android, iPhone, or macOS) to configure the softphone.
* For iPhone users, start with iPhone to set up the SessionTalk SIP Softphone.
* Ensure OpenVPN is configured if working outside the company network (see the note below).

{% hint style="info" %}
For external access, employees must use OpenVPN with the provided VPN file to connect to the company network (e.g., VLAN 21 for head office). Contact your IT admin for the VPN file and setup instructions.
{% endhint %}
