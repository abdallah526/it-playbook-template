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

# Add SIP Account

#### Prerequisites

* MicroSIP installed (see [Installation Guide](../installation.md)).
* SIP credentials from PBX admin (e.g., Username: `1001`, Password: `[secure-password]`, Server: `172.20.31.10`).

#### Steps

1. **Open MicroSIP**:
   * Launch MicroSIP with admin rights if needed.
2.  **Access Settings**:

    * Click the menu (top-right three lines) and select "Add Account."

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (167).png" alt="" width="386"><figcaption></figcaption></figure></div>
3.  **Configure Account**:

    * Enter:
      * **SIP Server**: `172.20.31.10`
      * **Account Name:** `1001`
      * **Username**: `1001`
      * **Domain:** `172.20.31.10`
      * **Login:** `1001`
      * **Password**: `[secure-password]`
      * **Display Name**: IT-assigned name (e.g., "IT Support").
    * Leave Proxy and Transport as default unless specified.

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (168).png" alt="" width="322"><figcaption></figcaption></figure></div>
4.  **Save and Test**:

    * Click "OK."
    * Verify "Online" status in the bottom bar.

    <div align="left"><figure><img src="../../../../../.gitbook/assets/image (169).png" alt="" width="219"><figcaption></figcaption></figure></div>
