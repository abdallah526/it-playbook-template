---
description: >-
  Instructions for upgrading a Windows PC from the Home edition to the Pro
  edition to enable domain joining and advanced features.
icon: up-to-line
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

# Upgrade Windows from Home to Pro Edition

### Prerequisites

* A Windows PC running Windows 10/11 Home edition.
* A valid product key for Windows 10/11 Pro (25-character code).
* Administrative privileges on the PC.
* Internet connection (for downloading the upgrade and activating).
* Backup of important data (recommended).

### Steps

1. **Open Settings**:
   * Press `Win + I` to open Settings.
   * Navigate to "Update & Security" > "Activation."
2.  **Initiate Upgrade**:

    * Click "Change product key".
    * Select the option to upgrade to Windows Pro or enter the Pro product key (stored in the password manager).

    <figure><img src="../.gitbook/assets/image (112).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../.gitbook/assets/image (113).png" alt=""><figcaption></figcaption></figure>
3. **Confirm and Download**:
   * Follow the on-screen prompts to confirm the upgrade.
   * Windows will download the Pro edition files (internet required).
4. **Install the Upgrade**:
   * After downloading, click "Install" to begin the upgrade process.
   * The PC will restart several times during installation (data is preserved).
5. **Verify Upgrade**:
   * After reboot, return to "Update & Security" > "Activation" and confirm "Windows 10/11 Pro" is activated.
   * Test domain joining (see Join a PC to the Domain under Active Directory > How To Guide).

{% hint style="info" %}
Ensure the Pro product key is valid and matches your organization’s licensing agreement. If the upgrade fails, use the Media Creation Tool from Microsoft’s website to perform a clean upgrade, or contact your IT administrator for assistance.
{% endhint %}
