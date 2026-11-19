---
description: >-
  This guide explains how to configure TeamViewer to automatically record remote
  sessions for documentation or auditing purposes.
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

# Recording Remote Sessions

### Prerequisites

* TeamViewer desktop application installed on your device.
* A TeamViewer account with appropriate permissions to modify settings.
* A designated network folder path for storing recorded sessions (e.g., \\\FILESERVER\TeamViewer$\jsmith).
* Active Directory credentials to access the network folder (username and password).

### Steps

1. **Open TeamViewer Options**:
   * Launch the TeamViewer application on your device.
   * Click the gear icon in the top right corner to open the **TeamViewer options**.
2. **Navigate to Remote Control Settings**:
   * In the TeamViewer options window, click **Remote control** from the left sidebar to access remote session settings.
3.  **Enable Automatic Recording**:

    * Under the **Remote control defaults** section, check the box for **Start recording of remote control sessions automatically**.
    * Ensure other desired settings (e.g., "Play computer sounds and music") are configured as needed.

    <figure><img src="../../../../.gitbook/assets/image (268).png" alt=""><figcaption></figcaption></figure>
4.  **Set the Recording Directory**:

    * In the **Advanced** section of the TeamViewer options, locate the **Session recording directory** field.
    * Enter the designated network folder path for storing recordings: \\\FILESERVER\TeamViewer$\Foldername.
    * The foldername will be given by IT Admin

    <figure><img src="../../../../.gitbook/assets/image (269).png" alt=""><figcaption></figcaption></figure>
5.  **Create a Network Location Folder**:

    * If the network folder path (e.g., \\\FILESERVER\TeamViewer$\jsmith) is not already set up as a network location, you need to add it.
    * Open File Explorer on your device.
    * Right-click on **This PC** or **Network** in the left sidebar and select **Add a network location**.
    * In the **Add Network Location** wizard, click **Next**.
    * In the **Internet or network address** field, enter the network path: \\\FILESERVER\TeamViewer$\Foldername.
    * Click **Next** to proceed.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (272).png" alt="" width="521"><figcaption></figcaption></figure></div>
6.  **Enter Network Credentials**:

    * A **Windows Security** pop-up will appear, asking for credentials to connect to the network location (e.g., \\\FILESERVER).
    * Enter your **User name** (e.g., your Active Directory username).
    * Enter your **Password** associated with your Active Directory account.
    * Check the box for **Remember my credentials** to avoid entering them again in the future.
    * Click **OK** to authenticate and connect to the network location.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (273).png" alt="" width="523"><figcaption></figcaption></figure></div>
7. **Save the TeamViewer Settings**:
   * Return to the TeamViewer options window.
   * Click **OK** to save the changes and apply the recording settings.

{% hint style="info" %}
Ensure the specified recording directory (\\\FILESERVER\TeamViewer$\foldername) is accessible and has sufficient storage space. Verify that the user account has write permissions to the folder. If you encounter access issues, confirm your Active Directory credentials with the IT admin. Recordings may contain sensitive data, so secure the directory and comply with company data retention policies.
{% endhint %}
