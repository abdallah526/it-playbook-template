---
description: >-
  Instructions for unlocking a user account in Active Directory to restore
  access after a lockout due to failed login attempts.
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

# Unlock User Account

### Prerequisites

* A domain controller running Active Directory.
* RSAT installed on your PC (see [Install RSAT](install-rsat/)).
* Administrative privileges on the domain controller.
* The username of the account to unlock (e.g., John Smith with logon name `extension@company.local`).

### Steps

1. **Open Active Directory Users and Computers**:
   * On your PC, open the Start menu, search for "Active Directory Users and Computers" (ADUC), and launch it.
2. **Locate the User Account**:
   * Expand your domain (e.g., company.local) and navigate to the OU containing the user (e.g., Company/HQ/Quality).
   * Find the user account (e.g., John Smith with logon name `extension@company.local`).
3. **Access Account Properties**:
   * Right-click the user account (e.g., John Smith) and select "Properties".
4.  **Unlock the Account**:

    * In the Properties window, go to the "Account" tab.
    * Under "Account options", check the "Unlock account" box to unlock the account.
    * Click "OK" to apply the changes.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (250).png" alt="" width="308"><figcaption></figcaption></figure></div>
5. **Verify the Account is Unlocked**:
   * Return to the user account in ADUC and confirm there is no lockout status.
   * Test login with the user’s credentials (e.g., `extension@company.local`) to ensure access is restored.

{% hint style="info" %}
Unlocking an account does not reset the password; ensure the user knows their current password or reset it if needed (see [Reset User Password](reset-user-password.md)). If the account locks again, review the domain’s lockout policies and investigate potential security issues (e.g., repeated failed login attempts).
{% endhint %}
