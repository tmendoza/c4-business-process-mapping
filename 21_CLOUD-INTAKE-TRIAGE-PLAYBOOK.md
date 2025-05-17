# **Intake Triage and Validation Playbook**

*(Cloud Product Management CoE - Initial TAP Review and Validation)*

---

# **Intake Triage and Validation Playbook**

---

## **1. Purpose**

To guide the Cloud Product Management Community of Practice (CoP) in reviewing incoming Technology Approval Requests (TAPs) for completeness, eligibility, and governance routing — ensuring the governance pipeline flows smoothly and no bad or incomplete requests proceed.

---

## **2. Audience (Who Uses This Playbook)**

| **Role**                            | **Responsibilities**                        |
| :---------------------------------- | :------------------------------------------ |
| Cloud Product Management Intake SME | Assigned to intake and review TAPs.         |
| Cloud Product Management Lead       | Oversees intake flow, escalates edge cases. |

---

## **3. Prerequisites**

* TAP Request must be properly submitted in ServiceNow.
* TAP includes all mandatory fields filled (Title, Business Driver, Data Sensitivity, etc.).
* ServiceNow TAP ID issued.

---

## **4. Intake Triage Steps**

### **Step 1: Initial TAP Completeness Check**

* Review submitted TAP form for all mandatory fields.
* Validate contact information is provided.
* Validate data sensitivity classification is specified.

**If incomplete:**

* Send TAP back to Requestor with change request comments (through ServiceNow TAP portal).

---

### **Step 2: Basic Eligibility Assessment**

* Is this a cloud-related request (IaaS, PaaS, SaaS)?
* Does it align with supported cloud providers (AWS, Azure, GCP, Private Cloud)?
* Is it a net-new service, a major upgrade, or an operational change requiring governance?

**If clearly out of scope:**

* Reject TAP formally with justification.

---

### **Step 3: Discovery Trigger Assessment**

* Based on information provided:

  * Is the request introducing **new, novel, or unvetted technologies**?
  * Is technical feasibility uncertain?
  * Are there known **security, compliance, or cost unknowns**?
* Use the Discovery Decision Tree checkpoints (previously defined).

| **If Yes**                | **If No**                              |
| :------------------------ | :------------------------------------- |
| Trigger Discovery Process | Move directly to Concept Note drafting |

---

### **Step 4: Triage Outcome**

| **Possible Outcome**          | **Next Step**                                           |
| :---------------------------- | :------------------------------------------------------ |
| Complete, straightforward TAP | Move to Concept Note creation.                          |
| TAP needs Discovery           | Initiate Discovery Document and assign Discovery Owner. |
| TAP incomplete                | Return to Requestor for more information.               |
| TAP out-of-scope              | Reject and close request.                               |

---

## **5. Discovery Trigger Actions (If Needed)**

* Create new Discovery Work Item (in Confluence and/or ServiceNow linked to TAP).
* Assign Discovery Lead (from Cloud Product Management or SME pool).
* Notify Application Team of Discovery initiation and timelines.

---

## **6. Documentation and Tracking**

* Update TAP status in ServiceNow:

  * **"Intake Accepted"** → if TAP moves forward.
  * **"Discovery Required"** → if Discovery process starts.
  * **"Needs More Information"** → if incomplete.
  * **"Rejected"** → if out of scope.
* Link Discovery Document to TAP ticket if Discovery initiated.
* Capture triage notes in ServiceNow TAP record.

---

## **7. SLA Expectations**

| **Action**                     | **SLA**                               |
| :----------------------------- | :------------------------------------ |
| Initial triage review complete | 5 business days after TAP submission  |
| Requestor notified of outcome  | 2 business days after triage decision |

---

## **8. Common Pitfalls to Avoid**

* Accepting incomplete TAPs without validation.
* Skipping Discovery when major technical unknowns exist.
* Allowing TAPs to age without clear triage decision.
* Missing data sensitivity classifications (high risk for healthcare environment).

---

# **End of Intake Triage and Validation Playbook**

---

# **Quick Visual (Summary Only)**

```
[TAP Submitted]
     ↓
[Intake Completeness and Eligibility Review]
     ↓
(Discovery Needed?)
     ↙          ↘
[Yes]          [No]
 ↓               ↓
[Start Discovery]    [Move to Concept Note Creation]
```


