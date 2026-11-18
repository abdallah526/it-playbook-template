---
description: >-
  This guide explains how to log in to the Sophos Firewall web admin console to
  manage network security settings and configurations.
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

# Login To The Firewall

### Prerequisites

* A PC with a web browser (e.g., Chrome, Firefox, Edge).
* The Sophos Firewall IP address, provided by the IT admin via Keeper Security.
* Administrative credentials for Sophos Firewall, also provided by the IT admin via Keeper Security.
* Network access to the Sophos Firewall device (ensure you are on the same network or have remote access if configured).

### Steps

1. **Open a Web Browser**:
   * Launch a supported web browser on your PC.
   * Ensure the browser is updated to avoid compatibility issues.
2. **Enter the Firewall IP Address**:
   * In the browser’s address bar, enter the Sophos Firewall IP address (e.g., `https://172.20.11.1:4545` or another IP provided by the IT admin via Keeper Security).
   * The Port of Web admin page is `4545`.
   * Press Enter to load the login page.
3.  **Enter Login Credentials**:

    * On the login page, enter the username and password provided by the IT admin via Keeper Security.
    * Avoid storing credentials in the browser for security reasons.

    <figure><img src="../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>
4. **Log in to the Dashboard**:
   * Click the **Login** button.
   * If the credentials are correct, you’ll be directed to the Sophos Firewall dashboard, which includes sections like System Status, Network, and Logs.
5.  **Verify Dashboard Access**:

    * Confirm you can navigate the dashboard and view key information (e.g., firewall status, active connections, or log entries).

    <figure><img src="../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
The address may use HTTPS (e.g., `https://`) depending on the firewall’s configuration; if it uses HTTP, adjust accordingly.
{% endhint %}

{% hint style="info" %}
If the login page does not load, verify the IP address and ensure port 4545 (for HTTPS) is open on your network firewall. Contact the IT admin to retrieve updated credentials from Keeper Security if access is denied.
{% endhint %}
