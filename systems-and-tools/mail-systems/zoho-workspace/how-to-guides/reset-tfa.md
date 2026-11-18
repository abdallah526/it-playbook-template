---
description: >-
  Instructions for resetting Two-Factor Authentication (TFA) for a user in Zoho
  Workspace.
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

# Reset TFA

### Prerequisites

* Admin access to the Zoho Mail Admin console.
* The user’s email address with TFA enabled.
* A web browser (e.g., Chrome, Firefox).

### Steps

1. **Navigate to Users in Zoho Mail Admin Panel**:
   * Log in to the Zoho Mail admin panel.
   * In the left sidebar, click on "Users" to view the list of users.
   * Locate the user whose TFA needs to be reset (e.g., "John Smith").
2.  **Access the User’s TFA Settings**:

    * Click the three-dot menu ("More Actions") next to the user’s name.
    * From the dropdown, select "Change TFA status" to open the TFA settings.

3.  **Reset TFA**:

    * In the user’s settings, navigate to the "Security" section.
    * Expand the "TFA" subsection to view the Two-Factor Authentication settings.
    * Click the "Reset TFA" button to reset the user’s TFA configuration.
    * Confirm the action if prompted (e.g., a confirmation dialog may appear).

    <figure><img src="../../../../.gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>
4. **Verify**:
   * Notify the user to log in to Zoho Mail.
   * The user will be prompted to set up TFA again during their next login.
   * Ensure the user can successfully configure TFA (e.g., using a mobile app or SMS).

{% hint style="info" %}
Ensure the user has access to a supported TFA method (e.g., a mobile device for an authenticator app or SMS). Contact your IT admin if the TFA reset fails or if the user encounters persistent issues.
{% endhint %}
