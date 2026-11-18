---
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

# Offboarding Checklist – Standard Employee

### **Account Deactivation**

* Disable user in Active Directory
* Remove user from all AD security groups.
* Move user to Deactivated security group.
* Disable WiFi authentication (RADIUS).
* Disable user account in ERP system (ERP/CRM).
* Change PBX Extension password.
* Disable email account (Google Workspace / Zoho).

### **Security Actions**

* Reset the AD password after disabling.
* Reset the Google / Zoho password after disabling.
* Review last login from AD & ERP system (optional check).

### **Data & Access Cleanup**

* Remove user access from shared folders.
* Transfer ownership of email (forwarding or delegation).
* Backup important work files before device wipe (if needed).

