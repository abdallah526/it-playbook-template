---
description: Instructions for finding the IP address of an extension in PBX.
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

# Get Status & IP Address of Extension

### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../logging-into-pbx-admin.md).
* An existing extension (e.g., "1001").
* A web browser (e.g., Chrome, Firefox).

### Steps

1. **Navigate to Asterisk-CLI**:
   * From the main menu, go to "PBX" > "PBX Configuration" > "Tools" > "Asterisk-CLI."
2. **Execute the SIP Peers Command**:
   * In the "Command:" field, type `sip show peers`.
   * Click the "Execute" button to run the command.
3. **Locate the Extension**:
   * Scroll through the results to find the extension number (e.g., "1001/1001").
   * Note the "Status" column (e.g., "OK (126 ms)") and the "Host" column (e.g., "172.20.21.191") for the IP address.
4.  **Interpret the Results**:

    * "OK" indicates the extension is registered; other statuses (e.g., "UNKNOWN") suggest it’s unregistered.
    * The "Host" value provides the IP address of the device associated with the extension.

5. **Troubleshoot if Needed**:
   * If the status is "UNKNOWN," verify the extension’s SIP credentials in "PBX" > "Extensions" or check network connectivity.

{% hint style="info" %}
<mark style="color:red;">**Use this command periodically to monitor extension registration. For detailed logs, combine with "sip show peer \[extension]" (e.g.,**</mark><mark style="color:red;">**&#x20;**</mark><mark style="color:red;">**`sip show peer 1001`**</mark><mark style="color:red;">**) for specific details.**</mark>
{% endhint %}
