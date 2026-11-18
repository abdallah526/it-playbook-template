---
description: >-
  Instructions for joining a Windows PC to an Active Directory domain for
  centralized management.
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

# Join a PC to the Domain

### Prerequisites

* A domain controller running Active Directory.
* Administrative privileges on the PC and domain credentials (e.g., admin with domain admin rights).
* The PC must be connected to the network with access to the domain controller.
* The PC name should follow the naming pattern (e.g., PC206, PC15).

### Steps

1.  **Open the System Control Panel**:

    * On the PC, press `Windows + R` to open the Run dialog.
    * Type `sysdm.cpl` and press Enter to open the System Properties window.



    <div align="left"><figure><img src="../../../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure></div>
2.  **Access Computer Name Settings**:

    * In the System Properties window, go to the "Computer Name" tab.
    * Click the "Change..." button to modify the computer name and domain settings.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (90).png" alt="" width="314"><figcaption></figcaption></figure></div>

    *
3.  **Set the Computer Name and Domain**:

    * In the "Computer Name/Domain Changes" window, set the computer name following the naming pattern (e.g., PC206) in the "Computer name" field.
    * Under "Member of," select "Domain" and enter the domain name (e.g., company.local).
    * Click "OK" to proceed.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (91).png" alt="" width="312"><figcaption></figcaption></figure></div>
4.  **Enter Domain Admin Credentials**:

    * When prompted, enter the username (e.g., admin) and password of an account with permission to join the domain.
    * Click "OK" to continue.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (92).png" alt="" width="393"><figcaption></figcaption></figure></div>
5.  **Confirm Domain Join**:

    * A "Welcome to the company.local domain" message will appear.
    * Click "OK" to close the message.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (93).png" alt="" width="329"><figcaption></figcaption></figure></div>
6.  **Restart the PC**:

    * A prompt will appear stating "You must restart your computer to apply these changes".
    * Save any open files, close all programs, and click "OK".
    * Restart the PC to complete the domain join process.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (94).png" alt="" width="332"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Ensure the PC name (e.g., PC206) is unique in the domain to avoid conflicts. Verify the PC appears in Active Directory under the PCs OU after the restart. If the PC fails to join the domain, check network connectivity, DNS settings, and the admin credentials used.
{% endhint %}
