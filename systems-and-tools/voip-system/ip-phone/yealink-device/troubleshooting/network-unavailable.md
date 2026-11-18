---
description: >-
  Instructions for troubleshooting the "Network Unavailable" issue on a Yealink
  IP phone, which occurs when the phone cannot detect a network connection.
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

# Network Unavailable

### Prerequisites

* A Yealink IP phone displaying "Network Unavailable" on the screen.
* Access to the phone’s physical connections and network switch.
* Administrative privileges or assistance from your IT admin.
* Network setup on VLAN 21 (IP range: 172.20.21.0/24) for the head office.

### Possible Causes and Solutions

The "Network Unavailable" issue is typically caused by physical connection problems or switch configuration errors. Follow these steps to resolve:

<div align="left"><figure><img src="../../../../../.gitbook/assets/image (114).png" alt="" width="375"><figcaption></figcaption></figure></div>

#### Solution: Check Cable Connections and Functionality

* **Description**: The issue may arise if the cables are not connected properly, damaged, or the internet port is not functioning.
* **Steps**:
  1. Verify that the Ethernet cable is securely plugged into both the internet port and the PC port on the Yealink phone.
  2. Ensure the cable is in good condition (e.g., no cuts or bends that could affect connectivity).
  3. Confirm that the internet port is operational by checking for link lights on the phone and the switch.
  4. Ensure the port is connected to the correct switch and has not been disabled on the switch configuration.
* **Verification**: After correcting the connections, check if the phone’s display updates to a registered status or shows an IP address.

{% hint style="info" %}
If the port is disabled on the switch, contact your IT admin to enable it. Ensure the switch is configured for VLAN 21 and that the cable meets network standards (e.g., Cat5e or higher). If the issue persists, replace the cable and retest.
{% endhint %}
