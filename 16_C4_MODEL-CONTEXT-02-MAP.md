# **C4 Level 2: Container Relationship Mapping**

*(Text Version — Logical Structure Before Drawing)*

---

# **Primary Containers** *(recap)*

```
1. Product Intake and Lifecycle Management (Cloud Product Management)
2. Architecture Governance Service (Enterprise Architecture)
3. Security Risk and Compliance Service (Security Risk Management)
4. Cloud Financial Operations Service (FinOps)
5. Governance Decision Service (Governance Board)
6. Portfolio Funding Interface (Corporate Finance/PMO)
7. Provisioning and Observability Enablement (Platform Engineering)
8. Service Lifecycle Management (Service Ownership)
```

---

# **Key Relationships (Flows)**

---

## **1. Product Intake and Lifecycle Management → Architecture Governance Service**

* **Purpose:**
  Submit initial service concepts and RFCs for architectural validation.

* **Artifact Flow:**
  Concept Note → Architecture Review Comments → RFC

---

## **2. Product Intake and Lifecycle Management → Security Risk and Compliance Service**

* **Purpose:**
  Submit initial service designs and RFCs for security, compliance risk evaluation.

* **Artifact Flow:**
  Concept Note → Security Review Comments → RFC

---

## **3. Product Intake and Lifecycle Management → Cloud Financial Operations Service**

* **Purpose:**
  Submit estimated architecture/service usage for cloud cost estimation and budget validation.

* **Artifact Flow:**
  Concept Note → Cost Estimation Analysis → RFC

---

## **4. Architecture Governance Service → Product Intake and Lifecycle Management**

* **Purpose:**
  Return architecture validation outputs (pass, minor adjustments, risks).

* **Artifact Flow:**
  Architecture Review Outcomes → RFC Update

---

## **5. Security Risk and Compliance Service → Product Intake and Lifecycle Management**

* **Purpose:**
  Return risk findings, compliance check outcomes.

* **Artifact Flow:**
  Security Risk Findings → RFC Update

---

## **6. Cloud Financial Operations Service → Product Intake and Lifecycle Management**

* **Purpose:**
  Return cost model validation, financial feasibility findings.

* **Artifact Flow:**
  Cost Review Outcomes → RFC Update

---

## **7. Product Intake and Lifecycle Management → Governance Decision Service**

* **Purpose:**
  Submit the finalized RFC for governance gate decision-making.

* **Artifact Flow:**
  Final RFC Submission

---

## **8. Governance Decision Service → Product Intake and Lifecycle Management**

* **Purpose:**
  Return governance decision (Approve / Approve with Conditions / Reject).

* **Artifact Flow:**
  Governance Decision Outcome → Blueprint Creation

---

## **9. Product Intake and Lifecycle Management → Portfolio Funding Interface (Corporate Finance/PMO)**

* **Purpose:**
  Submit Idea Card (business-facing summary) for funding prioritization.

* **Artifact Flow:**
  Idea Card Submission

---

## **10. Portfolio Funding Interface → Product Intake and Lifecycle Management**

* **Purpose:**
  Return funding approval or deferment outcome.

* **Artifact Flow:**
  Funding Decision (Approve/Defer/Reject)

---

## **11. Product Intake and Lifecycle Management → Provisioning and Observability Enablement**

* **Purpose:**
  After governance and funding approvals, hand off Blueprint for technical execution.

* **Artifact Flow:**
  Blueprint Handoff + Build Requirements

---

## **12. Provisioning and Observability Enablement → Service Lifecycle Management**

* **Purpose:**
  Upon deployment completion, transfer operational ownership of the new cloud service.

* **Artifact Flow:**
  Operational Handoff (Runbooks, Observability Integrations, SLA Tracking)

---

## **13. Service Lifecycle Management → Platform Engineering (Ongoing)**

* **Purpose:**
  Continuous collaboration on incidents, RCA findings, monitoring adjustments as services operate.

* **Artifact Flow:**
  Incident Tickets → Infrastructure Adjustments → Compliance Audit Feedback

---

# **Optional/Secondary Flows**

| **From**                                                   | **To**                                                                                   | **Reason** |
| :--------------------------------------------------------- | :--------------------------------------------------------------------------------------- | :--------- |
| Governance Decision Service → Portfolio Funding Interface  | Notify corporate finance teams about newly approved services needing funding visibility. |            |
| Service Lifecycle Management → Governance Decision Service | Request re-review if major incidents or compliance failures surface post-launch.         |            |

---

# **Quick Logical Flow Summary (Simple)**

```
Intake (Cloud Product Mgmt)
    ↓
Validation (Architecture, Security, FinOps)
    ↓
Governance Decision
    ↓
Funding Decision (Idea Card)
    ↓
Provisioning and Deployment
    ↓
Operational Lifecycle Management
```

---

# **Summary**

> **We now have a full logical relationship map** between the containers — describing **who talks to whom, why, and what artifacts flow** between them — **without yet needing to draw anything**.

