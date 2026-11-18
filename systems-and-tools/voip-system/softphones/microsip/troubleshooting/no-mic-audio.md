---
description: >-
  Instructions for troubleshooting and resolving the "No Mic Audio" issue in
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

# No Mic audio

### Prerequisites

* Access to the MicroSIP softphone application.
* Admin or user access to the PBX web interface (e.g., `http://[PBX-IP]/`) for verification.
* A web browser (e.g., Chrome, Firefox) and a microphone connected to the computer.
* Extension details (e.g., extension number, SIP server address).

### Steps

1. **Check Microphone Connection**:
   * Ensure the microphone is plugged in and recognized by the computer (check system sound settings).
2. **Verify MicroSIP Audio Settings**:
   * Open MicroSIP, go to "Menu" > "Settings".
   * Select the correct microphone from the "Microphone" dropdown.
3. **Adjust Volume Levels**:
   * Increase the microphone volume in MicroSIP settings and the computer’s sound control panel.
   * Ensure no mute settings are enabled.
4. **Test the Call**:
   * Make a test call within MicroSIP (e.g., to another extension).
   * Ask the recipient to confirm if they hear your voice.

{% hint style="info" %}
If the issue persists, check for driver updates for the microphone or contact the system admin to verify SIP codec compatibility (e.g., G.711 or G.729).
{% endhint %}
