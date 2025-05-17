# **Step 3: Discovery Decision Tree (Text Form)**

*(Guides whether Discovery is required after TAP is submitted)*

---

# **Discovery Decision Tree Logic**

1. **TAP Request Submitted**
   *(Technology Approval Request enters ServiceNow)*

2. **Intake Triage Review by Cloud Product Management CoP**

   * Quick validation checks: completeness, initial feasibility, relevance.

3. **Discovery Evaluation Criteria**

   Evaluate the request against these checkpoints:

   | **Checkpoint**                      | **Question**                                                                                                             |
   | :---------------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
   | New or Unfamiliar Technology?       | Is this a new cloud service, architecture pattern, vendor, or tooling we have no operational history with?               |
   | Unclear Technical Feasibility?      | Are there unresolved technical concerns (integration complexity, performance unknowns, scalability risk)?                |
   | Regulatory or Security Sensitivity? | Is there potential for non-standard HIPAA/HITRUST, security, or privacy challenges?                                      |
   | Financial or Cost Risk?             | Are projected cloud costs high, highly variable, or poorly understood based on initial input?                            |
   | Operational Complexity?             | Would deployment require new types of automation, observability patterns, or operations processes?                       |
   | Business Model Innovation?          | Is this introducing a new product class or strategic capability (e.g., first time AI model hosting, blockchain service)? |

4. **Discovery Decision Branch**

   * **If "Yes" to one or more Checkpoints → Discovery Required**

     * Initiate Discovery Process
     * Create Discovery Document
   * **If "No" to all Checkpoints → Discovery Not Required**

     * Proceed directly to Concept Note development

5. **Documentation**

   * Discovery Decision (Yes/No) logged in TAP record notes field in ServiceNow
   * If Discovery performed, link Discovery Document ID to TAP record

6. **Next Steps Based on Path**

   | **Path**            | **Next Action**                                                                           |
   | :------------------ | :---------------------------------------------------------------------------------------- |
   | Discovery Needed    | Create Discovery Document → Perform findings and recommendations → Feed into Concept Note |
   | No Discovery Needed | Move directly into drafting Concept Note                                                  |

---

# **Discovery Decision Tree (Visual Flow in Text)**

```
TAP Request Submitted (ServiceNow)
      ↓
Cloud Product Management Triage Review
      ↓
Discovery Evaluation Checkpoints:
    - New/Unfamiliar Tech?
    - Technical Uncertainty?
    - Regulatory/Security Sensitivity?
    - Financial Cost Risk?
    - Operational Complexity?
    - Business Model Innovation?
      ↓
[If YES to any]
      ↓
→ Initiate Discovery Process
→ Create Discovery Document
→ After Discovery → Create Concept Note
      ↓
[If NO to all]
      ↓
→ Create Concept Note Directly
```

---

# **Key Design Rules**

* **Bias for Speed:** If technology is already approved, safe, and well-understood, skip Discovery and accelerate governance.
* **Bias for Safety:** If unknowns exist in technical feasibility, security posture, or operational readiness, **Discovery is mandatory**.
* **Governance Audibility:** Discovery decisions must be **traceable back to TAP records** for compliance and operational transparency.

---

# **Summary**

> **Discovery is not a gate for everything** — it's a **protective diligence loop** triggered only when risk, complexity, or novelty requires it.
>
> **Embedding Discovery at the right point** strengthens product governance without slowing down routine innovation.

---

**That completes Step 3!**

