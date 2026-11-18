---
description: >-
  Instructions for performing a factory reset on a Grandstream GRP2612P IP phone
  to resolve issues or reconfigure.
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

# Reset Factory

### Prerequisites

* A Grandstream IP phone with access to the web interface.
* Administrative privileges (e.g., default login: admin/admin).

### Steps

1. **Access the Web Interface**:
   * Identify the phone’s IP address from the display (e.g., 172.20.21.x).
   * Open a browser and enter the IP address.
   * Log in with default credentials (e.g., username: admin, password: admin).
2.  **Navigate to Factory Reset**:

    * Click the "Maintenance" tab (1).
    * Select "Tools" from the left menu (2).
    * Click "Factory Reset" (3).

    <figure><img src="../../../../../.gitbook/assets/image (203).png" alt=""><figcaption></figcaption></figure>
3. **Perform Reset**:
   * Click the "Start" button next to "Factory Reset" (3).
   * Confirm the reset when prompted.
   * The phone will reboot and reset to factory settings.
4. **Reconfigure**:
   * After reset, the phone will lose all settings.
   * Follow Power On and Configure Settings to set up again.

{% hint style="info" %}
A factory reset erases all configurations, including SIP settings. Ensure you have SIP credentials and network details before proceeding. Contact your IT admin for reconfiguration assistance.
{% endhint %}
