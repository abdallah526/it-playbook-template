---
description: Instructions for resetting a user’s email password in Zoho Workspace.
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

# Reset Email Password

### Prerequisites

* Admin access to the Zoho Mail Admin console.
* The user’s email address (e.g., user@yourcompany.com).
* A web browser (e.g., Chrome, Firefox).

### Steps

1. **Navigate to Users in Zoho Mail Admin Panel**:
   * Log in to the Zoho Mail admin panel.
   * In the left sidebar, click on "Users" to view the list of users.
   * Locate the user whose password needs to be reset (e.g., "John Smith").
2.  **Access the User’s Password Settings**:

    * Click the three-dot menu ("More Actions") next to the user’s name.
    * From the dropdown, select "Change password" to open the password reset settings.

3. **Reset the Password**:
   * In the "Change password" section, enter the new password:
     * **New password**: Enter the fixed password designated for the user.
   * Check the following options:
     * **Force user to change password on first log in**: Enable to require the user to set a new password upon login.
     * **Sign out from all devices (Recommended)**: Enable to log the user out of all active sessions for security.
4.  **Apply the New Password**:

    * Click the "Change" button to apply the new password (8).
    * Confirm the password update is successful (e.g., a confirmation message may appear).

    <figure><img src="../../../../.gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>
5. **Verify**:
   * Notify the user to log in with the new password.
   * If "Force user to change password on first log in" was enabled, ensure the user can change their password successfully.

{% hint style="info" %}
If "Sign out from all devices" is enabled, inform the user they will need to log in again on all devices. Contact your IT admin if the password reset fails.
{% endhint %}
