---
description: >-
  Instructions for creating a new user account in Active Directory using Active
  Directory Users and Computers (ADUC).
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

# Create User Account

### Prerequisites

* A domain controller running Active Directory.
* RSAT installed on your PC (see [Install RSAT](install-rsat/)).
* Administrative privileges on the domain controller.
* User details (e.g., full name, username, initial password).

### Steps

1. Log in to the Active Directory Users and Computers tool.
2.  Right-click on the "OU" and select "New", then choose "User".<br>

    <figure><img src="../../../../.gitbook/assets/image (78).png" alt=""><figcaption></figcaption></figure>
3. In the "New Object - User" window, enter the first name (e.g., John), last name (e.g., Smith), and full name will auto-populate .
4. Enter the user logon name as <mark style="color:red;">**`extension@company.local`**</mark> (e.g., 658@company.local).
5.  Enter the user logon name (pre-Windows 2000) as the full name (e.g., John Smith), then click "Next".

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (79).png" alt="" width="465"><figcaption></figcaption></figure></div>
6. In the password setup window, enter and confirm the default password as **(the default password stored in the password manager)**).
7.  Uncheck "User must change password at next logon" and check "Password never expires", then click "Next" .<br>

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (80).png" alt="" width="440"><figcaption></figcaption></figure></div>
8. After creation user, In the user properties, go to the "Profile" tab.
9.  Set the home folder to "Connect" with drive letter `M:` and \
    path `\\DC1\Users Profiles$\%username%` , then click "OK" .



    <div align="left"><figure><img src="../../../../.gitbook/assets/image (81).png" alt="" width="404"><figcaption></figcaption></figure></div>
10. Right Click on the User then click "Add to Group"
11. Type group name then click "Check Names"
12. Click "OK"

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (82).png" alt="" width="523"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Ensure the profile path and drive letter are correctly configured to avoid access issues. Coordinate with your IT admin if the user cannot log in or if the profile does not load. Verify network share permissions if the home folder connection fails.
{% endhint %}
