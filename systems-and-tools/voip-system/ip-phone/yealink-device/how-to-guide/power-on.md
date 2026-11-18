---
description: >-
  Instructions for powering on a Yealink IP phone, with considerations for Power
  over Ethernet (PoE) support.
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

* A Yealink IP phone.
* A power adapter (for non-PoE models) or a PoE switch (for PoE models).
* Two Ethernet cables.
* Access to a network with VLAN 21 (IP range: 172.20.21.0/24) for the head office.

### Steps

1. **Connect the Ethernet cables**:
   * Plug one end of the Ethernet cable into the "Internet" port on the Yealink Phone.
   * Connect the other end to a network port on VLAN 21 (IP range: 172.20.21.0/24).
   * Plug the second Ethernet cable into the "PC" port on the Yealink IP Phone.
   * Connect the other end to the PC Ethernet port.
2. **Power the device**:
   * For PoE-supported models:
     * Ensure the switch provides Power over Ethernet (PoE). The phone will power on automatically.
   * For non-PoE models:
     * Connect the power adapter to the Yealink and plug it into a power outlet.
3.  **Verify Power**:

    * Check the phone’s display for activity (e.g., the Yealink logo or initialization screen).
    * Ensure the status LED on the phone lights up (typically green).

    <figure><img src="../../../../../.gitbook/assets/image (126).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
If the phone does not power on, verify the Ethernet connection or power adapter. For PoE issues, confirm the switch supports PoE and is configured for VLAN 21.
{% endhint %}
