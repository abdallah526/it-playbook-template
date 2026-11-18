---
description: >-
  Instructions for retrieving and reviewing inbound call recordings using the
  PBX Reports interface in the PBX system.
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

# Inbound Calls

### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../../logging-into-pbx-admin.md).
* A web browser (e.g., Chrome, Firefox).
* Date range or specific call details (e.g., caller number or called to extension) to search for.

### Steps

1. **Navigate to Call Recordings Report**:
   * From the main menu, go to "Reports" > "PBX Reports" > "Call Recordings."
2. **Set Search Criteria**:
   * In the "Date FROM:" field, select the start date for the call records (e.g., "14-03-2025 2:53 AM").
   * In the "Date TO:" field, select the end date for the call records (e.g., "14-03-2025 2:50 AM").
   * In the "Caller No:" field, enter a caller number (e.g., "0XXXXXXXXX") or leave blank to search all.
   * In the "Called To:" field, enter the destination number or extension (e.g., "147/SIP/788") or leave blank.
   * Optionally, check "Search as Extension e.g. 532" if searching by extension.
3. **Execute the Search**:
   * Click the "Search" button to retrieve the call records.
   * Click "Reset" if you need to clear the criteria and start over.
4. **Review Call Records**:
   * Check the table for details such as "Call Date," "Caller Name," "Called To," "Call Result," "Ring Time," "Talk Time," and "Call Recording."
   * Look for specific results (e.g., "ANSWERED" in green).
5.  **Access Call Recordings**:

    * For calls with recordings, click "Listen | Download" (e.g., under "Call Recording" for any entry) to play or save the audio.


{% hint style="info" %}
Export the data by clicking "Copy" or "CSV" for detailed analysis. If no recordings appear, verify that call recording is enabled in the queue or extension settings ("PBX" > "Queues" or "Extensions") .
{% endhint %}
