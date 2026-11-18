---
description: >-
  This guide explains how to assign the device to a TeamViewer account for
  remote management.
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

# Assign Device to TeamViewer Account

### Prerequisites

* TeamViewer installed on the device.
* TeamViewer account credentials:
  * Email: it-team@example.com
  * Password: Stored in Keeper Security (retrieve from Keeper using your credentials).
* A device to assign (e.g., a PC named PC159).

### Steps

1.  **Open TeamViewer and Check PC Name**:

    * Launch TeamViewer on the device.
    * In the TeamViewer main window, navigate to the **TeamViewer options** by clicking the gear icon in the top right corner.
    * In the options window, under the **General** tab, locate the **Your display name** field to check that the PC name is like our naming pattern (e.g., PC159).

    <figure><img src="../../../../.gitbook/assets/image (264).png" alt=""><figcaption></figcaption></figure>
2.  **Enable Unattended Access**:

    * In the TeamViewer main window, Click on **Easy Access not granted.**

    <figure><img src="../../../../.gitbook/assets/image (261).png" alt=""><figcaption></figcaption></figure>
3.  **Assign the Device to TeamViewer Account**:

    * In the **Grant Easy Access** pop-up window, enter the TeamViewer account email: it-team@example.com.
    * Retrieve the password from Keeper Security and enter it in the **Password** field.
    * Click **Assign** to link the device to the account.

    <figure><img src="../../../../.gitbook/assets/image (262).png" alt=""><figcaption></figcaption></figure>

    * A confirmation pop-up will appear, stating that a verification email has been sent to it-team@example.com. Check the inbox (or junk/spam folder) for the email and follow the link to confirm the device assignment.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (265).png" alt="" width="425"><figcaption></figcaption></figure></div>
4.  **Verify Assignment**:

    * After confirming the email, return to the TeamViewer main window.
    * Click **Easy Access not granted** again and repeat the above steps.
    * Under the **Unattended Access** section, confirm that **Easy Access for IT-Department is granted** is displayed.
    * Check the box for **Start TeamViewer with Windows**.
    * In the **TeamViewer options** window, under the **General** tab, verify that the **Account assignment** section shows "Assigned to IT-Department".

    <figure><img src="../../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Ensure the device is online during the assignment process. If the confirmation email is not received, check the spam/junk folder or verify the email address with the IT admin. Keep the TeamViewer password secure in Keeper Security.
{% endhint %}
