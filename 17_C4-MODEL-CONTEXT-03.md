# **C4 Level 3: Component Mapping**

*(For each container, what are the components inside it?)*

---

## **1. Product Intake and Lifecycle Management (Cloud Product Management CoE)**

| **Component**                            | **Purpose**                                                         |
| :--------------------------------------- | :------------------------------------------------------------------ |
| Cloud Intake Community of Practice (CoP) | Manages TAP intake, initial triage, Discovery decision-making.      |
| Discovery Management Process             | Coordinates Discovery Document production if needed.                |
| Concept Note Management Process          | Develops and approves Concept Notes.                                |
| RFC Consolidation Process                | Assembles Architecture, Security, and FinOps validations into RFCs. |
| Blueprint Management Process             | Creates Blueprints after Governance Approval.                       |
| Idea Card Preparation Process            | Prepares business-facing Idea Cards for Corporate Finance.          |

---

## **2. Architecture Governance Service (Enterprise Architecture CoE)**

| **Component**                                    | **Purpose**                                                   |
| :----------------------------------------------- | :------------------------------------------------------------ |
| Architecture Review Community of Practice (CoP)  | Conducts formal technical architecture reviews.               |
| Cloud Reference Architecture Library             | Maintains reusable architecture patterns and standards.       |
| Architecture Risk and Exception Handling Process | Reviews deviations from standards, risk acceptance processes. |

---

## **3. Security Risk and Compliance Service (Security Risk Management CoE)**

| **Component**                                            | **Purpose**                                                    |
| :------------------------------------------------------- | :------------------------------------------------------------- |
| Security Architecture Review Community of Practice (CoP) | Performs security assessments on RFCs.                         |
| Regulatory Compliance Review Unit                        | Validates HIPAA, HITRUST, internal compliance requirements.    |
| Threat Modeling Practice                                 | Conducts security threat analysis and data protection reviews. |

---

## **4. Cloud Financial Operations Service (FinOps CoE)**

| **Component**                        | **Purpose**                                                             |
| :----------------------------------- | :---------------------------------------------------------------------- |
| FinOps Community of Practice (CoP)   | Conducts cloud cost estimations and budget validations.                 |
| Spend Forecasting and Modeling Tools | Produces operational cost models.                                       |
| Optimization Recommendation Service  | Suggests reserved instances, autoscaling, cloud financial efficiencies. |

---

## **5. Governance Decision Service (Governance Board)**

| **Component**                                    | **Purpose**                                             |
| :----------------------------------------------- | :------------------------------------------------------ |
| Governance Review Council (Senior VPs, CIO, CTO) | Makes final product/service go/no-go decisions.         |
| Governance Exception Review Process              | Handles conditional approvals, exceptions, escalations. |

---

## **6. Portfolio Funding Interface (Corporate Finance/PMO)**

| **Component**              | **Purpose**                                                            |
| :------------------------- | :--------------------------------------------------------------------- |
| Idea Card Review Committee | Reviews submitted Idea Cards for prioritization and funding alignment. |
| Budget Approval Workflow   | Allocates project budgets and timelines based on approved Idea Cards.  |

---

## **7. Provisioning and Observability Enablement (Platform Engineering CoE)**

| **Component**                                    | **Purpose**                                                             |
| :----------------------------------------------- | :---------------------------------------------------------------------- |
| Platform Engineering Community of Practice (CoP) | Builds and provisions infrastructure using Terraform, Harness, Ansible. |
| Observability Integration Service                | Hooks telemetry (Cribl, Dynatrace) into deployed environments.          |
| Provisioning Automation Pipelines                | Executes infrastructure as code (IaC) automation pipelines.             |

---

## **8. Service Lifecycle Management (Service Ownership CoE)**

| **Component**                                 | **Purpose**                                                   |
| :-------------------------------------------- | :------------------------------------------------------------ |
| Service Ownership Community of Practice (CoP) | Takes operational ownership of live cloud services.           |
| SLA Management Unit                           | Tracks service level objectives, monitors KPIs.               |
| Incident and RCA Management Service           | Manages operational incidents, performs root cause analysis.  |
| Compliance Reporting Service                  | Handles audits, operational compliance reporting post-launch. |

---

# **Quick Summary Table**

| **Container**            | **Key Components**                                                                                                              |
| :----------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| Product Intake           | Cloud Intake CoP, Discovery Management, Concept Note Management, RFC Consolidation, Blueprint Management, Idea Card Preparation |
| Architecture Governance  | Architecture Review CoP, Cloud Reference Architecture Library, Risk/Exception Handling                                          |
| Security Risk Management | Security Architecture CoP, Regulatory Compliance Review, Threat Modeling                                                        |
| FinOps                   | FinOps CoP, Spend Forecasting, Optimization Service                                                                             |
| Governance Decision      | Governance Council, Exception Review Process                                                                                    |
| Portfolio Funding        | Idea Card Review Committee, Budget Approval Workflow                                                                            |
| Provisioning             | Platform Engineering CoP, Observability Integration, Automation Pipelines                                                       |
| Service Lifecycle        | Service Ownership CoP, SLA Management, Incident/RCA Management, Compliance Reporting                                            |

---

# **Important Design Pattern**

> Each **Container** contains **one or more Components** representing either:
>
> * A **Community of Practice (CoP)**
> * An **Internal Service or Workflow** supporting the business process.

This keeps the C4 modeling perfectly clean.

---

# **Next Step Options**

Now that we've mapped the Components, we can:

* **Map relationships between Components inside each Container** (optional, if you want super detailed internal views later).
* **Move forward to C4 Level 4 ("Code/Execution" layer)** — where we show the actual artifacts and work outputs moving between components (TAPs, RFCs, Blueprints, Runbooks, etc.).

