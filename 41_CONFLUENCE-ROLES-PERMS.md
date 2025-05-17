# **Confluence Space Roles and Permissions Proposal**

*(for HCSC Cloud Product Governance & Operations)*

---

# **Purpose**

Define **who can view, edit, create, approve**, or **administer** the documents, templates, trackers, and knowledge articles in the Governance & Operations Space.

Good **permission hygiene** is critical for:

* Avoiding accidental document corruption,
* Keeping templates pristine,
* Ensuring governance data is trustworthy.

---

# **Role Categories**

| **Role Name**               | **Who Fits Here**                                            | **Permissions Needed**                                           |
| :-------------------------- | :----------------------------------------------------------- | :--------------------------------------------------------------- |
| Space Admins                | Cloud Product Management Leadership Team                     | Full Admin Access (Create, Edit, Delete, Space Settings)         |
| Governance Document Editors | Cloud Product Managers, Architects, Security SMEs            | Create/Edit Pages for Templates, TAPs, RFCs, Blueprints, etc.    |
| Operational Owners          | Platform Engineering, Service Ownership Leads                | Edit Runbooks, RCA Reports, Compliance Trackers                  |
| Viewers                     | Application Teams, Engineering Teams, Finance, PMO, Auditors | Read-only Access                                                 |
| Approvers                   | Governance Board Members (VPs/Directors)                     | Comment on RFCs, Decision Summaries (but usually no edit needed) |

---

# **Detailed Permission Mapping**

| **Area**                               | **Admins**       | **Gov Doc Editors** | **Ops Owners** | **Viewers** | **Approvers** |
| :------------------------------------- | :--------------- | :------------------ | :------------- | :---------- | :------------ |
| Welcome & Overview                     | Edit             | Edit                | View           | View        | View          |
| Governance Process                     | Edit             | Edit                | View           | View        | View          |
| Templates Library                      | Manage Templates | View Only           | View Only      | View        | View          |
| Intake and Discovery                   | Edit             | Edit                | View           | View        | View          |
| Governance Reviews                     | Edit             | Edit                | View           | View        | Comment Only  |
| Service Blueprints                     | Edit             | Edit                | View           | View        | View          |
| Operational Management (Runbooks, RCA) | Edit             | View                | Edit           | View        | View          |
| Compliance and Audits                  | Edit             | View                | Edit           | View        | View          |
| Knowledge Base Articles                | Edit             | Edit                | View           | View        | View          |

---

# **Specific Rules to Implement**

1. **Templates Library** should be **protected**:

   * Only editable by Admins (Space Settings permissions)
   * End users **create from template**, **not modify templates directly**.

2. **Governance Decision Pages** (RFCs, Decisions) should be **editable only by Cloud Product Managers** and **commented on by Approvers**.

3. **Runbooks and RCA Reports** are **editable by Service Ownership and Platform Engineering** (since they maintain live services).

4. **Compliance Tracker** edits restricted to **Service Owners** and **Compliance SMEs**.

5. **Public access (unauthenticated users)** should be **disabled** entirely.

6. **Audit Trails enabled** — track who edited governance artifacts.

---

# **Visual Sketch (Role Access)**

```
Space Admins → Full Access Everywhere
Governance Editors → Create/Edit Documents
Ops Owners → Create/Edit Runbooks, RCA, Compliance
Approvers → Comment Only on RFCs/Decisions
Viewers → Read-only Access
```

