---
description: >-
  Instructions for troubleshooting a registration failure on a Grandstream
  GRP2612P IP phone, indicated by a "NO" status in Account Status.
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

# Registration Failure

### Prerequisites

* A Grandstream IP phone displaying "NO" under SIP Registration.
* Access to the phone’s web interface (default login: admin/admin).
* SIP account details (e.g., username "918", password, server 172.20.31.10:5060).

### Possible Causes and Solutions

The "NO" status indicates the phone is not registered with the PBX server. Follow these steps:

#### Cause 1: Incorrect SIP Settings

* See [Login to Extension](../how-to-guide/login-to-extension.md) to configure the correct settings.

#### Cause 2: Network Issue

* **Description**: Connectivity problem to the PBX server.
*   **Solution**:

    1. Click the "Network" tab and select "Basic Settings."
    2. Ensure "IPv4 Address" is set to DHCP.
    3. Ping 172.20.31.10 from another device to test connectivity.

    <figure><img src="../../../../../.gitbook/assets/image (201).png" alt=""><figcaption></figcaption></figure>

#### Cause 3: PBX Server Issue

* **Description**: The PBX server may be offline.
* **Solution**:
  1. Ping the PBX server.
  2. Contact your IT admin to verify the PBX server status.
  3. Wait for restoration and recheck registration.

### Verification

* Refresh "Account Status" to confirm "YES" under SIP Registration.
* Test a call to verify functionality.

{% hint style="info" %}
If unresolved, perform a factory reset (see Reset Factory) and reconfigure. Contact your IT admin for SIP credentials or server issues.
{% endhint %}
