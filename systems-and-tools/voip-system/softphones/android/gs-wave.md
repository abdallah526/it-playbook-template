---
description: >-
  Instructions for configuring a new SIP account on the GS Wave app for Android,
  allowing users to connect to the PBX server for VoIP calls.
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

# GS Wave

### Prerequisites

* An Android device with the GS Wave app installed from this link : \
  [https://play.google.com/store/apps/details?id=com.grandstream.wave](https://play.google.com/store/apps/details?id=com.grandstream.wave)
* SIP account details from your IT admin (e.g., SIP User ID, password, SIP server address).
* Network connectivity (Wi-Fi or mobile data).
* The PBX server (172.20.31.10:5060) is operational.
* For external use: OpenVPN app installed and a VPN file provided by your IT admin.

### Steps

1.  **Open the GS Wave App**:

    * Launch the GS Wave app on your Android device.
    * From the main screen (e.g., Call History), tap the "Settings" icon at the bottom right (1).



    <div align="left"><figure><img src="../../../../.gitbook/assets/image (210).png" alt="" width="228"><figcaption></figcaption></figure></div>
2.  **Navigate to Account Settings**:

    * In the Settings menu, tap "Account Settings" (2).

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (208).png" alt="" width="239"><figcaption></figcaption></figure></div>
3.  **Add a New Account**:

    * In the Account Settings screen, tap the "+" icon at the top right to add a new account (3).

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (209).png" alt="" width="236"><figcaption></figcaption></figure></div>
4.  **Select SIP Account Type**:

    * In the "Add New Account" menu, select "SIP Account" from the list (4).

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (211).png" alt="" width="245"><figcaption></figcaption></figure></div>
5.  **Configure the SIP Account**:

    * **Activate Account**: Toggle the "Active Account" switch to ON (5).
    * **SIP Server**: Enter the PBX server address: 172.20.31.10:5060 (6).
    * **SIP User ID**: Enter your extension (e.g., "918") (6).
    * **SIP Authentication ID**: Enter your extension (e.g., "918") (6).
    * **Password**: Enter the SIP password provided by your IT admin (6).
    * **Display Name**: Enter your name (e.g., "John") (6).
    * Leave "Voicemail UserID" blank unless specified by your IT admin.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (212).png" alt="" width="254"><figcaption></figcaption></figure></div>
6.  **Save the Account**:

    * Tap the checkmark icon at the top right to save the account (7).
    * The account (e.g., "John") will appear in the Account Settings list with a green dot indicating successful registration (8).

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (213).png" alt="" width="260"><figcaption></figcaption></figure></div>
7. **Verify**:
   * Return to the main screen and check if the account name (e.g., "John") appears at the top.
   * Make a test call to confirm the account is active and connected to the PBX server.

{% hint style="info" %}
Verify the SIP credentials with your IT admin if registration fails (e.g., no green dot appears). Contact your IT admin if the PBX server (172.20.31.10:5060) is unreachable. For troubleshooting, check network connectivity or reconfigure the account.
{% endhint %}
