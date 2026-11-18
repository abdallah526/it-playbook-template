---
description: >-
  Instructions for retrieving and reviewing outbound call records using the
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

# Outbound Calls

### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../../logging-into-pbx-admin.md).
* A web browser (e.g., Chrome, Firefox).
* Date range or specific call details (e.g., source or destination) to search for.

### Steps

1. **Navigate to Outbound Calls Report**:
   * From the main menu, go to "Reports" > "PBX Reports" > "Outbound Calls."
2. **Set Search Criteria**:
   * In the "Date FROM:" field, select the start date for the call records (e.g., "14-03-2025 2:51 AM").
   * In the "Date TO:" field, select the end date for the call records (e.g., "14-03-2025 4:38 AM").
   * In the "Source:" dropdown, select an employee or leave as "Select Employee" to include all sources.
   * In the "Destination:" field, enter a phone number (e.g., "0XXXXXXXXX") or leave blank to search all.
3. **Execute the Search**:
   * Click the "Search" button to retrieve the call records.
   * Click "Reset" if you need to clear the criteria and start over.
4. **Review Call Records**:
   * Check the table for details such as "Call Date," "Agent Name," "Called To," "Call Result," "Ring Time," "Talk Time," and "Call Recording."
   * Look for specific results (e.g., "ANSWERED" in green, "NO ANSWER-Cancelled" in blue).
5.  **Access Call Recordings**:

    * For calls with recordings, click "Listen | Download" (e.g., under "Call Recording" for the second entry) to play or save the audio.


{% hint style="info" %}
Export the data by clicking "Export Excel" for detailed analysis.
{% endhint %}
