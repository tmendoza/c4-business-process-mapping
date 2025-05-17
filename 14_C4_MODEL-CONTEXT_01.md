# **C4 Level 1: Context Diagram Setup for Cloud Product Governance**

---

# **Purpose of this Diagram**

* Show the **major organizational actors** (teams, business units, governance boards).
* Show the **main system** they are interacting with: the **Cloud Product Governance Framework**.
* Show **external dependencies** (only lightly — vendors, cloud providers).
* Show **relationships**: "who initiates, who governs, who operates" — but **high level only**.

---

# **Primary System in the Center**

| **System Being Modeled**                                          |
| :---------------------------------------------------------------- |
| **HCSC Cloud Product Governance and Service Lifecycle Framework** |

---

# **Primary Actors Around the System**

| **Actor**                                          | **Role/Relationship**                                                    |
| :------------------------------------------------- | :----------------------------------------------------------------------- |
| **Application Teams (Business Units, Developers)** | Submit service requests, consume approved cloud products.                |
| **Cloud Product Management CoE**                   | Owns intake, triage, product definition, lifecycle governance.           |
| **Enterprise Architecture CoE**                    | Validates technical soundness of cloud services/products.                |
| **Security Risk Management CoE**                   | Ensures regulatory, security, compliance alignment for services.         |
| **Cloud Financial Operations (FinOps) CoE**        | Reviews and approves cost feasibility for cloud services.                |
| **Governance Board (VP/CIO/CTO Leadership)**       | Final decision-makers for cloud product approvals and exceptions.        |
| **Platform Engineering CoE**                       | Provisions, automates, integrates approved cloud services.               |
| **Service Ownership CoE**                          | Operates live cloud services, monitors SLAs, manages incidents.          |
| **Corporate Finance/PMO**                          | Reviews and prioritizes business funding based on Idea Cards.            |
| **External Cloud Providers (AWS, Azure, GCP)**     | Supply raw cloud infrastructure consumed via internal governance models. |

---

# **High-Level Relationships (Narrative Form)**

* **Application Teams** → Submit service demand into the **Cloud Product Governance Framework**.
* **Cloud Product Management** → Manages intake, triage, and lifecycle of service products.
* **EA / Security / FinOps** → Validate each service proposal across architecture, risk, and financial feasibility.
* **Governance Board** → Approves or rejects cloud products after validations.
* **Corporate Finance** → Evaluates Idea Cards for portfolio funding decisions.
* **Platform Engineering** → Builds/deploys provisioned infrastructure post-approval.
* **Service Ownership** → Operates and manages the lifecycle of deployed services.
* **External Vendors** → Provide platforms (AWS, Azure, GCP) which are wrapped and governed internally.

---

# **Structural Layout for Diagram**

(Imagine center point is the Governance Framework)

```
                     +----------------+
                     | Application Teams|
                     +----------------+
                             |
                             v
+----------------+     +---------------------------------------+      +------------------+
| Enterprise     | --> | HCSC Cloud Product Governance System | <---> | Platform Engineering |
| Architecture CoE |   | (Managed by Cloud Product Mgmt CoE)  |       | Service Ownership    |
+----------------+     +---------------------------------------+      +------------------+
                             ^
                             |
+----------------+           |           +----------------+
| Security Risk  |           |           | FinOps (Cost Mgmt)|
| Mgmt CoE       |           |           +----------------+
+----------------+           |
                             v
                     +----------------+
                     | Governance Board |
                     +----------------+
                             |
                             v
                     +----------------+
                     | Corporate Finance |
                     +----------------+
                             |
                             v
                     +----------------+
                     | External Vendors |
                     | (AWS, Azure, GCP) |
                     +----------------+
```

---

# **C4 Context Diagram Key**

| **Element**      | **Type**                                                                                                       |
| :--------------- | :------------------------------------------------------------------------------------------------------------- |
| System           | The Cloud Product Governance Framework                                                                         |
| Person/Group     | Actors like Application Teams, EA, Security, FinOps, Platform Engineering, Governance Board, Corporate Finance |
| External Systems | AWS, Azure, GCP (providing infrastructure)                                                                     |

---

# **Summary**

> The **C4 Level 1 Context Diagram** will center around the **HCSC Cloud Product Governance System**
> and show how business teams, operational CoEs, governance bodies, and cloud providers **interact** with it.


