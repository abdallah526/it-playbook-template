---
description: >-
  Instructions for configuring the SessionTalk SIP Softphone app on an iPhone to
  make and receive VoIP calls, including setup for external access via OpenVPN.
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

# iPhone

### Prerequisites

* An iPhone running iOS (e.g., iOS 15 or later).
* The SessionTalk SIP Softphone app is installed (download from [App Store](https://apps.apple.com/us/app/sessiontalk-sip-softphone/id362501443)).
* SIP account details from your IT admin (e.g., username, password, domain, display name).
* Internet connection (Wi-Fi or mobile data).
* For external use: OpenVPN app installed and a VPN file provided by your IT admin.

### Steps

1.  **Install the SessionTalk SIP Softphone App**:

    * Open the App Store on your iPhone.
    * Search for "SessionTalk SIP Softphone" and install the app (version 7.0.5 or later).
    * Launch the app after installation.

    <div align="left"><figure><img src="../../../.gitbook/assets/image (125).png" alt="" width="185"><figcaption></figcaption></figure></div>
2.  **Access Settings**:

    * Open the SessionTalk app.
    * From the keypad screen, tap the "Settings" icon at the bottom right.

    <div align="left"><figure><img src="../../../.gitbook/assets/image (116).png" alt="" width="234"><figcaption></figcaption></figure></div>
3.  **Navigate to SIP Accounts**:

    * In the Settings menu, tap "SIP Accounts" under "CONFIGURE SETTINGS."

    <div align="left"><figure><img src="../../../.gitbook/assets/image (121).png" alt="" width="296"><figcaption></figcaption></figure></div>
4.  **Create a New SIP Account**:

    * Tap "Generic SIP" from the list of VoIP providers.

    <div align="left"><figure><img src="../../../.gitbook/assets/image (122).png" alt="" width="249"><figcaption></figcaption></figure></div>
5.  **Enter SIP Account Details**:

    * Fill in the following fields with the details provided by your IT admin:
      * **Account Name**: Generic SIP
      * **Enabled**: Toggle to "On"
      * **Display Name**: Your name (e.g., "John-Smith-IT")
      * **UserName**: Your SIP extension (e.g., "692")
      * **Password**: Your SIP password
      * **Domain**: SIP server address (e.g., "172.20.31.10")
    * Tap "Save" to apply the settings.

    <div align="left"><figure><img src="../../../.gitbook/assets/image (119).png" alt="" width="292"><figcaption></figcaption></figure></div>
6.  **Verify Registration**:

    * Return to the SIP Accounts screen.
    * Ensure the "Generic SIP" account shows a green checkmark.

    <div align="left"><figure><img src="../../../.gitbook/assets/image (117).png" alt="" width="270"><figcaption></figcaption></figure></div>
7. **Test the Softphone**:
   * Return to the keypad screen and dial a test extension (e.g., another employee’s extension).
   * Confirm you can make and receive calls successfully.

### External Access with OpenVPN

* If you are outside the company network (e.g., not on the network for the head office):
  1. Install the OpenVPN app from the App Store.
  2. Obtain the VPN file from your IT admin (e.g., `company_vpn.ovpn`).
  3. Import the VPN file into the OpenVPN app and connect to the VPN.
  4. Once connected, launch the SessionTalk app and confirm the SIP account registers successfully.

{% hint style="info" %}
Ensure the SIP server (e.g., 172.20.31.10:5060) is accessible. For external access, the OpenVPN connection is mandatory to securely connect to the company network. If the account fails to register, verify your SIP credentials and network connectivity. Contact your IT admin for assistance with VPN setup or SIP server issues.
{% endhint %}

