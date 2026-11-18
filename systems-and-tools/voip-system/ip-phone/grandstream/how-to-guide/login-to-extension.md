---
description: >-
  Instructions for configuring SIP settings on a Grandstream GRP2612P IP phone
  to connect to the PBX server.
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

# Login to Extension

### Prerequisites

* A powered-on Grandstream IP phone with network access.
* SIP account details from your IT admin (e.g., username, password, server address).
* Access to the phone’s web interface (default login: admin/admin).

### Steps

1.  **Access the Web Interface**:

    * Identify the phone’s IP address from the display (e.g., 172.20.21.x).
    * Open a browser and enter the IP address (e.g., http://172.20.21.x).
    * Log in with default credentials (e.g., username: admin, password: admin).

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (200).png" alt="" width="563"><figcaption></figcaption></figure></div>
2. **Configure SIP Settings**:
   * Click the "Accounts" tab.
   * **Account Active**: Set to "Yes".
   * **SIP Server**: Enter 172.20.31.10:5060.
   * **SIP User ID**: Enter your extension (e.g., "918").
   * **SIP Authentication ID**: Enter your extension (e.g., "918").
   * **SIP Authentication Password**: Enter the password provided by your IT admin.
   * **Name**: Enter your name (e.g., "Jane Doe").
3.  **Save and Apply**:

    * Click "Save and Apply" to update settings.

    <figure><img src="../../../../../.gitbook/assets/image (202).png" alt=""><figcaption></figcaption></figure>
4.  **Verify Registration**:

    * Go to the "Status" tab and select "Account Status".
    * Confirm "YES" under SIP Registration for Account 1.

    <figure><img src="../../../../../.gitbook/assets/image (205).png" alt=""><figcaption></figcaption></figure>
5. **Test**:

* Make a test call to verify the extension is active.

{% hint style="info" %}
Ensure the SIP server (172.20.31.10:5060) is accessible. If registration fails, refer to [Registration Failure](../troubleshooting/registration-failure.md). Contact your IT admin for credentials or issues.
{% endhint %}
