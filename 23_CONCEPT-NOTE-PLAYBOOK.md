# **Concept Note Development Playbook**

*(Building the Initial High-Level Business and Technical Case for Governance Intake)*

---

# **Concept Note Development Playbook**

---

## **1. Purpose**

To guide Cloud Product Management CoP and SMEs in creating a **Concept Note** after a TAP request is accepted (and Discovery completed if required), documenting the initial business justification, high-level technical viability, and framing the service/product for full governance review.

The Concept Note is **the first formal articulation** of what the cloud service/product is, why it matters, and whether it should move forward.

---

## **2. Audience (Who Uses This Playbook)**

| **Role**                                       | **Responsibilities**                          |
| :--------------------------------------------- | :-------------------------------------------- |
| Cloud Product Management Lead                  | Owns Concept Note creation and coordination.  |
| Discovery Lead (if applicable)                 | Supplies findings to inform the Concept Note. |
| Assigned SMEs (Architecture, Security, FinOps) | Provide input where needed.                   |

---

## **3. Prerequisites**

* TAP triaged and accepted.
* (Optional) Discovery completed and documented.
* Initial technical, security, and cost knowledge gathered (at a high level).

---

## **4. Concept Note Development Steps**

---

### **Step 1: Retrieve Discovery Document (If Exists)**

* If Discovery was performed, retrieve the final Discovery Document.
* Use findings to populate parts of the Concept Note (especially risks, technical feasibility).

---

### **Step 2: Create Concept Note Document**

* Start new Concept Note in Confluence under **Concept Notes Repository**.
* Use standardized Concept Note Template.

---

### **Step 3: Populate Concept Note Sections**

| **Section**                             | **Content**                                                                               |
| :-------------------------------------- | :---------------------------------------------------------------------------------------- |
| Executive Summary                       | 1-2 paragraph description of the service/product request, in business terms.              |
| Business Drivers                        | List the problems, goals, or opportunities this service addresses.                        |
| Sponsoring Business Unit                | Which team/business unit is requesting this service?                                      |
| Target Cloud Deployment Models          | IaaS, PaaS, SaaS (specify expected providers — AWS, Azure, GCP).                          |
| Data Sensitivity Level                  | HIPAA, HITRUST, PII, internal-only, public, etc.                                          |
| Estimated Size and Scope                | Expected scale (small, medium, large); expected user base.                                |
| Initial Security Considerations         | Any obvious security risks or protections known at this point.                            |
| Initial Cost Considerations             | Ballpark budget impacts (not detailed modeling yet).                                      |
| Technical Integration Points (If Known) | Any major systems this needs to integrate with (identity, networks, observability, etc.). |
| High-Level Timeline Needs               | Is there urgency? Regulatory deadlines?                                                   |
| Known Risks or Open Questions           | Early flags or risks needing resolution later.                                            |

---

### **Step 4: Link Back to TAP and Discovery**

* Add references/links:

  * TAP ID in ServiceNow.
  * Discovery Document ID (if Discovery completed).

---

### **Step 5: Conduct Internal Concept Note Review**

* Circulate draft Concept Note internally to:

  * Assigned SME reviewers (EA, Security, FinOps leads if available).
  * Application Team Requestor (optional but recommended).
* Incorporate major feedback before RFC Consolidation phase begins.

---

### **Step 6: Update Status and Notifications**

* Update TAP record in ServiceNow:

  * Status: "**Concept Note Created**"
* Notify Cloud Product Management CoP leadership that Concept Note is ready for RFC building.

---

## **5. SLA Expectations**

| **Action**                            | **Target Timeline**                                       |
| :------------------------------------ | :-------------------------------------------------------- |
| Concept Note Draft                    | Within 10 business days of Intake or Discovery Completion |
| Concept Note Internal Review Complete | Within 5 additional business days                         |

---

## **6. Common Pitfalls to Avoid**

* Writing a Concept Note **only from technical viewpoint** without business drivers clearly stated.
* Failing to mention data sensitivity — extremely important in healthcare cloud.
* Rushing into RFC building without a solid Concept Note foundation.
* Copy-pasting vendor marketing material — focus must be HCSC-specific needs.

---

# **End of Concept Note Development Playbook**

---

# **Quick Visual (Summary Only)**

```
[Intake/Discovery Completed]
     ↓
[Create Concept Note]
     ↓
[Internal SME Review]
     ↓
[Ready for RFC Consolidation]
```

