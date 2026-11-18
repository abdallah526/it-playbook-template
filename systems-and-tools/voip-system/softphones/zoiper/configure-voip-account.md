---
description: >-
  Instructions for configuring a SIP account in the Zoiper5 softphone on macOS
  to connect to the PBX server, including login, hostname setup, and audio
  configuration.
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

# Configure VoIP Account

### Prerequisites

* Zoiper installed on your macOS device (see[ Install Zoiper on macOS](installation.md)).
* SIP account details from your IT admin (e.g., SIP User ID, password, SIP server address).
* Network connectivity.
* The PBX server (172.20.31.10:5060) is operational.
* For external use: OpenVPN app installed and a VPN file provided by your IT admin.

### Steps

1.  **Launch Zoiper and Log In**:

    * Open Zoiper from the Applications folder.
    * On the initial login screen, enter the following:
      * **Username**: Enter your SIP User ID + SIP Server (e.g., "918@172.20.31.10") (1).
      * **Password**: Enter the SIP password provided by your IT admin (1).
    * Click the "Login" button to proceed.

    <figure><img src="../../../../.gitbook/assets/image (226).png" alt=""><figcaption></figcaption></figure>
2. **Configure Hostname**:
   *   After login, select your hostname provider:

       * Enter "172.20.31.10" as the hostname.
       * Click "Next" to continue.

       <figure><img src="../../../../.gitbook/assets/image (227).png" alt=""><figcaption></figcaption></figure>
3.  Click "Skip" to proceed.

    <figure><img src="../../../../.gitbook/assets/image (228).png" alt=""><figcaption></figcaption></figure>
4.  **Select Transport Protocol**:

    * Choose a transport protocol from the available options:
      * Select "SIP UDP" (recommended if available).
    * Click "Next" to continue.

    <figure><img src="../../../../.gitbook/assets/image (229).png" alt=""><figcaption></figcaption></figure>
5.  **Configure Audio Settings**:

    * On the audio configuration screen, test your devices:
      * Click "Start test" under "Speaker" to verify your speakers.
      * Click "Start test" under "Microphone" to verify your microphone.
    * Click "Skip" on each test if audio is already configured, or "Configure" and follow the prompts to adjust settings.

    <figure><img src="../../../../.gitbook/assets/image (231).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../../../.gitbook/assets/image (230).png" alt=""><figcaption></figcaption></figure>
6.  **Finalize Configuration**:

    * After audio setup, click "Finish" to complete the configuration.

    <figure><img src="../../../../.gitbook/assets/image (232).png" alt=""><figcaption></figcaption></figure>

    * Verify the account status in the Zoiper interface shows "Registered" with a green dot.
7. **Verify with a Test Call**:
   * Use the dialpad to make a test call to confirm the connection to the PBX server.

{% hint style="info" %}
If registration fails, verify the SIP credentials, hostname (172.20.31.10), and port (5060) with your IT admin. Check network connectivity to the PBX server. If audio issues persist, manually configure devices in Preferences > Audio. Contact your IT admin for assistance with outbound proxy or authentication settings if required.
{% endhint %}
