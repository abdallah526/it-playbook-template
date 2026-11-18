---
description: >-
  Instructions for removing a Windows PC from an Active Directory domain to
  revert it to a workgroup.
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

# Remove a PC from the Domain

### Prerequisites

* Administrative privileges on the PC.
* The PC must be connected to the network with access to the domain controller (optional for removal).
* Knowledge of the local administrator account credentials for post-removal login.
* The PC must currently be joined to the domain (e.g., company.local).

### Steps

1.  **Open the System Control Panel**:

    * On the PC, press `Windows + R` to open the Run dialog.
    * Type `sysdm.cpl` and press Enter to open the System Properties window.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure></div>
2.  **Access Computer Name Settings**:

    * In the System Properties window, go to the "Computer Name" tab.
    * Click the "Change..." button to modify the computer name and domain settings.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (95).png" alt=""><figcaption></figcaption></figure></div>
3.  **Change Membership to Workgroup**:

    * In the "Computer Name/Domain Changes" window, under "Member of," select "Workgroup".
    * Enter `WORKGROUP` as the workgroup name.
    * Click "OK" to proceed.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure></div>
4.  **Acknowledge BitLocker Warning**:

    * A warning will appear: "Before you leave the domain, you should do two things: Make sure you know the password for the local administrator account, or you won’t be able to sign in. Make sure you have a copy of your BitLocker recovery key saved somewhere other than this PC."
    * Click "OK" to continue (1).
    * Ensure you have the local administrator password and BitLocker recovery key saved before proceeding.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
After removal, the PC will no longer be managed by Active Directory policies. Log in using the local administrator account after restarting the PC. If BitLocker is enabled, ensure the recovery key is accessible to avoid data loss. Verify the PC’s removal from Active Directory by checking the appropriate OU (e.g., Company/HQ/Quality).
{% endhint %}
