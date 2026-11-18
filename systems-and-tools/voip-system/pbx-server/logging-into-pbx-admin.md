---
description: How to sign in to the PBX admin web interface.
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

# Logging into PBX Admin

## Prerequisites

* Admin credentials (username and password) provided by the VoIP admin.
* A web browser (e.g., Chrome, Firefox).
* Network access to `172.20.31.10`.

### Steps

1. **Open the Admin URL**:
   * In your browser, navigate to `http://172.20.31.10/index.php`.
   *

2. **Enter Credentials**:
   * Username: `[admin-username]` (e.g., `admin`).
   * Password: `[admin-password]`.
   * Click "Login."
3. **Verify Access**:
   * You should see the PBX admin dashboard, with options like "PBX," "Reports," and "System."

{% hint style="info" %}
If login fails, verify credentials with the VoIP admin and check server status. Ensure port 80 is open on your network.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>
