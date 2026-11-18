---
description: >-
  This guide explains how to use the Log Viewer in Sophos Firewall to monitor
  and troubleshoot network events in real-time.
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

# Use Log Viewer

### Prerequisites

* Access to the Sophos Firewall web admin console.
* Administrative credentials for Sophos Firewall, provided by the IT admin via Keeper Security.
* A PC with a web browser (e.g., Chrome, Firefox).
* The screenshot of the Log Viewer showing columns like Time, Firewall rule name, NAT rule, In interface, Out interface, Src IP, Dst IP, Src port, Dst port, and Active threat response.

### Steps

1. **Log in to Sophos Firewall**:
   * Open a web browser and navigate to the Sophos Firewall IP address (retrieve the IP from Keeper Security).
   * Log in using the administrative credentials provided by the IT admin.
2.  **Access the Log Viewer**:

    * From the Sophos Firewall dashboard, navigate to the  **Log Viewer** section&#x20;

    <figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

3. **Understand the Log Columns**:
   * Review the log entries with several columns like:
     * **Time**: Timestamp of the event (e.g., 2025-03-19 08:49:14).
     * **Firewall rule name**: Name of the firewall rule (e.g., "Rule," "RED to LAN").
     * **NAT rule**: Associated NAT rule number (e.g., 0).
     * **In interface**: Incoming interface (e.g., redS17, PCs by Users).
     * **Out interface**: Outgoing interface (e.g., Port110, Port160).
     * **Src IP**: Source IP address (e.g., 172.20.11.26, 172.20.11.141).
     * **Dst IP**: Destination IP address (e.g., 172.20.31.30, 142.250.190.78).
     * **Src port**: Source port number (e.g., 56750).
     * **Dst port**: Destination port number (e.g., 443).
     * **Active threat response**: Security actions (e.g., Application filter, IPS, Zero-day protection).
4. **Filter Logs for Specific Events**:
   * Click **Add filter** (as shown in the screenshot) to apply filters.
   * Select a field (e.g., Dst IP, Firewall rule name) and set a condition (e.g., "is," "contains") with a value (e.g., "172.20.31.30" or "Denied").
   * Example: Filter for denied connections by setting "Firewall rule name" to "Denied" to highlight blocked traffic like those from user@example.com.
5. **Analyze Log Entries**:
   * Identify patterns or issues, such as repeated "Denied" entries (e.g., multiple denials from 172.20.11.141 to 142.250.190.78 on port 443), indicating potential blocked access.
6. **Export Logs (Optional)**:
   * If needed, export the logs for further analysis by clicking **Export** or **Download Logs** (available in the Log Viewer interface).
   * Save the logs in a secure location for documentation or escalation.
