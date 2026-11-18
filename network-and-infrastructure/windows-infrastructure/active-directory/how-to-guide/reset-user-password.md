---
description: >-
  Instructions for resetting a user’s password in Active Directory to restore
  access.
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

# Reset User Password

### Prerequisites

* A domain controller running Active Directory.
* RSAT installed on your PC (see Install RSAT).
* Administrative privileges on the domain controller.
* The username of the account to reset.

### Steps

1. **Open Active Directory Users and Computers**:
   * On your PC, open the Start menu, search for "Active Directory Users and Computers" (ADUC), and launch it.
2. **Locate the User Account**:
   * Expand your domain (e.g., company.local) and navigate to the OU containing the user (e.g., Company/HQ/Quality).
   * Find the user account (e.g., John Smith with logon name `extension@company.local`).
3.  **Reset the Password**:

    * Right-click the user account (e.g., John Smith) and select "Reset Password...".

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (86).png" alt="" width="317"><figcaption></figcaption></figure></div>
4.  **Enter New Password Details**:

    * In the "Reset Password" window, enter the default password in the "New password" field  <mark style="color:red;">**(the default password stored in the password manager)**</mark>.
    * Confirm the new password in the "Confirm password" field.
    * Check "User must change password at next logon" if required.
    * Check "Unlock the user's account" if the account is locked.
    * Click "OK" to apply the changes.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (87).png" alt="" width="412"><figcaption></figcaption></figure></div>
5.  **Verify the Password Reset**:

    * A confirmation message will appear (e.g., "The password for John Smith has been changed") with an "OK" button.
    * Click "OK" to close the confirmation.
    * Test the login with the new password to ensure access is restored.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (88).png" alt="" width="397"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Ensure the new password meets domain security policies. Document the reset action and reason in your IT records. If the user cannot log in after the reset, verify the "User must change password at next logon" setting and network connectivity.
{% endhint %}
