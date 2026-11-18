---
description: >-
  This guide outlines the steps to set up a PC for remote work, including
  installing MicroSIP, configuring a VPN (Sophos Connect or OpenVPN), and
  ensuring PBX login access.
icon: house-signal
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

# Configure PC for Work From Home

### Steps

1. **Install and Configure MicroSIP**
   * Download and install MicroSIP, then configure it with SIP details from your PBX to enable VoIP calls.
   * See [MicroSIP Configuration Details](../systems-and-tools/voip-system/softphones/microsip/).
2. **Install and Configure Remote Access VPN**
   * Set up a VPN using Sophos Connect or OpenVPN to securely access the company network.
   * [Sophos Connect VPN Setup](../network-and-infrastructure/remote-access-vpn/access-vpn-portal-and-download-client.md).
3. **Ensure User Can Login to the Call Center**
   * Verify the user can log in to the call center using their credentials for unified communications access.
   * [Queue Login](../systems-and-tools/voip-system/pbx-server/how-to-guides/login-to-queue.md).

{% hint style="info" %}
Ensure the PC has a stable internet connection. Test MicroSIP and VPN connectivity before proceeding to the call center login. Contact IT Admin if issues arise.
{% endhint %}
