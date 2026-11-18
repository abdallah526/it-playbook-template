---
description: >-
  Instructions for disabling a user account in Active Directory to prevent login
  without deleting the account.
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

# Disable User Account

### Prerequisites

* A domain controller running Active Directory.
* RSAT installed on your PC (see Install RSAT).
* Administrative privileges on the domain controller.
* The username of the account to disable.

### Steps

1. **Open Active Directory Users and Computers**:
   * On your PC, open the Start menu, search for "Active Directory Users and Computers" (ADUC), and launch it.
2. **Locate the User Account**:
   * Expand your domain (e.g., company.local) and navigate to the OU containing the user (e.g., Company/HQ/Quality).
   * Find the user account (e.g., John Smith with logon name `extension@company.local`).
3.  **Disable the Account**:

    * Right-click the user account (e.g., John Smith) and select "Disable Account."
    * Confirm the action if prompted.

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (83).png" alt="" width="323"><figcaption></figcaption></figure></div>

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (84).png" alt="" width="329"><figcaption></figcaption></figure></div>
4. **Verify the Account is Disabled**:
   * The user account icon should show a downward arrow, indicating it’s disabled.
   * Attempt to log in with the user’s credentials (e.g., `extension@company.local`) to confirm access is blocked.
5. **Move the Disable user to "De-activated Users" OU.**


{% hint style="info" %}
Disabling an account preserves its settings (e.g., profile path `\\DC1\Users Profiles$\%username%` and drive letter `M:`) for future reactivation. Document the reason for disabling in your IT records.
{% endhint %}
