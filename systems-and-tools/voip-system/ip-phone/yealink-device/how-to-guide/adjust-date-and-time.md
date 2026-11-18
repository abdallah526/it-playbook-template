---
description: >-
  Instructions for adjusting the date and time settings on a Yealink IP phone to
  ensure accurate time display.
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

* A powered-on Yealink IP phone.
* Admin credentials (default: username "admin", password "admin").
* Access to the phone’s web interface via its IP address.
* NTP server details (e.g., "dc1.company.local").

### Steps

1. **Access the Web Interface**:
   * Refer to Login to access the IP Phone web interface using its IP address.
2. **Navigate to Time & Date Settings**:
   * Go to the "Settings" tab and select "Time\&Date" from the left menu.
3. **Configure Time Settings**:
   * Set "DHCP Time" to "Disabled."
   * Set "Manual Time" to "Disabled."
   * Select "Time Zone" (the site's time zone).
   * Enable "Daylight Saving Time" to "Automatic."
   * Set "Location" to your city.
4. **Configure NTP Server**:
   * Set "NTP by DHCP Priority" to "High."
   * Enter "Primary Server" as "dc1.company.local."
   * Enter "Secondary Server" as "172.20.31.250."
   * Set "Update Interval" to "1000" seconds.
5. **Save Changes**:
   * Set "Time Format" to "12-Hour" and "Date Format" to "WWW MMM DD."
   * Click "Confirm" to save.

{% hint style="info" %}
If the time doesn’t sync, verify the NTP server’s accessibility and network connectivity. Ensure VLAN 21 allows NTP traffic
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>
