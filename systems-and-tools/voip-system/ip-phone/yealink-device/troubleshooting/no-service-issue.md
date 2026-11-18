---
description: Instructions for troubleshooting the "No Service" issue on a Yealink IP phone.
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

# No Service Issue

### Prerequisites

* A Yealink IP phone displaying "No Service" on the screen.
* Access to the phone’s interface (via hotdesking or web interface).
* Administrative privileges or assistance from your IT admin.
* Network connectivity to VLAN 21 (IP range: 172.20.21.0/24) for the head office.
* SIP server details (e.g., 172.20.31.10:5060) provided by your IT admin.

### Possible Causes and Solutions

<div align="left"><figure><img src="../../../../../.gitbook/assets/yealink-auto-provisioning-6 (1).png" alt=""><figcaption></figcaption></figure></div>

The "No Service" issue typically arises due to one of the following problems. Follow the corresponding steps to resolve:

#### Cause 1: Incorrect Extension Password

* **Description**: The user may have entered the wrong password when logging into the extension via hotdesking.
* **Solution**:
  1. Log out of the current session by pressing the "Message" button and selecting "Clear all accounts"
  2. Re-enter the correct credentials using the hotdesking process.
  3. Refer to [Login to Extension](../how-to-guide/configure-settings.md) under How To Guide for detailed steps to log in correctly.
  4. Verify the phone displays the extension (e.g., "692") and updates to "Registered" status.

#### Cause 2: Unable to Connect to PBX Server

* **Description**: The phone cannot reach the PBX server, possibly due to network issues or the server being offline.
* **Solution**:
  1. Check the network connection by ensuring the phone is on VLAN 21 (IP range: 172.20.21.0/24).
  2. Ping the PBX server (e.g., 172.20.31.10) from another device to confirm connectivity.
  3. If the server is unreachable, contact your IT admin to verify the server status.

#### Cause 3: Misconfigured Server Address

* **Description**: The SIP server address entered in the phone settings may be incorrect or outdated.
* **Solution**:
  1. Access the phone’s web interface using its IP address (see [Login for instructions](../how-to-guide/configure-settings.md)).
  2. Navigate to the "Account" or "SIP" settings and verify the server address (e.g., 172.20.31.10:5060).
  3. Correct the server address if necessary and save the changes.
  4. Refer to [Configure Settings](../how-to-guide/configure-settings.md) under How To Guide for detailed configuration steps.
  5. Restart the phone and check if the "No Service" issue is resolved.

### Verification

* After applying the solution, check the phone’s display to ensure the status changes from "No Service" to "Extension Number or Name."
* Test a call using the extension to confirm functionality.

{% hint style="info" %}
If the issue persists after trying the above solutions, reset the phone to factory settings (see [Reset Factory](../how-to-guide/reset-factory.md) under How To Guide) and reconfigure it. Ensure the PBX server is operational and the network switch is configured for VLAN 21. Contact your IT admin for further assistance if needed.
{% endhint %}
