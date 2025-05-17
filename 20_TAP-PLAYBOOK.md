# **TAP Request Submission Playbook**

*(Technology Approval Process Intake — Cloud Product Governance Program)*

---

## **1. Purpose**

To guide Application Teams and Requestors on how to properly initiate a Technology Approval Request (TAP) within HCSC’s Cloud Product Governance intake system.

Ensures all requests are complete, standardized, and ready for governance triage without unnecessary rework.

---

## **2. Audience (Who Uses This Playbook)**

| **Role**                              | **Responsibilities**                                      |
| :------------------------------------ | :-------------------------------------------------------- |
| Application Team Leaders              | Submit TAPs for cloud products, services, tooling needs.  |
| Technical Architects (Requestor Side) | Assist in completing technical fields (if needed).        |
| Business Owners / Product Owners      | Provide business justification and alignment to strategy. |

---

## **3. Prerequisites**

* Alignment with a sponsoring Business Unit.
* Initial internal review (within the Application Team) to confirm the need.
* (Optional but recommended) Consult with Cloud Product Management CoP early if unclear about scope.

---

## **4. Submission Steps**

### **Step 1: Access ServiceNow TAP Module**

* Log into ServiceNow portal.
* Navigate to the **Technology Approval Request** section.

### **Step 2: Complete TAP Form Fields**

| **Field**                         | **What to Fill**                                                   |
| :-------------------------------- | :----------------------------------------------------------------- |
| Title                             | Clear, business-readable title (e.g., "New AI Workbench on Azure") |
| Business Driver                   | What business problem or opportunity is this solving?              |
| Sponsoring Business Unit          | Which BU is requesting this?                                       |
| Primary Contact                   | Requestor name, department, and contact info.                      |
| Secondary Contacts (optional)     | Architects, SMEs helping with this request.                        |
| Requested Cloud Type              | (IaaS, PaaS, SaaS, or combination)                                 |
| Target Providers                  | (AWS, Azure, GCP, Private Cloud)                                   |
| Estimated Size/Cost (if known)    | (optional at this stage)                                           |
| Data Sensitivity Classification   | (HIPAA-regulated, PII, internal only, public)                      |
| Time Sensitivity / Deadlines      | Any urgent timelines (explain why).                                |
| Special Compliance Needs (if any) | E.g., HITRUST, PCI, GDPR, etc.                                     |

### **Step 3: Attach Supporting Documents (Optional)**

* Architecture sketches, vendor proposals, prior PoC results, budget estimates if available.

### **Step 4: Submit the TAP**

* Ensure no mandatory fields are missing.
* Submit via ServiceNow portal.
* Capture TAP Request ID for future tracking.

---

## **5. Immediate Post-Submission Expectations**

| **After Submission** | **What Happens**                                                                      |
| :------------------- | :------------------------------------------------------------------------------------ |
| TAP ID Assigned      | Unique identifier issued (email confirmation).                                        |
| Intake Triage Review | Cloud Product Management CoP initiates triage within 5 business days.                 |
| Possible Next Steps  | Discovery, Concept Note drafting, or immediate RFC kickoff (depending on complexity). |

---

## **6. Common Mistakes to Avoid**

* Submitting incomplete business drivers (e.g., “need new service” without explaining why).
* Omitting sensitive data classification (critical for security review later).
* Estimating technical sizing inaccurately (better to say “Unknown” than guessing wildly).

---

## **7. SLA Expectations**

* TAP will be reviewed within **5 business days**.
* Initial feedback (acceptance, request for Discovery, clarification needed) issued within **7 business days**.

---

# **End of TAP Request Submission Playbook**

---

# **Quick Visual (Summary Only)**

```
[Submit TAP Form] → [Triage Review by Cloud Product Management] → [Move into Discovery or Concept Note phase]
```


