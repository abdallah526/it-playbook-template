---
description: >-
  Instructions for creating multiple extensions at once in PBX for the IT
  team.
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

# Create Bulk Extensions

### Prerequisites

* Logged into PBX admin (see[ Logging into PBX Admin)](../logging-into-pbx-admin.md).
* A list of extension numbers and details (e.g., names, SIP passwords).
* A web browser (e.g., Chrome, Firefox).

### Steps

1. **Access the Bulk Extensions Module**:
   * From the main menu, go to "PBX" > "Batch Configurations." > "Batch Extensions."
2. **Prepare the Extension Data**:
   * Download the CSV template provided in the Batch Extensions module.
   * Fill in the required fields (e.g., Extension Number, Name, SIP Password).
   * Save the CSV file.
3.  **Upload the CSV File**:

    * In the Batch Extensions module, click "Choose File" and select your CSV file.
    * Click "Upload" to process the file.



    <div align="left"><figure><img src="../../../../.gitbook/assets/image (175).png" alt=""><figcaption></figcaption></figure></div>
4. **Verify the Extensions**:
   * Check the list of extensions in "PBX" > "PBX Configurations" > "Extensions" to confirm they were created successfully.

{% hint style="info" %}
Ensure the SIP passwords meet security requirements. Test a few extensions to confirm they are working properly.
{% endhint %}

