# **Cloud Product Governance and Operations: Execution Checklists**

---

## **1. TAP Request Submission Checklist**

*(For Application Teams submitting a TAP)*

| **Item**                                        | **Status** |
| :---------------------------------------------- | :--------- |
| TAP Title is clear and business-readable        |            |
| Business Driver field is completed              |            |
| Sponsoring Business Unit identified             |            |
| Primary and secondary contacts listed           |            |
| Cloud deployment type selected (IaaS/PaaS/SaaS) |            |
| Target cloud provider selected (AWS/Azure/GCP)  |            |
| Data sensitivity level classified               |            |
| Time sensitivity noted (if applicable)          |            |
| Special compliance needs noted (if any)         |            |
| Supporting documentation attached (optional)    |            |
| TAP successfully submitted in ServiceNow        |            |
| TAP ID captured for tracking                    |            |

---

## **2. Intake Triage and Validation Checklist**

*(For Cloud Product Management reviewing TAPs)*

| **Item**                                          | **Status** |
| :------------------------------------------------ | :--------- |
| TAP completeness reviewed                         |            |
| Scope and eligibility validated                   |            |
| Data sensitivity classification validated         |            |
| Discovery need evaluated (Yes/No)                 |            |
| Triage decision made (Advance, Discovery, Reject) |            |
| TAP status updated in ServiceNow                  |            |
| Discovery Work Item created if needed             |            |

---

## **3. Discovery Execution Checklist**

*(For Discovery Leads coordinating Discovery)*

| **Item**                                                              | **Status** |
| :-------------------------------------------------------------------- | :--------- |
| Discovery scope defined (objectives, boundaries)                      |            |
| Discovery team (SMEs) assigned                                        |            |
| Discovery activities planned (PoC, PoV, vendor demos, risk workshops) |            |
| Discovery activities executed                                         |            |
| Discovery findings documented                                         |            |
| Discovery recommendation (proceed, caution, reject) made              |            |
| Discovery Document finalized and linked to TAP                        |            |
| Stakeholders notified of Discovery outcome                            |            |

---

## **4. Concept Note Development Checklist**

*(For Cloud Product Management creating Concept Notes)*

| **Item**                                     | **Status** |
| :------------------------------------------- | :--------- |
| Executive summary completed                  |            |
| Business drivers documented                  |            |
| Target cloud model and provider specified    |            |
| Data sensitivity level identified            |            |
| Initial cost and timeline estimates included |            |
| Technical integration points outlined        |            |
| Risks and open questions listed              |            |
| TAP and Discovery Documents referenced       |            |
| Internal SME review completed                |            |
| Concept Note linked to TAP in ServiceNow     |            |

---

## **5. RFC Development Checklist**

*(For RFC Owners building full governance packets)*

| **Item**                                                     | **Status** |
| :----------------------------------------------------------- | :--------- |
| Executive Summary populated                                  |            |
| Business Context section completed                           |            |
| Technical Architecture section drafted                       |            |
| Security and Compliance findings incorporated                |            |
| Financial analysis validated by FinOps SME                   |            |
| Operational considerations (monitoring, ownership) addressed |            |
| Risk and mitigation strategies documented                    |            |
| Discovery summary (if applicable) linked                     |            |
| TAP and Concept Note cross-referenced                        |            |
| RFC internally reviewed and finalized                        |            |
| RFC status updated as "Ready for Governance" in ServiceNow   |            |

---

## **6. Governance Review Preparation Checklist**

*(For Governance Review readiness)*

| **Item**                                                              | **Status** |
| :-------------------------------------------------------------------- | :--------- |
| RFC posted to Governance Confluence space (5 days before meeting)     |            |
| Governance meeting scheduled                                          |            |
| Governance pre-read summary email sent                                |            |
| SMEs ready for Q\&A support                                           |            |
| Governance Board members invited                                      |            |
| Governance Decision recorded (Approve/Approve with Conditions/Reject) |            |
| Decision documented in ServiceNow linked to TAP                       |            |

---

## **7. Infrastructure Provisioning Checklist**

*(For Platform Engineering post-approval)*

| **Item**                                      | **Status** |
| :-------------------------------------------- | :--------- |
| Final Blueprint reviewed and signed off       |            |
| Terraform modules authored/updated            |            |
| Harness pipelines created/updated             |            |
| Infrastructure provisioned in target cloud(s) |            |
| Dynatrace monitoring agents deployed          |            |
| Cribl telemetry configured                    |            |
| Backup/DR policies applied                    |            |
| Final architecture diagram produced           |            |
| Infrastructure health validated               |            |
| Service marked ready for operational handoff  |            |

---

## **8. Operational Handoff Checklist**

*(For Handoff Review Meetings)*

| **Item**                                                  | **Status** |
| :-------------------------------------------------------- | :--------- |
| Runbooks completed and linked                             |            |
| Monitoring/alerting active                                |            |
| Backup/DR policies documented and validated               |            |
| Security guardrails verified                              |            |
| SLA/SLO draft targets defined                             |            |
| Handoff review meeting held                               |            |
| Service ownership formally accepted (or gap plan created) |            |
| ServiceNow/Service Catalog updated                        |            |

---

## **9. Service Lifecycle Management Checklist**

*(For Ongoing Service Ownership)*

| **Item**                                      | **Status** |
| :-------------------------------------------- | :--------- |
| Daily health monitoring active (Dynatrace)    |            |
| Incident response procedures in place         |            |
| RCA performed for Severity 1/2 incidents      |            |
| Compliance audit evidence collected quarterly |            |
| SLA/SLO reviews conducted quarterly           |            |
| Enhancement backlog updated regularly         |            |
| Service Retirement Plans created if needed    |            |

---

# **Summary**

> **Each governance phase now has an exact, operational checklist.**
> These will ensure:
>
> * **Execution consistency**
> * **Audit readiness**
> * **Clear quality gates between stages**

