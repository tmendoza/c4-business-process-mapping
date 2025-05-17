# **C4 Level 3: Internal Component Relationships (Text Mapping)**

---

## **1. Product Intake and Lifecycle Management (Cloud Product Management CoE)**

| **From Component**              | **To Component**                | **Relationship/Interaction**                                                  |
| :------------------------------ | :------------------------------ | :---------------------------------------------------------------------------- |
| Cloud Intake CoP                | Discovery Management Process    | Initiates Discovery if needed.                                                |
| Discovery Management Process    | Concept Note Management Process | Provides findings to inform the Concept Note.                                 |
| Cloud Intake CoP                | Concept Note Management Process | Directly provides input for straightforward requests (no discovery).          |
| Concept Note Management Process | RFC Consolidation Process       | Submits validated Concept Note into RFC building.                             |
| RFC Consolidation Process       | Blueprint Management Process    | After validations are complete, transforms RFC into Blueprint.                |
| Blueprint Management Process    | Idea Card Preparation Process   | Provides technical Blueprint inputs for executive-level Idea Card formatting. |

**Pattern:**
Sequential workflow through intake, discovery (if needed), concept note, RFC, blueprint, and idea card.

---

## **2. Architecture Governance Service (Enterprise Architecture CoE)**

| **From Component**      | **To Component**                                 | **Relationship/Interaction**                                             |
| :---------------------- | :----------------------------------------------- | :----------------------------------------------------------------------- |
| Architecture Review CoP | Cloud Reference Architecture Library             | Consults standards when performing architecture reviews.                 |
| Architecture Review CoP | Architecture Risk and Exception Handling Process | Flags deviations for further review and exception approval if necessary. |

**Pattern:**
Reviews consult standards → escalate exceptions when detected.

---

## **3. Security Risk and Compliance Service (Security Risk Management CoE)**

| **From Component**        | **To Component**                  | **Relationship/Interaction**                                                                |
| :------------------------ | :-------------------------------- | :------------------------------------------------------------------------------------------ |
| Security Architecture CoP | Regulatory Compliance Review Unit | Requests compliance validation when reviewing services.                                     |
| Security Architecture CoP | Threat Modeling Practice          | Initiates threat models for services handling sensitive data or non-standard architectures. |

**Pattern:**
Security reviews branch into compliance checks and threat modeling as needed.

---

## **4. Cloud Financial Operations Service (FinOps CoE)**

| **From Component** | **To Component**                     | **Relationship/Interaction**                                                  |
| :----------------- | :----------------------------------- | :---------------------------------------------------------------------------- |
| FinOps CoP         | Spend Forecasting and Modeling Tools | Uses forecasting models to validate expected service costs.                   |
| FinOps CoP         | Optimization Recommendation Service  | Suggests cost optimization strategies during review (optional feedback loop). |

**Pattern:**
Cost estimation first → optimization feedback loop optional.

---

## **5. Governance Decision Service (Governance Board)**

| **From Component**        | **To Component**                    | **Relationship/Interaction**                                       |
| :------------------------ | :---------------------------------- | :----------------------------------------------------------------- |
| Governance Review Council | Governance Exception Review Process | If standard approval cannot be given, triggers exception handling. |

**Pattern:**
Simple approval or conditional approval branching.

---

## **6. Portfolio Funding Interface (Corporate Finance/PMO)**

| **From Component**         | **To Component**         | **Relationship/Interaction**                                    |
| :------------------------- | :----------------------- | :-------------------------------------------------------------- |
| Idea Card Review Committee | Budget Approval Workflow | Approves project funding based on prioritization of Idea Cards. |

**Pattern:**
Idea Card review first → Budget approval afterward.

---

## **7. Provisioning and Observability Enablement (Platform Engineering CoE)**

| **From Component**       | **To Component**                  | **Relationship/Interaction**                                       |
| :----------------------- | :-------------------------------- | :----------------------------------------------------------------- |
| Platform Engineering CoP | Provisioning Automation Pipelines | Executes deployments using pipelines.                              |
| Platform Engineering CoP | Observability Integration Service | Ensures all new services have telemetry and monitoring integrated. |

**Pattern:**
Deploy services → immediately integrate observability hooks.

---

## **8. Service Lifecycle Management (Service Ownership CoE)**

| **From Component**                  | **To Component**                    | **Relationship/Interaction**                                                  |
| :---------------------------------- | :---------------------------------- | :---------------------------------------------------------------------------- |
| Service Ownership CoP               | SLA Management Unit                 | Sets and monitors SLAs for all owned services.                                |
| Service Ownership CoP               | Incident and RCA Management Service | Investigates operational issues impacting services.                           |
| Incident and RCA Management Service | Compliance Reporting Service        | If RCAs reveal compliance violations, trigger compliance reporting processes. |

**Pattern:**
Normal service operations → incident handling → compliance escalations if needed.

---

# **Summary of Relationship Patterns Inside Containers**

| **Container**            | **Internal Pattern**                                                             |
| :----------------------- | :------------------------------------------------------------------------------- |
| Product Intake           | Sequential workflow (Intake → Discovery → Concept → RFC → Blueprint → Idea Card) |
| Architecture Governance  | Review standards → escalate exceptions                                           |
| Security Risk Management | Security review → compliance check and threat model if needed                    |
| FinOps                   | Cost estimation → optional optimization                                          |
| Governance Board         | Approve or escalate exception                                                    |
| Portfolio Funding        | Idea Card review → budget approval                                               |
| Provisioning             | Deployment → Observability integration                                           |
| Service Lifecycle        | Service operations → Incident/RCA → Compliance reporting if triggered            |

---

# **Big Architectural Pattern Emerging:**

> **Sequential assembly lines** inside Product Intake,
> **Validation-check branching** inside Review CoEs (Architecture, Security, FinOps),
> **Approval gates** at Governance and Portfolio stages,
> **Deployment-to-Operations transitions** post-approval.

This is extremely strong and clean from an enterprise architecture standpoint.

