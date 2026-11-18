---
description: Instructions for changing a user’s email address in Zoho Workspace.
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

# Change Email Address

### Prerequisites

* Access to the Zoho Mail admin panel with administrative privileges.
* The user’s email account must be active in the Zoho Mail organization.
* A new email address owned by the user that is not already in use within Zoho Mail.
* Network connectivity to access the Zoho Mail admin panel.

### Steps

1. **Navigate to Users in Zoho Mail Admin Panel**:
   * Log in to the Zoho Mail admin panel.
   * In the left sidebar, click on "Users" to view the list of users.
   * Locate the user whose login email address needs to be changed (e.g., "John Smith") and click on it.
2.  **Add a New Login Email Address**:

    * In the left sidebar, under "Security," click on "Login Email Address" to view the current login email settings.
    * Click the "+ Add" button to add a new login email address.
    * In the "Confirm Action" popup, enter the new email address (e.g., "new.name@example.com").
    * Click the "Add" button to send a confirmation email to the new address.
    * The user must confirm the new email address by following the link in the confirmation email.

    <figure><img src="../../../../.gitbook/assets/image (108).png" alt=""><figcaption></figcaption></figure>
3. **Make the New Address Primary (Optional)**:
   * Once confirmed, the new email address will appear in the list.
   * Check the "Make as primary address" box next to the new email address (e.g., "new.name@example.com") if it should replace the old address.
   * The old address (e.g., "old.name@example.com") will remain active until manually removed.
4.  **Delete the Old Email Address**:

    * Click the trash icon next to the old email address to remove it.
    * Confirm the deletion if prompted.

    <figure><img src="../../../../.gitbook/assets/image (109).png" alt=""><figcaption></figcaption></figure>
5. **Notify the User**:
   * Inform the user that emails will no longer reach the old address ("old.name@example.com") and will now be directed to the new address ("new.name@example.com").
   * We must take care to inform the employee that the old email will no longer receive any emails and that they will now go to the new address
6. **Verify**:
   * Ensure the user can log in using the new email address.
   * Confirm that emails are being received at the new address and not the old one.
   * If issues arise, verify the confirmation process and network connectivity.

{% hint style="info" %}
Ensure the new email address is owned by the user and not already associated with another Zoho Mail account.\
Coordinate with your IT admin to align with organizational email policies. \
After deleting the old address, monitor for any delivery issues and contact your IT admin if necessary.
{% endhint %}
