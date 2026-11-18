---
description: >-
  Instructions for installing Windows on a PC through the network using Windows
  Deployment Services (WDS) by booting via PXE.
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

# Install Windows Through WDS

### Prerequisites

* A configured WDS server (e.g., 172.20.31.252) with a boot image (e.g., boot.wim) and install image (e.g., Windows 10 OS).
* A PC with PXE boot capability and network connectivity to the WDS server.
* DHCP server configured to provide IP addresses (e.g., 172.20.31.250).
* Administrative credentials for the WDS server (e.g., admin@company.local).

### Steps

1. **Configure the PC to Boot from Network**:
   * Power on the PC and click F12 from the keyboard to change the boot order to IPV4 PXE boot.
2.  **Select the Boot Image**:

    * In the Windows Boot Manager (displaying the WDS server IP, e.g., 172.20.31.252), use the arrow keys to highlight the desired boot image (e.g., Windows 10 OS).
    * Press Enter to select the image and proceed.

    <figure><img src="../../../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>
3.  **Load Boot Files**:

    * The PC will load the boot files (e.g., boot.wim) from the WDS server (e.g., IP: 172.20.31.252).
    * Wait for the loading process to complete.

    <figure><img src="../../../.gitbook/assets/image (253).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../../.gitbook/assets/image (254).png" alt=""><figcaption></figcaption></figure>
4.  **Wait for Windows Setup to Start**:

    * The Windows Setup screen will appear, showing the Windows logo and a loading animation.
    * Wait for the setup to initialize.

    <figure><img src="../../../.gitbook/assets/image (256).png" alt=""><figcaption></figcaption></figure>
5.  **Set Language and Keyboard**:

    * In the Windows Setup window, select the locale (e.g., English (United States)) and keyboard input method (e.g., US).
    * Click "Next" to continue.

    <figure><img src="../../../.gitbook/assets/image (257).png" alt=""><figcaption></figcaption></figure>
6.  **Connect to the WDS Server**:

    * In the "Connect to 172.20.31.250" window, enter the administrative credentials (e.g., User name: admin@company.local, Password).
    * Click "OK" to connect.

    <figure><img src="../../../.gitbook/assets/image (258).png" alt=""><figcaption></figcaption></figure>
7. **Select the Install Image**:
   * In the Windows Setup window, select the desired install image (e.g., Windows 10 OS) (1).
   * Click "Next" to begin the installation.
8. **Wait for Installation to Complete**:
   * The setup will proceed with installing Windows, starting with "Setup is starting".
   * Follow any additional on-screen prompts to complete the installation.

{% hint style="info" %}
Ensure the PC’s network adapter supports PXE boot and is properly configured in the BIOS. Verify the WDS server (e.g., 172.20.31.250) is online and accessible. If the PC fails to boot or connect, check DHCP settings, network connectivity, and the WDS server configuration.
{% endhint %}
