---
description: Instructions for logging an agent into a call queue in PBX.
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

# Login to Queue

### Prerequisites

* Access to the Agent Console via the Call Center interface.
* Valid extension details (e.g., "SIP/677 - John Smith") and password.
* A web browser (e.g., Chrome, Firefox).
* The extension must be registered and assigned to a queue (see [Add Extension to Queue](add-extension-to-queue.md)).

### Steps

1. **Navigate to the Agent Console**:
   * Log in to the Call Center interface.
   * From the main menu, go to "Call Center" > "Agent Console."
2.  **Enter Login Credentials**:

    * In the "Extension:" dropdown, select your extension (e.g., "SIP/677 - John Smith").
    * In the "Password:" field, enter your password.
    * check the "Callback" checkbox, callback login is required.

    <figure><img src="../../../../.gitbook/assets/image (141).png" alt=""><figcaption></figcaption></figure>
3. **Log In to the Queue**:
   * Click the "Enter" button to log in.
   * Wait for the interface to load and display your agent console (e.g., "Agent Console: SIP/587 - John Smith").
4.  **Verify Queue Login**:

    * Confirm the interface shows "No active call" and options like "Take Break," "Transfer," and "End session."
    * Ensure you receive calls from the assigned queue (test by having someone call the queue number).

    <figure><img src="../../../../.gitbook/assets/image (142).png" alt=""><figcaption></figcaption></figure>
5. **Troubleshoot if Needed**:
   * If login fails, verify the extension and password created in [Create Callback Extension](create-callback-extension.md).
   * Check the queue configuration to ensure the extension is added (see [Add Extension To Queue](add-extension-to-queue.md)).
   * Ensure that the Extension is registered (see [Get Status & IP Address of Extension](get-status-and-ip-address-of-extension.md)).
