---
description: >-
  This guide explains how to turn off Tamper Protection for a device in Sophos
  Central to allow administrative changes.
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

# Turn Off Tamper Protection

### Prerequisites

* Access to the Sophos Central web portal.
* Sophos Central credentials and Tamper Protection password, provided by the IT admin via Keeper Security.
* A device with Sophos Endpoint Protection installed (e.g., BRANCH-C-PC01).

### Steps

1.  **Log in to Sophos Central**:

    * Open a web browser and navigate to the Sophos Central login page.
    * Sign in using the credentials provided by the IT admin via Keeper Security

    <figure><img src="../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>
2.  **Navigate to Computers**:

    * From the dashboard, click **My Products** and select **Endpoint Protection.**
    * Click **Computers** in the left sidebar to view the list of devices.

    <figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>
3.  **Select the Device**:

    * Locate the device (e.g., BRANCH-C-PC01) in the list..
    * Click the device name to access its details.

    <figure><img src="../../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>
4.  **Turn Off Tamper Protection**:

    * In the device details, scroll to the **Tamper Protection** section.
    * Click **Turn off tamper protection**.
    * Or copy the Tamper Protection password shown on this page.

    <figure><img src="../../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>
5.  **Verify Tamper Protection Status**:

    * On the device, open the Sophos Endpoint Protection client.

    <figure><img src="../../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

    * Click **Admin sign-in**.
    * Enter the Tamper Protection password and click **Admin sign-in**.

    <figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

    * Confirm that Tamper Protection is disabled, allowing administrative changes.

    <figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Use the Tamper Protection password only when necessary, as disabling it reduces security. Re-enable Tamper Protection after making changes to ensure device protection.
{% endhint %}
