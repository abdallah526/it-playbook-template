---
description: >-
  This guide explains how to access the Sophos VPN Portal, log in using Active
  Directory credentials, and download the VPN client configuration files (Sophos
  Connect or OpenVPN) for remote access.
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

# Access VPN Portal & Download Client

Prerequisites

* A web browser (e.g., Chrome, Firefox).
* The Sophos VPN Portal URL with the specific port (e.g., https://\[firewall-ip]:4646).
* Active Directory credentials (username and password) or the user folder name.
* A device to install the VPN client (e.g., Windows, macOS, Linux, Android, or iOS).

### Steps

1. **Access the Sophos VPN Portal**:
   * Open a web browser and navigate to the Sophos VPN Portal URL using the specific port: https://\[firewall-ip]:4646.
   * Replace \[firewall-ip] with your Sophos Firewall’s IP address.
   * You will be directed to the VPN Portal login page.
2.  **Log in to the VPN Portal**:

    * On the login page, enter your **Username**. Use your Active Directory username or the user folder name (e.g., "jsmith").
    * Enter your **Password** associated with your Active Directory account.
    * Click **Login** to access the VPN Portal.

    <figure><img src="../../.gitbook/assets/image (259).png" alt=""><figcaption></figcaption></figure>
3. **Download the VPN Client Configuration**:
   * After logging in, you will see the VPN Portal dashboard with the **Sophos Connect client** section.
   * To download the Sophos Connect client:
     * Click **Download for Windows** if using a Windows device.
     * Click **Download for macOS** if using a macOS device.
   * To download the OpenVPN configuration for other devices:
     * In the **SSL VPN configuration** section, click **Download for Windows, macOS, Linux** under "Use with Sophos Connect and OpenVPN Connect clients" to download the configuration file for Sophos Connect or OpenVPN.
     * Alternatively, click **Download for Windows, macOS, Linux** under "Use with OpenVPN v3 clients" to download the configuration file for OpenVPN v3 clients.
     * For mobile devices, click **Download for Android and iOS** to download the configuration file for mobile OpenVPN clients.

<div align="left"><figure><img src="../../.gitbook/assets/image (260).png" alt=""><figcaption></figcaption></figure></div>

1.  **Install and Configure the VPN Client**:

    * Install the downloaded Sophos Connect client (for Windows or macOS) by running the installer and following the on-screen instructions.
    * If you get an Error during installation: 2502 or 2503, See ([MSI Installation Error 2502](../../incidents-and-troubleshooting/common-issues-quick-fixes/msi-installation-error-2502.md)).

    <div align="left"><figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure></div>

    * Import the downloaded VPN configuration file into the Sophos Connect client or OpenVPN client, depending on your device.

    <figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

    * Connect to the VPN using your Active Directory credentials.

    <div align="left"><figure><img src="../../.gitbook/assets/image (7).png" alt="" width="416"><figcaption></figcaption></figure></div>

    <div align="left"><figure><img src="../../.gitbook/assets/image (8).png" alt="" width="414"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Ensure the VPN Portal port (4646) is open on the firewall and accessible from your network. If you encounter login issues, verify the Active Directory username and password with the IT admin. Keep the downloaded configuration files secure, as they contain sensitive connection details.
{% endhint %}

<br>
