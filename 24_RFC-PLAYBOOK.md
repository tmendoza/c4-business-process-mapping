# **RFC Development and Consolidation Playbook**

*(Building the Full Governance Packet for Review)*

---

# **RFC Development and Consolidation Playbook**

---

## **1. Purpose**

To guide the Cloud Product Management CoE and assigned SMEs through building a complete **Request for Comment (RFC)** document, consolidating all business, architecture, security, and financial validations needed for governance approval.

The RFC is the **formal package** presented to the Governance Board for decision-making.

---

## **2. Audience (Who Uses This Playbook)**

| **Role**                                  | **Responsibilities**                                       |
| :---------------------------------------- | :--------------------------------------------------------- |
| RFC Owner (Cloud Product Management Lead) | Manages RFC development and consolidation.                 |
| Assigned Architecture SME                 | Provides architecture review findings.                     |
| Assigned Security SME                     | Provides security and risk findings.                       |
| Assigned FinOps SME                       | Provides cost modeling and financial analysis.             |
| Application Team (Optional Contributor)   | Provides context, clarifications, pilot results if needed. |

---

## **3. Prerequisites**

* Completed and approved **Concept Note**.
* Discovery findings (if Discovery was conducted).
* Initial business case and technical feasibility outlined.

---

## **4. RFC Development Steps**

---

### **Step 1: Create RFC Document**

* Start new RFC in Confluence under **RFC Repository**.
* Use standardized RFC Template.

---

### **Step 2: Populate Core RFC Sections**

| **Section**                        | **Content**                                                                   |
| :--------------------------------- | :---------------------------------------------------------------------------- |
| Executive Summary                  | Short description summarizing business drivers and solution intent.           |
| Business Context                   | Detailed business drivers, success criteria, sponsors.                        |
| Technical Architecture Overview    | High-level diagrams, architecture decisions, deployment models.               |
| Security and Compliance Assessment | Known risks, required protections, initial compliance validation.             |
| Financial Analysis                 | Estimated cost structures, cloud spend forecasts, FinOps findings.            |
| Operational Considerations         | Observability plans, SLAs, ownership plan, support model.                     |
| Integration Requirements           | Identity management, networking, monitoring, incident management touchpoints. |
| Known Risks and Mitigation         | Documented risks and initial mitigation approaches.                           |
| Supporting Discovery (If Done)     | Summary of key Discovery findings, if applicable.                             |
| TAP and Concept Note References    | Cross-links for full traceability.                                            |

---

### **Step 3: Solicit Inputs from Review SMEs**

| **SME Area**                | **Contribution Needed**                                         |
| :-------------------------- | :-------------------------------------------------------------- |
| Enterprise Architecture SME | Validate architecture design, cloud model fit, reuse alignment. |
| Security SME                | Validate data protection, compliance, threat surfaces.          |
| FinOps SME                  | Validate cost realism, sustainability, optimizations.           |

* Send RFC draft sections to SMEs.
* Hold working sessions if major issues surface.
* Record SME comments directly in the RFC or Confluence comment threads.

---

### **Step 4: Consolidate RFC Inputs**

* Incorporate SME findings into final RFC document.
* Ensure all sections are completed — **no gaps**.

---

### **Step 5: Conduct Internal Pre-Governance Review**

* Circulate RFC internally to Cloud Product Management CoP leadership.
* Optional: pre-review with Architecture Review Board or Security Risk Council.
* Adjust RFC based on pre-review feedback.

---

### **Step 6: Update Status and Link Artifacts**

* Update ServiceNow TAP record:

  * Status: "**RFC Ready for Governance Submission**"
* Link final RFC Document to TAP and Concept Note records.

---

### **Step 7: Prepare for Governance Submission**

* Final RFC ready for formal Governance Board Review.
* No additional work needed at this stage unless requested.

---

## **5. SLA Expectations**

| **Action**           | **Target Timeline**                             |
| :------------------- | :---------------------------------------------- |
| RFC Drafting Started | Within 5 business days of Concept Note approval |
| SME Inputs Completed | Within 10 business days after RFC start         |
| Internal Pre-Review  | Within 5 additional business days               |

---

## **6. Common Pitfalls to Avoid**

* Leaving blank sections in RFC (Governance Boards reject incomplete packets).
* Not properly linking TAP/Discovery/Concept Note back to RFC.
* Glossing over security compliance risks without clear language.
* Providing vague financial estimates without FinOps validation.
* Ignoring operational integration (identity, observability, SLA planning).

---

# **End of RFC Development and Consolidation Playbook**

---

# **Quick Visual (Summary Only)**

```
[Concept Note Approved]
     ↓
[Start RFC Draft]
     ↓
[Architecture/Security/FinOps Inputs]
     ↓
[Consolidate RFC]
     ↓
[Internal Review]
     ↓
[Governance Submission Ready]
```

