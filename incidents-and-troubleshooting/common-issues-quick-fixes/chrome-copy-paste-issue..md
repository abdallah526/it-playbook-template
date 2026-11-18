---
description: >-
  This guide addresses the issue of copy-paste not working in Chrome or Google
  Sheets due to a specific Chrome extension.
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

# Chrome Copy-Paste Issue

### Overview

* **Issue**: Copy-paste fails in Chrome or Google Sheets.
* **Cause**: The Chrome extension **Don't F\*\*\* with Paste** interferes with clipboard functionality, especially in Google Sheets.

### Steps to Resolve

1. **Identify the Extension**
   * Open Chrome and check if the **Don't F\*\*\* with Paste** extension is enabled (visible in the Extensions menu).
2.  **Modify Extension Settings**

    * Go to Chrome **Extensions** > **Manage Extensions**.
    * Find **Don't F\*\*\* with Paste**, click **Details**, then **Extension options**.
    * In the options, locate the list of patterns (e.g., https://docs.google.com).
    * Remove the pattern https://docs.google.com by clicking the **X** next to it.
    * Click **Save** to apply changes.

    <figure><img src="../../.gitbook/assets/image (285).png" alt=""><figcaption></figcaption></figure>
3. **Test Copy-Paste**
   * Open Google Sheets and test copy-paste functionality to confirm the issue is resolved.

{% hint style="danger" %}
If the issue persists, disable the extension temporarily via **Manage Extensions** > toggle off. Educate users to avoid enabling this extension on critical sites like Google Sheets.
{% endhint %}
