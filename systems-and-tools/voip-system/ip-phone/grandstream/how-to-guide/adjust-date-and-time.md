---
description: >-
  Instructions for setting the correct date and time on a Grandstream GRP2612P
  IP phone using the web interface.
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

# Adjust Date & Time

### Prerequisites

* A powered-on Grandstream IP phone with network access.
* Access to the phone’s web interface (default login: admin/admin).

### Steps

1. **Access the Web Interface**:
   * Identify the phone’s IP address from the display (e.g., 172.20.21.x).
   * Open a browser and enter the IP address (e.g., http://172.20.21.x).
   * Log in with the credentials (e.g., username: admin, password: admin).
2.  **Navigate to Date and Time Settings**:

    * Click on the "Settings" tab.
    * In the left menu, click "Date and Time."

    <figure><img src="../../../../../.gitbook/assets/image (111).png" alt=""><figcaption></figcaption></figure>
3. **Configure Date and Time**:
   * **NTP Server**: Enter "pool.ntp.org" in the NTP Server field (4).
   * **Time Zone**: Select the site's time zone.
   * **Time Display Format**: Select "12 Hour."
   * **Show Date on Status Bar**: Check "Yes" if desired.
4. **Save and Apply**:
   * Click "Save and Apply" to apply the settings.
   * The phone will update the date and time automatically via NTP.
5. **Verify**:
   * Check the phone’s display to confirm the date and time are correct .
   * If incorrect, ensure the NTP server is reachable.

{% hint style="info" %}
If NTP fails, verify network connectivity to "pool.ntp.org" or use a company NTP server (e.g., 172.20.31.250). Contact your IT admin for issues.
{% endhint %}
