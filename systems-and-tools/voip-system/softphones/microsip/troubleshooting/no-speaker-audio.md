---
description: >-
  Instructions for troubleshooting and resolving the "No Speaker Audio" issue in
  MicroSIP.
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

# No Speaker Audio

### Prerequisites

* Access to the MicroSIP softphone application.
* Admin or user access to the PBX web interface (e.g., `http://[PBX-IP]/`) for verification.
* A web browser (e.g., Chrome, Firefox) and speakers or headphones connected to the computer.
* Extension details (e.g., extension number, SIP server address).

### Steps

1. **Check Speaker Connection**:
   * Ensure the speakers or headphones are plugged in and powered on.
   * Verify they are recognized by the computer (check system sound settings).
2. **Verify MicroSIP Audio Settings**:
   * Open MicroSIP, go to "Menu" > "Settings".
   * Select the correct speaker or headphone device from the "Speaker" dropdown.
3. **Adjust Volume Levels**:
   * Increase the speaker volume in MicroSIP settings and the computer’s sound control panel.
   * Ensure no mute settings are enabled.
4. **Test the Call**:
   * Make a test call within MicroSIP (e.g., to another extension).
   * Confirm you can hear the recipient’s voice.
