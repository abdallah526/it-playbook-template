---
description: >-
  Instructions for logging into the Yealink T21P IP phone, including hotdesking
  via the Message button and web interface access.
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

* A powered-on Yealink IP phone connected to the network (eg, VLAN 21, IP range: 172.20.21.0/24).
* A computer on the same network for web login.
* The phone’s IP address (obtainable from the phone’s display or DHCP logs) for web login.
* admin credentials (eg, username: "admin", password: "admin") for web login.
* Hotdesking configured (e.g., Message button set to "Hot Desking" with value "692" as per [Configure Settings](configure-settings.md)).

### Steps

#### Method 1: Login via Hotdesking

1. **Access the Message Button**:
   * On the Yealink IP phone, locate the "Message" button (configured for hotdesking).
2.  **Initiate Hotdesking**:

    * Press the "Message" button to start the hotdesking login process.
    * Click OK for "Clear all account config?"

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (194).png" alt="" width="364"><figcaption></figcaption></figure></div>
3.  **Enter Credentials**:

    * Use the phone’s keypad to enter your hotdesking credentials (e.g., extension "692" and associated password).
    * Click the down button to go to the password step.

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (199).png" alt="" width="333"><figcaption></figcaption></figure></div>

    * Enter the password, then click Save (see the screenshot for changing the input type)

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (196).png" alt="" width="335"><figcaption></figcaption></figure></div>

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (197).png" alt="" width="317"><figcaption></figcaption></figure></div>
4.  **Verify Login**:

    * Ensure the phone displays your extension (e.g., "692") or name (e.g., "John Smith") after login.
    * If you see "No Service," ensure you have entered the correct password, or see ([No Service](../troubleshooting/no-service-issue.md)) for more troubleshooting methods.

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (198).png" alt="" width="321"><figcaption></figcaption></figure></div>

#### Method 2: Login via Web Interface

* See ([Configure Account Settings](configure-settings.md)).

{% hint style="info" %}
For hotdesking issues, verify the Message button configuration in Configure Settings. If web login fails, ensure the phone’s IP is correct and your computer is on VLAN 21. Reset the password if changed (see Reset Factory).
{% endhint %}
