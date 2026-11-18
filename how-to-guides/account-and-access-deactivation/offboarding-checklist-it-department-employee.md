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

# Offboarding Checklist – IT Department Employee

### **Privileged Access Removal**

* Disable any elevated AD roles assigned to the user
* Remove the user from any admin groups
* Disable access to the ERP system with admin or power-user privileges
* Disable PBX admin access
* Disable access to the Google/Zoho admin console
* Ensure RADIUS does not include any privileged WiFi/VLAN profiles tied to the user

### **Email & Communication**

* Disable email access (Google Workspace / Zoho)
* Reset password immediately after disabling
* Review email filters for suspicious forwarding rules (IT users only)

### **Internal Systems**

* Remove access from:
  * Documentation and task tools
  * Any internal dashboards or management portals
* Transfer ownership of their documents and projects

### **Security Audit**

* Review the user's activities for the last 30–60 days in:
  * AD logs
  * ERP system logs
  * PBX call logs (optional)
* Confirm no test accounts or temporary accounts were created
* Remove the user from any documentation or admin lists
