# **Step 2: Updated Stage-by-Stage Artifact Mapping (Including Discovery Process)**

This updated version **slots Discovery correctly** and **makes the path clear** depending on whether Discovery is needed or not.

---

# **Updated Artifact Flow Across Governance Stages**

| **Stage**                | **Action**                                                | **Primary Artifact(s)**                            | **Storage Location**                                     | **Notes**                                                 |
| :----------------------- | :-------------------------------------------------------- | :------------------------------------------------- | :------------------------------------------------------- | :-------------------------------------------------------- |
| Stage 1                  | Product Demand Intake                                     | **Technology Approval Request (TAP)**              | ServiceNow                                               | Mandatory for all requests                                |
| *Stage 1a* (Conditional) | **Discovery Process** *(Optional)*                        | **Discovery Document**                             | Confluence (Discovery Documents Repo)                    | Only created if deeper validation is needed               |
| Stage 2                  | Intake Triage and Quick Validation                        | **Concept Note**                                   | Confluence (Concept Notes Repo)                          | Created whether or not Discovery was performed            |
| Stage 3–5                | Architecture Review, Security Assessment, Cost Estimation | **Request for Comment (RFC)**                      | Confluence (RFC Repo)                                    | Consolidates all technical, security, and cost findings   |
| Stage 6                  | Governance Gate Review and Decision                       | **Blueprint**                                      | Confluence (Blueprints Repo)                             | Governance-signed design and operational standard         |
| Stage 7                  | Provisioning and Observability Integration                | **Project Initialization Docs**                    | Jira / Confluence (Project Docs Repo)                    | Converts Blueprint into real build work                   |
| Stage 8                  | Product Launch and Operational Handoff                    | **Runbooks**, **Operational Guidelines**, **SOPs** | Confluence (Runbooks Repo) and ServiceNow Knowledge Base | Guides for operational support and escalation             |
| Stage 9                  | Ongoing Monitoring and Compliance                         | **Incident Records**, **RCAs**, **Audit Reports**  | ServiceNow, Dynatrace, Cribl, ELK Stack                  | Real-time and historical operational compliance artifacts |

---

# **Key Flow Behavior with Discovery**

* **If Discovery is NOT needed:**
  TAP → Concept Note → RFC → Blueprint → Deployment

* **If Discovery IS needed:**
  TAP → Discovery Document → Concept Note → RFC → Blueprint → Deployment

* **Discovery Document references back to TAP**

* **Concept Note references Discovery Document if it exists**

**Discovery Document becomes "evidence"** that more thorough diligence was done before promoting the product/service into the architecture review stream.

---

# **Updated End-to-End Visual (Textual)**

```
Technology Approval Request (TAP) [ServiceNow]
      ↓
(Optional) Discovery Document [Confluence]
      ↓
Concept Note [Confluence]
      ↓
Request for Comment (RFC) [Confluence]
      ↓
Blueprint [Confluence]
      ↓
Project Initialization [Jira / Confluence]
      ↓
Runbooks, SOPs [Confluence / ServiceNow KB]
      ↓
Incidents, RCA, Compliance Reports [ServiceNow, Dynatrace, Cribl, ELK]
```

---

# **Summary**

> The Discovery Document sits cleanly **between TAP and Concept Note** and only triggers when **greater technical/operational diligence is necessary**.
>
> It adds **no friction for simple/routine cloud services** but **adds safety and rigor** for complex, risky, or novel ones.

