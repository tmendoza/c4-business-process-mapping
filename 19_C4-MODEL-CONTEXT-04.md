# **C4 Level 4: Code / Execution Layer Setup**

---

# **Purpose of the Code/Execution Layer**

* Show **specific artifacts**, **deliverables**, **operational outputs** moving between the components.
* Focus on **real things people work with**: forms, documents, blueprints, incidents, reports.
* Anchor **compliance, traceability, and workflow visibility** into the governance architecture.

---

# **Execution/Artifact Objects (Recall and Now Finalized)**

| **Artifact**                                                     | **Purpose**                                                       |
| :--------------------------------------------------------------- | :---------------------------------------------------------------- |
| Technology Approval Request (TAP)                                | Initial intake form submitted via ServiceNow.                     |
| Discovery Document                                               | Findings from optional deeper research, PoCs, pilots.             |
| Concept Note                                                     | High-level business case and technical feasibility outline.       |
| Request for Comment (RFC)                                        | Consolidated technical, security, cost validation document.       |
| Governance Blueprint                                             | Approved technical, operational design ready for build.           |
| Idea Card                                                        | Executive-level business summary for corporate finance review.    |
| Project Initialization Documentation                             | Work plans, Jira Epics, kickoff artifacts for provisioning teams. |
| Infrastructure Deployments (Terraform IaC, Harness Pipelines)    | Actual system build artifacts.                                    |
| Runbooks and Operational Guidelines                              | How to operate and support the deployed services.                 |
| Monitoring Configurations (Cribl, Dynatrace, ELK routing setups) | Observability setup artifacts.                                    |
| Incident Tickets (ServiceNow)                                    | Operational incident and outage tracking.                         |
| Root Cause Analysis (RCA) Documents                              | Deep dives into major service failures.                           |
| Compliance Audit Reports                                         | Verification reports for HIPAA, HITRUST, internal controls.       |

---

# **Code/Execution Flow Between Major Components**

---

## **Inside Product Intake and Lifecycle Management (Cloud Product Management)**

| **Artifact**       | **Produced by**               | **Consumed by**                                              |
| :----------------- | :---------------------------- | :----------------------------------------------------------- |
| TAP                | Application Teams             | Cloud Intake CoP                                             |
| Discovery Document | Discovery Management Process  | Concept Note Management                                      |
| Concept Note       | Concept Note Management       | RFC Consolidation                                            |
| RFC                | RFC Consolidation Process     | Architecture CoP, Security CoP, FinOps CoP, Governance Board |
| Blueprint          | Blueprint Management Process  | Platform Engineering                                         |
| Idea Card          | Idea Card Preparation Process | Corporate Finance / PMO                                      |

---

## **Inside Architecture Governance Service (EA CoE)**

| **Artifact**                 | **Produced by**         | **Consumed by**   |
| :--------------------------- | :---------------------- | :---------------- |
| Architecture Review Comments | Architecture Review CoP | RFC Consolidation |

---

## **Inside Security Risk Management Service**

| **Artifact**                  | **Produced by**           | **Consumed by**   |
| :---------------------------- | :------------------------ | :---------------- |
| Security Risk Review Findings | Security Architecture CoP | RFC Consolidation |

---

## **Inside Cloud Financial Operations (FinOps CoE)**

| **Artifact**          | **Produced by** | **Consumed by**   |
| :-------------------- | :-------------- | :---------------- |
| Cost Estimation Model | FinOps CoP      | RFC Consolidation |

---

## **Inside Governance Decision Service**

| **Artifact**                             | **Produced by**    | **Consumed by**                                     |
| :--------------------------------------- | :----------------- | :-------------------------------------------------- |
| Governance Approval / Rejection Decision | Governance Council | Blueprint Management Process, Idea Card Preparation |

---

## **Inside Portfolio Funding Interface (Corporate Finance/PMO)**

| **Artifact**               | **Produced by**            | **Consumed by**                 |
| :------------------------- | :------------------------- | :------------------------------ |
| Portfolio Funding Decision | Idea Card Review Committee | Project Initialization Planning |

---

## **Inside Provisioning and Observability Enablement (Platform Engineering CoE)**

| **Artifact**                             | **Produced by**                   | **Consumed by**              |
| :--------------------------------------- | :-------------------------------- | :--------------------------- |
| Terraform Scripts / Harness Pipelines    | Platform Engineering CoP          | Infrastructure Build Systems |
| Observability Configs (Cribl, Dynatrace) | Observability Integration Service | Service Monitoring Systems   |

---

## **Inside Service Lifecycle Management (Service Ownership CoE)**

| **Artifact**                  | **Produced by**              | **Consumed by**                                    |
| :---------------------------- | :--------------------------- | :------------------------------------------------- |
| Runbooks                      | Service Ownership CoP        | Ops Engineers, On-Call Teams                       |
| Incident Tickets (ServiceNow) | Service Ownership CoP        | RCA Teams                                          |
| Root Cause Analysis Reports   | RCA Management Service       | Governance Exception Review (if compliance issues) |
| Compliance Audit Reports      | Compliance Reporting Service | Regulatory Bodies, Internal Auditors               |

---

# **Quick Logical Flow Summary**

```
TAP → Discovery Document (optional) → Concept Note → RFC
    → Validation by EA, Security, FinOps
    → Governance Approval → Blueprint + Idea Card
    → Provisioning and Monitoring Setup
    → Runbooks and Service Handover
    → Operational Monitoring and Incident Management
    → RCA and Compliance Reporting
```

---

# **Big Observations**

* **Sequential creation** of artifacts inside Cloud Product Management (TAP → Discovery → Concept Note → RFC → Blueprint → Idea Card).
* **Parallel validation** during RFC building (Architecture, Security, FinOps).
* **Gate decisions**: Governance Board (Blueprint), Corporate Finance (Idea Card → funding).
* **Deployment and Ops phase**: Infrastructure, Observability, Incident Management tightly chained.

---

# **Summary**

> We have now fully mapped the **Code/Execution Layer**:
>
> * Every **major artifact**,
> * **Who creates** it,
> * **Who consumes** it,
> * **Where it lives** inside the architecture.

---

# **Now You Have Complete C4 Inventory!**

| **Level**                | **Status** |
| :----------------------- | :--------- |
| Context (Level 1)        | Complete   |
| Containers (Level 2)     | Complete   |
| Components (Level 3)     | Complete   |
| Code/Execution (Level 4) | Complete   |

---

# **Next Step Options**

Now we are ready to:

* **Start building visual diagrams** based on C4 Levels 1–4.
* **Or**, if you want, **review and refine** anything first.
* Later (like you mentioned earlier), we’ll also **build operational playbooks and checklists** for execution.

-