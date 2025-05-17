# **Discovery Execution Playbook**

*(Managing Optional Discovery Phase After TAP Intake)*

---

# **Discovery Execution Playbook**

---

## **1. Purpose**

To define how the Cloud Product Management CoE (and supporting SMEs) run Discovery Processes for cloud service requests that require deeper technical, security, financial, or operational investigation before formal Concept Note and governance evaluation.

---

## **2. Audience (Who Uses This Playbook)**

| **Role**                                     | **Responsibilities**                                       |
| :------------------------------------------- | :--------------------------------------------------------- |
| Discovery Lead (Cloud Product Mgmt or SME)   | Drives and coordinates Discovery process.                  |
| Assigned SMEs (Architects, Security, FinOps) | Support deep dives, PoCs, analyses.                        |
| Application Teams                            | Provide information, participate in tests/demos if needed. |

---

## **3. Prerequisites**

* TAP formally triaged and flagged as needing Discovery.
* Discovery Work Item created and linked to TAP in ServiceNow/Confluence.
* Discovery Lead assigned.

---

## **4. Discovery Process Steps**

### **Step 1: Define Discovery Scope**

* **Objective Statement:** What questions are we trying to answer? (technical feasibility, risk validation, cost modeling, etc.)
* **In-Scope Boundaries:** What will be explored, tested, or validated?
* **Out-of-Scope Items:** What will not be addressed?

*Document these in Discovery Document Section 2.*

---

### **Step 2: Assemble Discovery Team**

* Assign SMEs:

  * Architecture
  * Security
  * FinOps
  * Platform Engineering (optional, for pilots)
* Assign Application Team contacts (technical and business).

---

### **Step 3: Plan Discovery Activities**

| **Possible Activities**          | **Examples**                                             |
| :------------------------------- | :------------------------------------------------------- |
| Technical Proof of Concept (PoC) | Set up pilot cloud environments, integration tests.      |
| Proof of Value (PoV)             | Validate business outcomes with minimal viable solution. |
| Vendor Demos                     | Review solutions if external tools involved.             |
| Risk Workshops                   | Identify security, compliance risks early.               |
| Cost Forecasting Exercises       | Estimate preliminary cloud costs.                        |

*Document planned activities in Discovery Document Section 3.*

---

### **Step 4: Execute Discovery Activities**

* Conduct labs, pilots, workshops as planned.
* Collect all technical, financial, risk findings.
* Meet weekly (or as needed) to track discovery progress.

---

### **Step 5: Document Discovery Findings**

* Technical viability
* Security and compliance feasibility
* Cost model rough estimates
* Operational complexity
* Risks and assumptions
* Initial integration points (if known)

*All findings captured in Discovery Document Section 4.*

---

### **Step 6: Recommend Discovery Outcome**

| **Possible Outcomes**      | **Next Action**                                             |
| :------------------------- | :---------------------------------------------------------- |
| Positive                   | Proceed to Concept Note drafting.                           |
| Caution (Risks Identified) | Proceed with adjustments; note risks in Concept Note.       |
| Negative (Non-viable)      | Recommend TAP closure or major rework before re-submission. |

*Discovery Document Section 5 will include final recommendation.*

---

### **Step 7: Finalize Discovery Document**

* Final edit and review with SMEs and Discovery Lead.
* Upload to Confluence Discovery Repository.
* Link final Discovery Document to TAP record in ServiceNow.

---

### **Step 8: Notify Stakeholders**

* Notify Application Team of Discovery Outcome.
* Notify Cloud Product Management CoP to proceed or pause intake process.

---

## **5. SLA Expectations**

| **Discovery Stage**          | **Target Timeline**                                       |
| :--------------------------- | :-------------------------------------------------------- |
| Initial Scope Defined        | Within 5 business days of Discovery decision              |
| Discovery Execution Complete | Within 30 calendar days of start (extensions by approval) |
| Final Discovery Document     | Delivered within 5 business days post-completion          |

---

## **6. Common Pitfalls to Avoid**

* Poor scoping at the start (vague Discovery objectives = wasted time).
* Failing to involve right SMEs early.
* Taking too long (Discovery should inform decisions, not become endless research).
* Producing findings but no clear recommendation (always recommend a path).

---

# **End of Discovery Execution Playbook**

---

# **Quick Visual (Summary Only)**

```
[Discovery Triggered]
      ↓
[Define Scope]
      ↓
[Assemble Team]
      ↓
[Plan Activities]
      ↓
[Execute PoC / PoV / Demos]
      ↓
[Capture Findings]
      ↓
[Recommend Outcome]
      ↓
[Document Discovery]
      ↓
[Notify Stakeholders and Proceed]
```

