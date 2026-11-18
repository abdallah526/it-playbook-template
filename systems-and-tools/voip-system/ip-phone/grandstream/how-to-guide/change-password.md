---
description: >-
  Instructions for changing the admin password on a Grandstream IP phone. This
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

* A powered-on Grandstream IP phone with network access.
* Access to the phone’s web interface.
* The phone has undergone a factory reset (see [Reset Factory](reset-factory.md)) or is a new device.
* Current admin credentials (default: admin/admin).

### Steps

1. **Access the Web Interface**:
   * Identify the phone’s IP address from the display (e.g., 172.20.21.x ).
   * Open a browser and enter the IP address (e.g., http://172.20.21.x).
   * Log in with the default admin credentials (username: admin, password: admin).
2. **Navigate to Web Access Settings**:
   * Click on the "Maintenance" tab at the top.
   * In the left menu, click "Web Access".
3. **Change the Admin Password**:
   *   Under "Admin Password", enter the following:

       * **Current Password**: Input the current admin password (default: admin).
       * **New Password**: Enter the fixed password designated for your branch (head office or branches) as provided by your IT admin.
       * **Confirm Password**: Re-enter the fixed password to confirm.

       <figure><img src="../../../../../.gitbook/assets/image (206).png" alt=""><figcaption></figcaption></figure>
4. **Save Changes**:
   * Click the "Save" button to apply the new password.
   * The web interface may log you out; log back in with the new password to verify.
5. **Verify**:
   * Log out and log back into the web interface using the new fixed password.
   * If login fails, ensure the password was entered correctly or contact your IT admin.

{% hint style="info" %}
Use the fixed password designated for the branch: one for the head office and a different one for the branches. Store the passwords securely (e.g., in Keeper Security). If the password is forgotten, a factory reset will be required, and the phone must be reconfigured, including SIP settings for the PBX server (172.20.31.10:5060). Ensure the phone remains on the correct VLAN (e.g., VLAN 21 for head office). Contact your IT admin if unsure about the branch-specific password.
{% endhint %}
