---
description: >-
  This guide explains how to configure the ADMS (Access Data Management Service)
  settings in ZKTeco BioTime to enable cloud-based communication between the
  BioTime server and ZKTeco devices.
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

# Connect Biometric Device - ADMS

### Prerequisites

* BioTime server running at `http://172.20.31.30:8081`.
* Administrative access to BioTime.
* A ZKTeco device supporting ADMS (e.g., fingerprint or facial recognition device).
* An active internet connection for cloud communication.

### Steps

1.  Go to "Menu" from the Device and Select "COMM."<br>

    <div align="left"><figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure></div>
2.  Go To "Cloud Server Settings"



    <div align="left"><figure><img src="../../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure></div>
3. Make sure the "Server Mode" is set to "ADMS."
4. Set "Server Address" to "172.20.31.30."
5. Set "Server Port" to "8081."
6. Set " Enable Proxy Server" to **OFF**
7.  Set "Enable Domain Name" to **OFF**



    <div align="left"><figure><img src="../../../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure></div>
8.  Return Back and select "Ethernet" or  "Wireless Network" based on the type of connection.



    <div align="left"><figure><img src="../../../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure></div>
9.  Make sure the Device is set to "DHCP"



    <div align="left"><figure><img src="../../../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure></div>
10. Now you can run the BioTime 8.0 Software and enter the credential
11. In the Device Tab, the Status of the device will be Green

<figure><img src="../../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
ADMS enables remote management of devices over the internet. If the device fails to connect, ensure port 8081 is open on your firewall and that the device has internet access.
{% endhint %}

