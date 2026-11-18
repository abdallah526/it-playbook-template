---
description: >-
  Instructions for configuring the network, account, and DSS key settings on a
  Yealink T21P IP phone, including hotdesking setup.
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

# Configure Settings

### Prerequisites

* A powered-on Yealink IP phone.
* Admin credentials (default: username "admin", password "admin").
* Network details: VLAN 21, IP range 172.20.21.0/24, SIP server (e.g., 172.20.31.10, port 5060, UDP).
* Access to the phone’s web interface via its IP address.

### Steps

1.  **Get IP Address of IP Phone:**

    * Click "OK" button in the IP Phone to see Status and IP Address.

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (193).png" alt="" width="316"><figcaption></figcaption></figure></div>
2.  **Access the Web Interface**:

    * Refer to Login to access the IP Phone web interface using its IP address.

    <figure><img src="../../../../../.gitbook/assets/image (127).png" alt=""><figcaption></figcaption></figure>
3.  **Configure Network Settings**:

    * Navigate to the "Network" tab.
    * Under "Internet Port," set "Mode (IPv4/IPv6)" to "IPv4."
    * Select "DHCP" to automatically obtain an IP address (e.g., within 172.20.21.0/24 for VLAN 21).
    * Select Advanced, Under "VLAN," enable "WAN Port" and set "VID (1-4094)" to "21" with "Priority" as "0."
    * Ensure that "PC Port" status is Disabled.&#x20;
    * Click "Confirm" to save.

    <figure><img src="../../../../../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../../../../.gitbook/assets/image (130).png" alt=""><figcaption></figcaption></figure>
4.  **Configure Account Settings**:

    * Navigate to the "Account" tab.
    * Set "Line Active" to "Enabled."
    * Enter "Label" and "Display Name" (e.g., "John - IT").
    * Set "Register Name" and "User Name" to the extension (e.g., "677").
    * Enter the SIP server details:
      * Server Host: "172.20.31.10"
      * Port: "5060"
      * Transport: "UDP"
      * Server Expires: "3600"
      * Server Retry Counts: "3"
    * Click "Confirm" to save.

    <figure><img src="../../../../../.gitbook/assets/image (128).png" alt=""><figcaption></figcaption></figure>
5.  **Set Up Hotdesking with the Message Button and Other Buttons:**

    * Navigate to the "DSSkey" tab.
    * Under "Programmable Key," set "SoftKey1" to "History".
    * Set "Down" to "Directory".
    * Set "Right" to "Menu".
    * Set "OK" to "Status".
    * Set "TRAN" to "Forward".
    * Set "Message" to "Hot Desking".
    * Other Keys to " N/A".
    * Click "Confirm" to save.

    <figure><img src="../../../../../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure>
6. **Verify Configuration**:
   * Ensure the phone registers with the SIP server (check the "Status" tab for "Registered").
   * Test the Message button to confirm hotdesking functionality.

{% hint style="info" %}
If the phone fails to register, verify the SIP server details and network connectivity. Ensure VLAN 21 is properly configured on the switch.
{% endhint %}
