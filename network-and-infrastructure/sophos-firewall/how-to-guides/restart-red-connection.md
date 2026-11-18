---
description: >-
  This guide explains how to restart a RED (Remote Ethernet Device) connection
  in the Sophos Firewall web admin console to troubleshoot connectivity issues.
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

# Restart RED Connection

### Prerequisites

* Access to the Sophos Firewall web admin console.
* Sophos Firewall admin credentials.
* A web browser (e.g., Chrome, Firefox).
* Knowledge of the RED interface to restart (e.g., Branch C).

### Steps

1. **Log in to the Sophos Firewall Web Admin Console**:
   * Open a web browser and navigate to the Sophos Firewall IP address (retrieve the IP from Keeper Security).
   * Log in using the administrative credentials provided by the IT admin.
2. **Navigate to Interfaces**:
   * From the left sidebar, click **NETWORK** to expand the menu.
   * Select **Interfaces** to view the list of interfaces.
3. **Locate the RED Interface**:
   * In the interfaces list, find the RED interface you want to restart (e.g., Branch C with type "Firewall RED Server").
   * Ensure the interface is marked as **RED** in the list.
4.  **Restart the RED Connection**:

    * Click the three-dot menu icon next to the RED interface (e.g., Branch C).
    * Toggle the **Status** switch to **Disabled** to turn off the interface.
    * Click **Save** to apply the changes.
    * Wait for a few seconds, then toggle the **Status** switch back to **Enabled**.


{% hint style="info" %}
Restarting the RED connection may temporarily disrupt network access for devices using that interface. Monitor the interface status after restarting to ensure it reconnects successfully (e.g., Uplink IP should reappear, such as 203.0.113.10 for Branch C). If the connection does not restore, escalate to the IT admin.
{% endhint %}
