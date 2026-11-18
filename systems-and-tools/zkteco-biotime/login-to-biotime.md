---
description: >-
  This guide explains how to log in to the ZKTeco BioTime web interface to
  manage time and attendance operations.
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

# Login To BioTime

### Prerequisites

* A PC with a web browser (e.g., Chrome, Firefox).
* BioTime server accessible at `http://172.20.31.30:8081`.
* Valid administrative credentials for BioTime (username and password set during installation).

### Steps

1.  **Open the BioTime Login Page**:

    * Open a web browser on your PC.
    * Enter the BioTime server URL: `http://172.20.31.30:8081`.
    * Press Enter to load the login page.

    <figure><img src="../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>
2. **Enter Login Credentials**:
   * On the login page, enter your username and password in the respective fields.
   * Ensure the credentials match those set up during the BioTime server installation.
3. **Log In to the Dashboard**:
   * Click the **Log In** button.
   * If the credentials are correct, you’ll be directed to the BioTime dashboard, which includes the Real-Time Monitoring interface by default.
4.  **Verify Dashboard Access**:

    * Confirm you can see the dashboard with sections like Devices, Personnel, and Attendance Reports.
    * Check for real-time data, such as device status or recent clock-ins.

    <figure><img src="../../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
If you cannot access the login page, ensure the BioTime server at `http://172.20.31.30:8081` is running and that port 8081 is not blocked by your firewall. For security, avoid sharing administrative credentials and consider enabling two-factor authentication if supported by your BioTime version.
{% endhint %}
