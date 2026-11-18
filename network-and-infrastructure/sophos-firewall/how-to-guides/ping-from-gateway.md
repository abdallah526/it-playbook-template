---
description: >-
  This guide explains how to perform a ping test from a specific gateway in the
  Sophos Firewall web admin console to troubleshoot network connectivity.
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

# Ping From Gateway

### Prerequisites

* Access to the Sophos Firewall web admin console.
* Sophos Firewall admin credentials.
* A web browser (e.g., Chrome, Firefox).
* The IP address or hostname to ping (e.g., 8.8.8.8 for Google DNS).
* Knowledge of the gateway interface to use (e.g., ISP-1).

### Steps

1. **Log in to the Sophos Firewall Web Admin Console**:
   * Open a web browser and navigate to the Sophos Firewall IP address (retrieve the IP from Keeper Security).
   * Log in using the administrative credentials provided by the IT admin.
2. **Navigate to Diagnostics**:
   * From the left sidebar, click **DIAGNOSTICS** to expand the menu.
   * Select **Tools** to access diagnostic tools.
3.  **Perform a Ping Test**:

    * In the **Ping** section, enter the **IP address/hostname** to ping (e.g., 8.8.8.8 for Google DNS).
    * In the **Interface** dropdown, select the gateway interface (e.g., ISP-1).
    * Leave the **IP version** as **IPv4** (or select **IPv6** if applicable).
    * Leave the **Size** field at its default value (e.g., 1-65507).
    * Click **Ping** to initiate the test.

    <figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>
4.  **Review the Ping Results**:

    * A pop-up window will display the ping results.
    * Check for successful responses (e.g., "64 bytes from 8.8.8.8: seq=1 ttl=117 time=43.753 ms").
    * Note the packet loss percentage (e.g., 25% packet loss) and round-trip times (e.g., min/avg/max = 42.813/43.230/43.753 ms).
    * Click **OK** to close the results window.

    <figure><img src="../../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
If the ping test shows packet loss (e.g., 25%) or no response, verify the gateway’s connectivity (e.g., ISP-1) and escalate to the IT admin if needed. Ensure the target IP (e.g., 8.8.8.8) is reachable.
{% endhint %}

