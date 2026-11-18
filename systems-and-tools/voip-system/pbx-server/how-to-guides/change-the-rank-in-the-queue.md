---
description: Instructions for adjusting an agent’s rank in a call queue in PBX.
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

# Change the Rank in the Queue

### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../logging-into-pbx-admin.md).
* An existing queue with agents (e.g., "Support Queue").
* A web browser (e.g., Chrome, Firefox).

### Steps

1. **Access the Queues Module**:
   * Go to "PBX" > "PBX Configuration" > "Queues."
2. **Edit the Queue**:
   * Select the queue (e.g., "Support Queue").
3.  **Change the Agent Rank**:

    * In the "Static Agents" or "Dynamic Agents" section, find the agent’s extension.
    * Adjust the rank/priority number after comma (e.g., S675,0 - set to "0" for highest priority).

4. **Save and Apply**:
   * Click "Submit" and then "Apply Changes" to save the configuration.

{% hint style="info" %}
Test the queue to ensure calls are distributed according to the new rank.
{% endhint %}
