---
description: Instructions for creating a call queue in PBX to manage incoming calls.
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

# Create Queue

### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../logging-into-pbx-admin.md).
* A unique queue number and password.
* A web browser (e.g., Chrome, Firefox).

### Steps

1. **Navigate to the Queues Module**:
   * From the main menu, go to "PBX" > "PBX Configuration" > "Queues."
2. **Add a New Queue**:
   * Click the "Add Queue" button.
3. **Configure Basic Queue Settings**:
   * In the "Queue Number:" field, enter a unique number (e.g., "600-Support").
   * In the "Queue Password:" field, enter a secure password (optional, for agent login).
   * In the "CID Name Prefix:" field, enter a prefix (e.g., "Support") to identify calls from this queue.
4. **Set Timing and Agent Options**:
   * In the "Max Wait Time:" field, select "Unlimited" or set a specific time limit.
   * In the "Agent Timeout:" field, set the time (e.g., "15 seconds") before an agent call times out.
   * In the "Agent Timeout Restart:" field, select "No" or set to "Yes" if restarting the timeout is needed.
5.  **Configure Advanced Queue Options**:

    * In the "Ring Strategy:" field, select a strategy (e.g., "ringall" to ring all agents simultaneously).
    * In the "Dynamic Agents:" field, add extension numbers with rank after comma (e.g., "S1001,0") .



    <figure><img src="../../../../.gitbook/assets/image (179).png" alt=""><figcaption></figcaption></figure>
6. **Set Failover and Continuation Destinations**:
   * In the "Fail Over Destination:" field, select a destination (e.g., "Voicemail" or another queue) if no agents are available.
   * In the "Queue Continue Destination:" field, select a destination for calls to continue to after the queue.
7.  **Save and Apply Changes**:

    * Click the "Submit Changes" button.
    * Click "Apply Config" (if prompted) to activate the new queue.



    <figure><img src="../../../../.gitbook/assets/image (180).png" alt=""><figcaption></figcaption></figure>

    <div align="left"><figure><img src="../../../../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure></div>
8. **Verify the Queue**:
   * Return to "PBX" > "PBX Configuration" > "Queues." and confirm the new queue (e.g., "600-Support") appears in the list.
   * Test by calling the queue number to ensure it rings agents.

{% hint style="info" %}
Test the queue with a live call to verify the ring strategy and timeout settings. If issues occur, check the PBX logs ("Reports" > "Asterisk Logs") or ensure extensions are registered ("PBX" > "Extensions").
{% endhint %}
