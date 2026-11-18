---
description: >-
  Instructions for logging into the PortSIP UC app on Android to connect to the
  PBX server for VoIP calls, ensuring the account is active and registered.
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

# PortSip UC

## Prerequisites

* An Android device with the PortSIP UC app installed.
* SIP account details from your IT admin (e.g., SIP User ID, password, SIP server address).
* Network connectivity (Wi-Fi or mobile data).
* The PBX server (172.20.31.10:5060) is operational.
* For external use: OpenVPN app installed and a VPN file provided by your IT admin.

### Steps

1.  **Open the PortSIP UC App**:

    * Launch the PortSIP UC app on your Android device.
    * The app will open directly to the Sign in screen.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (214).png" alt="" width="242"><figcaption></figcaption></figure></div>
2. **Log in with SIP Credentials**:
   * **SIP User ID**: Enter your extension (e.g., "677").
   * **Password**: Enter the SIP password provided by your IT admin.
   * **SIP Server**: Enter the PBX server address: 172.20.31.10.
   * Tap the "Sign in" button to log in.
   * The app will attempt to register with the PBX server.
3.  **Navigate to Settings to Verify Login**:

    * Once logged in, you’ll be taken to the Dialpad screen.
    * Tap the "Settings" icon at the bottom right.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (215).png" alt="" width="237"><figcaption></figcaption></figure></div>
4.  **Check Account Status**:

    * In the Settings menu, tap "Account" to view the account status.
    * Confirm the status shows "Online" with a green dot next to the account (e.g., "677 Online").

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (216).png" alt="" width="235"><figcaption></figcaption></figure></div>
5. **Verify with a Test Call**:
   * Return to the Dialpad screen by tapping the "Dialpad" icon.
   * Make a test call to verify the account is active and connected to the PBX server.

{% hint style="info" %}
If the login fails or the status remains offline, verify the SIP credentials and server address with your IT admin. Check network connectivity to 172.20.31.10:5060, and contact your IT admin if issues persist.
{% endhint %}
