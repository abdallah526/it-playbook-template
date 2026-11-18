---
description: Instructions for adding an extension to a call queue in PBX.
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

# Add Extension To Queue

### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../logging-into-pbx-admin.md).
* An existing queue (e.g., "Support Queue").
* An existing extension (e.g., "1001").
* A web browser (e.g., Chrome, Firefox).

### Steps

1. **Access the Queues Module**:
   * Go to "PBX" > "PBX Configuration" > "Queues."
2. **Edit the Queue**:
   * Select the queue (e.g., "Support Queue").
3.  **Add the Extension**:

    * In the "Static Agents" or "Dynamic Agents" section, add the extension (e.g., "S1001").
    * Set the agent’s priority (Rank) if needed (e.g., "S1001,0").

4. **Save and Apply**:
   * Click "Submit" and then "Apply Changes" to save the configuration.

{% hint style="info" %}
Ensure the extension is logged in to the queue (see [Login to Queue](login-to-queue.md)).
{% endhint %}
