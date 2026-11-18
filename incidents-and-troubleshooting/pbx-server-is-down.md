---
description: >-
  This guide outlines the steps to troubleshoot an PBX server outage (e.g.,
  "This site can’t be reached" error) between head office and Branch A branches.
icon: phone-slash
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

# PBX Server is Down

<div align="left"><figure><img src="../.gitbook/assets/image (286).png" alt="" width="563"><figcaption></figcaption></figure></div>

### Steps

1. **Verify Red VPN Between head office and Branch A**
   * Check if the Red VPN between head office and Branch A is operational.
   * Notify IT Admin and IT Manager of the issue immediately.
2. **Check Internet in Branch A if Red VPN is Down**
   * If Red VPN is down, verify if the internet in Branch A is working.
   * If the internet is down, follow: the internet outage runbook until resolved.
3. **Troubleshoot Server if Internet and Red VPN are Up**
   * If both internet and Red VPN are working, the issue is likely with the PBX server.
   * Perform a ping test to the PBX server from Branch A (from the firewall and an employee’s device).
   * See [Ping From Gateway](../network-and-infrastructure/sophos-firewall/how-to-guides/ping-from-gateway.md)
4. **Escalate Based on Ping Results**
   * **If ping fails**: Notify the IT Admin to coordinate with someone in Branch A to check the PBX server hardware or configuration.
   * **If ping succeeds**: The issue may be with the Red VPN connection or a misconfiguration between head office and Branch A.
     * Restart the Red VPN between head office and Branch A as an initial fix See ([Restart RED VPN](../network-and-infrastructure/sophos-firewall/how-to-guides/restart-red-connection.md)).
     * Investigate potential configuration issues (e.g., someone altered settings).
5. **Monitor and Resolve**
   * Follow up quickly until the PBX server is fully operational.

{% hint style="info" %}
Prioritize resolution to minimize downtime. Document all steps and findings in the team documentation for future reference.
{% endhint %}
