---
description: >-
  This guide explains how to make outbound calls using different routing keys
  based on the telecom provider.
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

# Make Outbound Calls (Trunks)

### Call Routing Keys

Use the following keys to route your outbound calls through the correct provider:

***

#### Landline (PSTN)

**Routing Key:** `22`\
**Route:** Landline (PSTN)

**Dial format:**

* Start the number with `22`
* Then add `0` before the phone number

**Example:** `220XXXXXXXXX`

***

#### Mobile SIM Gateway

**Routing Key:** `88`\
**Route:** Mobile SIM gateway

**Dial format:**

* Start the number with `88`
* Then add `0` before the phone number

**Example:** `880XXXXXXXXX`

***

#### SIP Trunk

**Routing Key:** `66`\
**Route:** SIP Trunk

**Dial format:**

* Start the number with `66`
* Do NOT add `0` before the phone number

**Example:** `66XXXXXXXXX`

***

### Important Notes

* Always dial the **routing key first**
* Follow the correct format based on the provider
* Calling with wrong format may result in:
  * Call failure
  * Wrong route selection
  * Higher call cost
