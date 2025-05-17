# **Confluence Template 10: Compliance Audit Evidence Tracker**

**Template Title:**

> Compliance Audit Evidence Tracker

**Purpose:**

> Document and organize all compliance-related operational artifacts and audit evidence for cloud services — ensuring HCSC's adherence to HIPAA, HITRUST, and internal regulatory frameworks.

This tracker helps simplify **audit preparation**, **compliance reviews**, and **regulatory reporting**.

---

# **Template Structure:**

---

### Compliance Tracker Overview

* **Compliance Tracker ID:**
* **Associated Service/Product Name:**
* **Service Owner:**
* **Compliance Contact (Risk/Compliance Team SME):**
* **Date Tracker Opened:**
* **Last Review Date:**

---

### Compliance Frameworks Applied

*(Mark all that apply.)*

| **Framework**                          | **Applies?** | **Notes**                                      |
| :------------------------------------- | :----------- | :--------------------------------------------- |
| HIPAA                                  | Yes/No       | (Scope notes if partial coverage)              |
| HITRUST                                | Yes/No       | (Certification or Alignment)                   |
| PCI-DSS                                | Yes/No       | (If applicable)                                |
| SOC 2                                  | Yes/No       | (If applicable)                                |
| Internal Security Controls (Corporate) | Yes/No       | (Baseline hardening, encryption, IAM controls) |

---

### Data Handling Compliance

| **Aspect**                    | **Requirement**                           | **Status**                | **Evidence Link**           |
| :---------------------------- | :---------------------------------------- | :------------------------ | :-------------------------- |
| Data Classification Confirmed | HIPAA, HITRUST, PII                       | Compliant / Not Compliant | (Link to Blueprint section) |
| Encryption at Rest            | AES-256 minimum                           | Compliant / Not Compliant | (Link to settings, configs) |
| Encryption in Transit         | TLS 1.2+ minimum                          | Compliant / Not Compliant | (Link to certs, policies)   |
| Access Control Configured     | Role-Based Access Control (RBAC) enforced | Compliant / Not Compliant | (IAM Config Doc Link)       |
| Audit Logging Enabled         | Full access logs captured                 | Compliant / Not Compliant | (Cribl/ELK links)           |

---

### Operational Compliance

| **Aspect**                         | **Requirement**                | **Status**                | **Evidence Link**           |
| :--------------------------------- | :----------------------------- | :------------------------ | :-------------------------- |
| Backup and Restore Procedures      | DR tested annually             | Compliant / Not Compliant | (Runbook or DR test report) |
| Incident Response Process          | Documented and tested annually | Compliant / Not Compliant | (RCA Samples Link)          |
| Security Patching Policy Adherence | Updates within SLA windows     | Compliant / Not Compliant | (Patch Management Records)  |
| Quarterly Reviews Completed        | Service Reviews logged         | Compliant / Not Compliant | (Meeting Minutes Link)      |

---

### Third-Party Vendor Compliance (if applicable)

*(Complete if service integrates third-party vendors.)*

| **Vendor Name** | **Contracted Compliance Requirements** | **Evidence of Compliance**   |
| :-------------- | :------------------------------------- | :--------------------------- |
| Vendor 1        | HIPAA BAA, SOC 2 Type II               | (Link to BAA, audit reports) |
| Vendor 2        | HITRUST Certified                      | (Certification link)         |

---

### Audit History

| **Audit Type**                  | **Date**   | **Result**                | **Notes/Findings**     |
| :------------------------------ | :--------- | :------------------------ | :--------------------- |
| Internal Audit (Cloud Controls) | MM/DD/YYYY | Pass / Remediation Needed | (Link to Audit Report) |
| HIPAA Compliance Review         | MM/DD/YYYY | Pass / Remediation Needed | (Link to Assessment)   |
| HITRUST Interim Review          | MM/DD/YYYY | Pass / Remediation Needed | (Notes)                |

---

### Outstanding Compliance Actions

*(Track issues not yet fully remediated.)*

| **Issue**                                      | **Priority** | **Action Owner**     | **Target Resolution Date** |
| :--------------------------------------------- | :----------- | :------------------- | :------------------------- |
| Example: IAM role drift detected               | High         | Security Engineering | MM/DD/YYYY                 |
| Example: Backup validation failed for Region A | Medium       | Platform Engineering | MM/DD/YYYY                 |

---

### Final Compliance Certification (Annual Sign-Off)

* **Signed by Service Owner:**
* **Signed by Compliance Reviewer:**
* **Date Signed:**

---

> **\[Instruction Tip (in Confluence):]**
> *"Update this tracker quarterly, even if no audits are scheduled — ongoing compliance posture maintenance reduces risk of audit surprises."*

