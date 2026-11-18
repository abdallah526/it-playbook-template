---
description: >-
  Instructions for troubleshooting and resolving the "Incorrect Password Error"
  issue in MicroSIP.
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
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

# Incorrect Password Error

## Prerequisites

* Access to the MicroSIP softphone application.
* Admin or user access to the PBX web interface (e.g., `http://[PBX-IP]/`) for verification.
* A web browser (e.g., Chrome, Firefox).
* Extension details (e.g., extension number, SIP password, server address).

### Steps

1. **Verify Password in MicroSIP**:
   * Open MicroSIP, go to "Menu" > "Edit Account".
   * Check the "Password" field for the extension (e.g., "1001") and ensure it matches the PBX configuration.
2. **Check PBX Extension Settings**:
   * Log in to the PBX web interface (e.g., `http://[PBX-IP]/`).
   * Go to "PBX" > "Extensions," select the extension (e.g., "1001"), and verify the SIP password.
3. **Re-enter the Password**:
   * Update the password in MicroSIP if it differs from PBX.
   * Click "OK" and restart MicroSIP to apply changes.
4. **Test Registration**:
   * Check if MicroSIP registers successfully (look for a green status indicator).
   * If the error persists, note the exact error message.
5. **Reset the Password (if needed)**:
   * In PBX, edit the extension and generate a new SIP password.
   * Update MicroSIP with the new password and test again.
