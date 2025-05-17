# **Infrastructure Provisioning Playbook**

*(Deploying Approved Cloud Products and Services Post-Governance Approval)*

---

# **Infrastructure Provisioning Playbook**

---

## **1. Purpose**

To define how Platform Engineering CoE provisions cloud infrastructure and services based on approved Blueprints, ensuring deployments meet HCSC standards for security, observability, automation, and operational readiness.

This covers the **build phase** after Governance Board approval.

---

## **2. Audience (Who Uses This Playbook)**

| **Role**                      | **Responsibilities**                                                       |
| :---------------------------- | :------------------------------------------------------------------------- |
| Platform Engineering Lead     | Oversees provisioning and automation execution.                            |
| Platform Engineering SMEs     | Build Terraform modules, configure Harness pipelines, deploy environments. |
| Observability Engineers       | Integrate monitoring and telemetry during provisioning.                    |
| Cloud Product Management Lead | Tracks progress for governance reporting.                                  |

---

## **3. Prerequisites**

* Approved **Blueprint** and **Governance Decision Summary** available.
* (Optional) Portfolio funding approval (Idea Card acceptance if needed).
* Clear ServiceNow or Jira project entry opened for provisioning tasks.
* Required credentials, cloud subscriptions, access policies available.

---

## **4. Provisioning Process Steps**

---

### **Step 1: Provisioning Kickoff**

* Platform Engineering Lead reviews approved Blueprint.
* Confirm scope, timelines, observability, and compliance expectations.

---

### **Step 2: Build Automation and Infrastructure Code**

| **Technology**          | **Action**                                                         |
| :---------------------- | :----------------------------------------------------------------- |
| Terraform               | Author/Update modules for environment provisioning.                |
| Harness (IaC Pipelines) | Create or update automated build/deploy pipelines.                 |
| GitHub                  | Commit Infrastructure as Code artifacts; follow PR review process. |
| Ansible (optional)      | Use for legacy or IaaS-specific configurations.                    |

---

### **Step 3: Execute Environment Provisioning**

* Trigger pipelines to deploy environments into:

  * AWS
  * Azure
  * (Future: GCP)
* Set up resource groups, IAM roles, VPCs/subnets, compute, storage, managed services (as defined in Blueprint).

---

### **Step 4: Integrate Observability and Telemetry**

| **Platform**        | **Action**                                                                                     |
| :------------------ | :--------------------------------------------------------------------------------------------- |
| Dynatrace           | Enable infrastructure monitoring agents (VMs, containers, serverless, etc.).                   |
| Cribl               | Configure telemetry routing from new services to internal observability hubs (Dynatrace, ELK). |
| ELK (Elasticsearch) | Set up initial dashboards or log ingestion rules (if required).                                |

---

### **Step 5: Operational Hardening**

* Enforce tagging standards (ownership, cost center, environment, compliance).
* Enable backup policies (where required).
* Apply security guardrails (firewall rules, encryption, secrets management).
* Document resource architectures if dynamic.

---

### **Step 6: Operational Readiness Validation**

* Perform initial service health checks (compute, network, storage, platform-specific).
* Validate observability hooks:

  * Metrics flowing into Dynatrace.
  * Logs routed correctly through Cribl/ELK.
* Test basic alerting triggers.

---

### **Step 7: Prepare Operational Artifacts**

| **Artifact**                       | **Purpose**                                                        |
| :--------------------------------- | :----------------------------------------------------------------- |
| Runbook                            | How to operate and troubleshoot the service (Cloud Support Teams). |
| Operational Checklist              | Configurations, integrations, backup, disaster recovery readiness. |
| Architecture Diagram (Final Build) | Updated final deployment diagram.                                  |

---

### **Step 8: Handoff to Service Ownership CoE**

* Conduct Handoff Review Meeting:

  * Runbook review.
  * Architecture review.
  * Monitoring & alerting validation walkthrough.
* Officially transfer operational responsibility after sign-off.

---

## **5. SLA Expectations**

| **Action**                                     | **Target Timeline**                            |
| :--------------------------------------------- | :--------------------------------------------- |
| Provisioning Kickoff After Governance Approval | Within 5 business days                         |
| Initial Infrastructure Build Complete          | Within 30 calendar days (normal size projects) |
| Handoff to Operations Complete                 | Within 5 business days after build validated   |

---

## **6. Common Pitfalls to Avoid**

* Skipping observability integration during provisioning (causes major ops issues later).
* Missing critical resource tagging (hurts security, billing, compliance).
* Over-provisioning or under-provisioning due to poor translation of Blueprint sizing.
* Failing to update final build architecture documentation.

---

# **End of Infrastructure Provisioning Playbook**

---

# **Quick Visual (Summary Only)**

```
[Blueprint Approved]
     ↓
[Provisioning Kickoff]
     ↓
[Terraform + Harness Builds]
     ↓
[Deploy Environments]
     ↓
[Observability Integration]
     ↓
[Operational Readiness Validation]
     ↓
[Handoff to Service Ownership]
```

