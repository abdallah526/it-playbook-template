---
description: >-
  This guide explains how to configure an SD-WAN route in Sophos Central to
  direct traffic for a specific website (e.g., Google) through a designated
  gateway (e.g., Branch D or Branch C).
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

# Route Website from Specific gateway

### Prerequisites

* Access to the Sophos Firewall web admin console.
* Sophos firewall credentials, provided by the IT admin via Keeper Security.
* A web browser (e.g., Chrome, Firefox).
* Knowledge of the website to route (e.g., Google) and the preferred gateway (e.g., Branch D).

### Steps

1. **Log in to Sophos Firewall**:
   * Open a web browser and navigate to the Sophos Firewall IP address (retrieve the IP from Keeper Security).
   * Log in using the administrative credentials provided by the IT admin.
2.  **Navigate to SD-WAN Routes**:

    * From the Sophos Firewall dashboard Click **Routing** to access routing settings.
    * Select the **SD-WAN routes** tab.

3. **Add a New SD-WAN Route**:
   * Click **Add** to create a new SD-WAN route.
   * In the **Name** field, enter a descriptive name for the route (e.g., "Google").
   * In the **Description** field, provide a brief description (e.g., "Route Google from Branch Gateways").
   * In the **Route position** dropdown, select **Top** to prioritize this route.
4. **Configure Traffic Selector**:
   * Under **Source networks**, leave the default as **Any** or specify a source network if needed (e.g., PC107)
   * Under **Destination networks**, click **Add new item** and enter the website domain (e.g., "Google").
   * Under **Services**, leave the default as **Any service**.
   * Under **Application object**, leave the default as **Any application**.
5.  **Set Link Selection Settings**:

    * Under **Link selection settings**, select **Primary and Backup gateways**.
    * In the **Primary gateway** dropdown, select the preferred gateway (e.g., "Branch D").
    * In the **Backup gateway** dropdown, select a backup gateway (e.g., "Branch C").
    * Check the box for **Route only through specified gateways**.

    <figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
6.  **Save the Route**:

    * Click **Save** to apply the new SD-WAN route.
    * Verify the route appears in the SD-WAN routes list (e.g., "Google" with ID #3).


{% hint style="info" %}
Ensure the selected gateways (e.g., Branch D, Branch C) are online and operational before configuring the route. Monitor the route’s performance to confirm traffic is directed as expected.
{% endhint %}
