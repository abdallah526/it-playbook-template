---
description: >-
  Instructions for changing the admin password on a Yealink IP phone. This
  process is typically performed after a factory reset or on a new device to
  replace the default password.
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

# Change Password

### Prerequisites

* A powered-on Yealink IP phone with network access.
* Access to the phone’s web interface.
* The phone has undergone a factory reset (see [Reset Factory](reset-factory.md)) or is a new device.
* Current admin credentials (default: admin/admin).
* Network connectivity to VLAN 21 (IP range: 172.20.21.0/24 for head office).

### Steps

1. **Access the Web Interface**:
   * Identify the phone’s IP address from the display (e.g., 172.20.21.x for head office).
   * Open a browser and enter the IP address (e.g., http://172.20.21.x).
   * Log in with the default admin credentials (username: admin, password: admin).
2. **Navigate to Password Settings**:
   * Click on the "Security" tab at the top (1).
   * In the left menu, click "Password" (2).
3.  **Change the Password**:

    * **User Type**: Ensure "admin" is selected from the dropdown (3).
    * **Old Password**: Enter the current admin password (default: admin) (3).
    * **New Password**: Enter the fixed password designated for your branch (head office or branches) as provided by your IT admin (3).
    * **Confirm Password**: Re-enter the fixed password to confirm (3).

    <figure><img src="../../../../../.gitbook/assets/image (207).png" alt=""><figcaption></figcaption></figure>
4. **Save Changes**:
   * Click the "Confirm" button to save the new password (4).
   * The web interface may log you out; log back in with the new password to verify.
5. **Verify**:
   * Log out and log back into the web interface using the new fixed password.
   * If login fails, ensure the password was entered correctly or contact your IT admin.

{% hint style="info" %}
Use the fixed password designated for the branch: one for the head office and a different one for the branches. Store the passwords securely (e.g., in Keeper Security). If the password is forgotten, a factory reset will be required, and the phone must be reconfigured, ensuring it remains on the correct VLAN (e.g., VLAN 21 for head office). Contact your IT admin if unsure about the branch-specific password.
{% endhint %}
