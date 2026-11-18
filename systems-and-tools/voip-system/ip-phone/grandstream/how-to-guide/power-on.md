---
description: Instructions for powering on a Grandstream IP phone to initiate setup.
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

# Power On

### Prerequisites

* A Grandstream IP phone.
* A power adapter (for non-PoE models) or a PoE switch (for PoE models).
* Two Ethernet cables.

### Steps

<div align="left"><figure><img src="../../../../../.gitbook/assets/image (110).png" alt="" width="563"><figcaption></figcaption></figure></div>

1. **Connect the Ethernet cables**:
   * Plug one end of the Ethernet cable into the "Internet" port on the Grandstream Phone.
   * Connect the other end to a network port.
   * Plug the second Ethernet cable into the "PC" port on the IP Phone.
   * Connect the other end to the PC Ethernet port.
2.  **Power On**:

    * The phone will automatically power on once connected to power (via PoE or adapter).
    * Wait for the phone to boot up; the display will show the Grandstream logo, and then attempt to obtain an IP address.
    * **Verify Boot**:
      * Confirm the phone displays an IP address (e.g., 172.20.21.x) or a registration status.
      * If "No Service" or "Obtaining IP Address" appears, refer to Registration Failure.

{% hint style="info" %}
Ensure the switch port is active. If using a power adapter, verify it matches the phone’s voltage requirements (e.g., 5V DC). Contact your IT admin if the phone fails to boot.
{% endhint %}
