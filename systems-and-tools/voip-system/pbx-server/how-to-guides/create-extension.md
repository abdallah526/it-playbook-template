---
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

# Create Extension

#### Purpose

Create SIP extensions for users to enable internal calls between departments and branches.

#### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../logging-into-pbx-admin.md).
* User details (e.g., name, extension number like `1001`).

#### Steps

1. **Navigate to PBX**:
   * From the PBX dashboard, click "PBX" > "PBX Configuration" > "Extensions."
2.  **Add a New Extension**:

    * Select "Generic SIP Device" as the device type.
    * Click "Submit."

3.  **Enter Details**:

    * **User Extension:** `679`
    * **Display Name**: User’s name (e.g., "John Smith").
    * **Secret**: Generate or set a password (store it in the password manager).
    * **Call Waiting:** Disable.
    * dtmfmode: RFC 2833
    * nat: Yes
    * Recording Options : All is always.
    * Leave other settings default unless specified.

    <figure><img src="../../../../.gitbook/assets/image (173).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>
4.  **Save and Apply**:

    * Click "Submit."
    * Click "Apply Changes" at the top to update the server.

5. **Test**:
   * Configure the extension in MicroSIP (see MicroSIP > How-To Guides >[ Adding a SIP Account](../../softphones/microsip/how-to-guides/add-sip-account.md)).
