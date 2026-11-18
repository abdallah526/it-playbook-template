---
description: >-
  Instructions for troubleshooting the "Obtaining IP Address" issue on a Yealink
  IP phone, which occurs when the phone fails to acquire an IP address.
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

# Obtaining IP Address

### Prerequisites

* A Yealink IP phone stuck on "Obtaining IP Address" on the screen.
* Access to the phone’s physical connections and network switch.
* Administrative privileges or assistance from your IT admin.
* Network setup on VLAN 21 (IP range: 172.20.21.0/24) for the head office.
* Another device (e.g., a laptop) for testing DHCP.

### Possible Causes and Solutions

<div align="left"><figure><img src="../../../../../.gitbook/assets/image (115).png" alt="" width="375"><figcaption></figcaption></figure></div>

The "Obtaining IP Address" issue is typically caused by cable problems, DHCP failures, port security issues, or incorrect VLAN configuration. Follow these steps to resolve:

#### Solution 1: Check Cable and DHCP Functionality

* **Description**: The cable may be faulty, or the DHCP server may not be responding.
* **Steps**:
  1. Verify that the Ethernet cable is securely connected and in good condition.
  2. Connect another device (e.g., a laptop) to the same cable and check if it obtains an IP address.
  3. If the other device fails to get an IP, confirm that the DHCP server is operational.
* **Verification**: If the alternate device gets an IP, reconnect the phone and check if it obtains an address (e.g., 172.20.21.x).

#### Solution 2: Check Port Security and Device Movement

* **Description**: Port security may block the DHCP request if the phone has been moved to a different switch port.
* **Steps**:
  1. If DHCP fails, check with your IT admin if port security is enabled and blocking the phone.
  2. If the phone was recently moved, this could trigger a security block due to MAC address changes.
  3. Contact your IT admin to resolve the port security issue and allow the phone’s MAC address.
* **Verification**: After IT admin intervention, confirm the phone obtains an IP address.

#### Solution 3: Verify VLAN Configuration

* **Description**: The IP phone VLAN may not be set to 21, or the PC VLAN may be enabled incorrectly.
* **Steps**:
  1. Access the phone’s web interface (see [Login under How-To Guides for instructions](../how-to-guide/configure-settings.md)).
  2. Navigate to the "Network" settings and verify that the VLAN ID is set to 21 for the phone.
  3. Ensure the PC port VLAN is disabled to avoid conflicts.
  4. Save the settings and restart the phone.
* **Verification**: Check if the phone displays an IP address within the 172.20.21.0/24 range.

{% hint style="info" %}
For port security or VLAN problems, coordinate with your IT admin to update switch settings. If necessary, perform a factory reset (see [Reset Factory under How-To Guides](../how-to-guide/reset-factory.md)) and reconfigure.
{% endhint %}
