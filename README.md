# 90TaskofDevOps

# Task-Based DevOps & DevSecOps Job-Readiness Roadmap

### Learn • Build • Practice • Prove Your Skills • Get Job-Ready

A self-paced, hands-on roadmap inspired by TrainWithShubham's **#90DaysOfDevOps** learning approach, adapted for professionals who want to become job-ready as quickly as possible.

**This is task-based, not day-based.** There is no 90-day deadline and no daily schedule. Complete tasks in priority order, demonstrate the outcome, document your work, and move forward. Apply for jobs and prepare for interviews from the beginning.

> This is an independent, personalized roadmap inspired by the README structure shared for TrainWithShubham. It is not an official TrainWithShubham curriculum.

---

## 🎯 Objective

Prepare for these roles:

- Senior DevOps Engineer
- Cloud Engineer / Senior Cloud Engineer
- Cloud Security Engineer
- DevSecOps Engineer

The roadmap assumes existing hands-on experience with AWS, Terraform, Kubernetes, Linux, Docker, CI/CD, and cloud security. It prioritizes practical validation, production-style troubleshooting, portfolio evidence, and interview readiness rather than repeating beginner lessons unnecessarily.

## 🧭 How to Use This Roadmap

1. Complete tasks in priority order, not according to a calendar.
2. If you can already demonstrate a skill confidently, validate it quickly and move on.
3. Every task should produce evidence: working code, test output, screenshots, diagrams, or a documented troubleshooting case.
4. Keep secrets, private keys, credentials, personal information, and sensitive infrastructure details out of public repositories.
5. Apply for relevant jobs while learning. Do not wait until the entire roadmap is complete.
6. Use interview feedback to decide which skill to improve next.
7. Keep cloud costs under control. Use budgets, small environments, and teardown procedures.

### Definition of Done

A task is complete when:

- [ ] The solution works or the scenario can be reproduced.
- [ ] You can explain the approach and important trade-offs.
- [ ] You have tested the expected behavior and relevant failure cases.
- [ ] The README documents setup, validation, results, and cleanup where applicable.
- [ ] The GitHub deliverable contains no secrets or sensitive data.
- [ ] You can discuss the work confidently in an interview.

---

# 🚀 Phase 1 — Job-Search Foundation

Start this phase immediately. Job applications and interview preparation should continue throughout the roadmap.

## Task 1.1 — Create a Job-Targeting Matrix

**Actions**
- [ ] Collect 5–10 job descriptions for Senior DevOps / Cloud Engineer roles.
- [ ] Collect 5–10 job descriptions for Cloud Security / DevSecOps roles.
- [ ] Record recurring technologies, responsibilities, security requirements, and seniority expectations.
- [ ] Map each requirement to your experience and evidence.
- [ ] Identify the most important skill gaps based on real vacancies.

**Completion criteria:** A prioritized list of strengths, gaps, and target roles.

**Deliverable:** `job-readiness/role-requirements-matrix.md`

## Task 1.2 — Prepare Two Targeted Resumes

**Actions**
- [ ] Create a Senior DevOps / Cloud Engineer resume.
- [ ] Create a Cloud Security / DevSecOps Engineer resume.
- [ ] Highlight AWS, Terraform, Kubernetes, CI/CD, automation, security, and troubleshooting.
- [ ] Quantify achievements only where the results can be substantiated.
- [ ] Include links to relevant GitHub projects.
- [ ] Make sure every listed skill can be explained in an interview.

**Completion criteria:** Each resume clearly matches its target role and demonstrates technical ownership, outcomes, and relevant experience.

**Deliverable:** Keep the resumes privately and link to public project repositories where appropriate.

## Task 1.3 — Upgrade Your GitHub Profile

**Actions**
- [ ] Improve your GitHub profile README.
- [ ] Add a concise professional introduction and target roles.
- [ ] Pin your strongest repositories.
- [ ] Add architecture diagrams, setup steps, test results, and project outcomes.
- [ ] Review existing repositories for accidental secrets and sensitive information.
- [ ] Make each featured repository easy for a recruiter to understand.

**Completion criteria:** A recruiter can quickly understand your skills and inspect credible proof of work.

**Deliverable:** Profile README and 3–5 well-documented repositories, built progressively.

## Task 1.4 — Start Applying for Jobs

**Actions**
- [ ] Apply to roles that match your current experience.
- [ ] Tailor the appropriate resume to each vacancy.
- [ ] Track applications, recruiter conversations, interviews, and follow-ups.
- [ ] Record interview questions and weak areas.
- [ ] Prioritize learning based on actual role requirements and interview feedback.

**Completion criteria:** You have an active application workflow and use feedback to guide your learning.

**Deliverable:** Maintain a private job application tracker.

---

# 🧰 Phase 2 — Validate Core Engineering Skills

Do not repeat fundamentals you can already demonstrate. Use these tasks to confirm practical readiness.

## Task 2.1 — Linux Troubleshooting

**Practice**
- Disk exhaustion and filesystem usage
- CPU and memory pressure
- Process and service failures
- Permissions and ownership
- systemd and log analysis
- Network connectivity and listening ports

**Actions**
- [ ] Reproduce a Linux issue in a safe test environment.
- [ ] Diagnose it using commands and logs.
- [ ] Identify the root cause.
- [ ] Apply a safe fix and verify recovery.
- [ ] Document the diagnostic process.

**Completion criteria:** You can explain the evidence that led to the diagnosis and demonstrate the fix.

**Deliverable:** `linux-troubleshooting/README.md`

## Task 2.2 — Bash Automation

Build a reliable backup script with:
- [ ] Timestamped archives
- [ ] Error handling and safe command execution
- [ ] Logging and meaningful exit codes
- [ ] Retention for local backups
- [ ] Optional S3 archival and remote cleanup
- [ ] Validation and failure tests

**Completion criteria:** The script works on valid inputs, handles failures safely, preserves the required backups, and documents recovery behavior.

**Deliverable:** `automation/backup.sh`, tests, and usage documentation.

## Task 2.3 — Git and GitHub Workflows

**Actions**
- [ ] Practice branching and pull requests.
- [ ] Resolve a merge conflict.
- [ ] Use `.gitignore` correctly.
- [ ] Recover from an accidental local file deletion.
- [ ] Demonstrate safe rollback and explain the difference between local and remote changes.

**Completion criteria:** You can demonstrate the workflow and explain how to recover without losing important work.

**Deliverable:** `git-workflows/README.md` with reproducible examples.

## Task 2.4 — Networking Troubleshooting

**Practice**
- DNS resolution
- TCP connectivity and ports
- Routing and firewall rules
- TLS certificates and protocol negotiation
- HTTP status codes and reverse proxies
- Load balancer and service connectivity

**Completion criteria:** Diagnose a failed request, identify the failing layer, and support the conclusion with evidence.

**Deliverable:** `networking/troubleshooting-playbook.md`

---

# ☁️ Phase 3 — AWS and Terraform

## Task 3.1 — Build a Secure AWS Infrastructure Baseline

**Actions**
- [ ] Design a VPC with public and private subnets.
- [ ] Configure routing, security groups, and required network access.
- [ ] Deploy a test application behind an Application Load Balancer.
- [ ] Use IAM roles instead of hard-coded AWS credentials.
- [ ] Enable appropriate CloudTrail logging and encryption.
- [ ] Document cost assumptions and teardown steps.

**Completion criteria:** The application is reachable through the intended entry point, private resources are not unnecessarily exposed, and access paths are documented.

**Deliverable:** `aws-secure-baseline/` containing Terraform, architecture diagram, security decisions, validation evidence, and cleanup instructions.

## Task 3.2 — Build Reusable Terraform Modules

**Actions**
- [ ] Create modules for networking, IAM, compute, and security controls.
- [ ] Use variables, outputs, validation, and sensible defaults.
- [ ] Define a clear environment and state strategy.
- [ ] Configure protected remote state in S3 with encryption, restricted access, and state locking supported by the Terraform version and backend configuration.
- [ ] Pin provider versions and commit the dependency lock file.
- [ ] Validate formatting and configuration before applying changes.

**Completion criteria:** You can deploy the design consistently and explain module boundaries, state protection, and change management.

**Deliverable:** `terraform-aws-modules/` with example environments and documentation.

## Task 3.3 — Terraform Drift and Deleted-Resource Recovery

**Actions**
- [ ] Create a disposable test resource using Terraform.
- [ ] Delete the resource manually in the AWS console.
- [ ] Run `terraform plan` and inspect the proposed changes.
- [ ] Explain the difference between configuration, state, and actual infrastructure.
- [ ] Demonstrate a safe recovery or recreation procedure.
- [ ] Explain when import, refresh-only operations, or state repair may be appropriate.
- [ ] Avoid destructive experiments on production state.

**Completion criteria:** You can explain what Terraform detects and how to restore the desired state safely.

**Deliverable:** `terraform-drift-lab/README.md` with before-and-after plans, sanitized outputs, and a recovery runbook.

## Task 3.4 — Implement AWS Security Controls

**Actions**
- [ ] Apply least-privilege IAM policies.
- [ ] Protect encryption keys and key-management permissions.
- [ ] Configure relevant logging and threat-detection controls.
- [ ] Investigate sample findings from AWS security services.
- [ ] Remediate a test misconfiguration and verify the result.
- [ ] Document exceptions and evidence collection.

**Completion criteria:** You can demonstrate a misconfiguration, explain its risk, remediate it, and verify the corrected control.

**Deliverable:** `aws-cloud-security/` with IAM examples, policy checks, sample findings, and remediation procedures.

**Interview gate:** Be ready to discuss Terraform state security, drift, IAM trust policies, cross-account access, VPC design, KMS, incident investigation, and recovery after resource deletion.

---

# 🐳 Phase 4 — Docker and Kubernetes

Build on existing hands-on work with Kind, Services, Ingress, and application troubleshooting instead of repeating basic tutorials.

## Task 4.1 — Build Production-Quality Docker Images

**Actions**
- [ ] Create a multi-stage Dockerfile for an application.
- [ ] Run the application as a non-root user.
- [ ] Handle application shutdown correctly.
- [ ] Reduce image size and remove unnecessary build dependencies.
- [ ] Scan the image for known vulnerabilities.
- [ ] Document image tagging and versioning.

**Completion criteria:** The image builds reproducibly, the application passes its health checks, and the container runs with reduced privileges.

**Deliverable:** `docker-production/` with Dockerfile, build instructions, scan results, and design rationale.

## Task 4.2 — Deploy a Multi-Component Kubernetes Application

**Actions**
- [ ] Deploy a frontend, API, and database or equivalent multi-component application.
- [ ] Configure Deployments, Services, ConfigMaps, and Secrets appropriately.
- [ ] Add readiness, liveness, and startup probes where suitable.
- [ ] Set resource requests and limits.
- [ ] Configure persistent storage where needed.
- [ ] Configure Ingress or a suitable gateway and verify routing.
- [ ] Restrict unnecessary network communication.

**Completion criteria:** The application works end-to-end, survives a pod restart, and behaves correctly when a dependency becomes unavailable.

**Deliverable:** `kubernetes-production/` with manifests or Helm charts, architecture, validation commands, and troubleshooting notes.

## Task 4.3 — Kubernetes Troubleshooting Lab

Reproduce and diagnose:
- [ ] `CrashLoopBackOff`
- [ ] `ImagePullBackOff`
- [ ] Pending pods and storage failures
- [ ] Incorrect Service selectors or ports
- [ ] Ingress routing failures and HTTP 404/502 responses
- [ ] DNS failures and connectivity problems
- [ ] Resource pressure and failed probes

**Completion criteria:** For each scenario, use tools such as `kubectl describe`, events, logs, endpoints, and network tests to identify the cause, fix it, and prove recovery.

**Deliverable:** `kubernetes-incident-labs/` with at least five reproducible failure scenarios and resolutions.

## Task 4.4 — Helm, Scaling, and Cluster Operations

**Actions**
- [ ] Package the application as a Helm chart.
- [ ] Create environment-specific values.
- [ ] Configure resource-based autoscaling where metrics are available.
- [ ] Test rolling updates and rollback.
- [ ] Understand PodDisruptionBudgets, resource requests and limits, and scheduling constraints.
- [ ] Explain managed control-plane and worker-node responsibilities.

**Completion criteria:** You can install, upgrade, scale, diagnose, and roll back the application using documented commands.

**Deliverable:** `helm-app-chart/` with deployment and rollback demonstrations.

**Interview gate:** Explain request routing through a load balancer, Ingress, Service, and Pod; Kubernetes DNS; pending pods; and how to separate application, networking, and cluster-level failures.

---

# 🔄 Phase 5 — CI/CD and GitOps

## Task 5.1 — Build a Complete CI/CD Pipeline

Use Jenkins or GitHub Actions, prioritizing the tool most relevant to your target vacancies.

**Actions**
- [ ] Trigger builds on pull requests and merges.
- [ ] Run linting and unit tests.
- [ ] Build and scan a container image.
- [ ] Publish a versioned image to a registry.
- [ ] Deploy to a Kubernetes test environment.
- [ ] Verify deployment health and document rollback.
- [ ] Store credentials securely.

**Completion criteria:** A code change triggers an automated pipeline, failed tests block release, and a successful change reaches the test environment with verifiable evidence.

**Deliverable:** `cicd-pipeline/` with pipeline configuration, test results, architecture, and recovery instructions.

## Task 5.2 — Implement GitOps with Argo CD

**Actions**
- [ ] Store Kubernetes configuration in Git.
- [ ] Configure Argo CD to reconcile the desired application state.
- [ ] Demonstrate detection and correction of configuration drift.
- [ ] Separate development and production configuration.
- [ ] Test a controlled rollback and explain its limitations.

**Completion criteria:** A Git change updates the application through GitOps, and you can explain continuous reconciliation.

**Deliverable:** `argocd-gitops/` with application configuration and deployment evidence.

## Task 5.3 — Add Release Safety Controls

**Actions**
- [ ] Version releases and trace each image to its source commit.
- [ ] Add environment approvals where appropriate.
- [ ] Prevent deployment of failed or unverified builds.
- [ ] Define and test a rollback trigger.
- [ ] Document release evidence and recovery procedures.

**Completion criteria:** You can show what was released, how it was verified, and how to recover from a failed release.

**Deliverable:** `release-engineering/` with release workflow, evidence, and rollback runbook.

---

# 🛡️ Phase 6 — Cloud Security and DevSecOps

## Task 6.1 — Implement Shift-Left Security Gates

Integrate suitable tools for:
- [ ] Source-code and dependency scanning
- [ ] Terraform and Kubernetes configuration scanning
- [ ] Container image vulnerability scanning
- [ ] Secret detection
- [ ] Software bill of materials (SBOM) generation
- [ ] Risk-based pull-request quality gates

**Completion criteria:** Introduce a controlled test vulnerability or misconfiguration, demonstrate detection and pipeline behavior, then remediate it. Document severity thresholds and exception handling.

**Deliverable:** `devsecops-security-gates/` with pipeline configuration, sample reports, and remediation guidance.

## Task 6.2 — Artifact Signing and Supply-Chain Integrity

**Actions**
- [ ] Compare Cosign/Sigstore, GPG-based signing, and AWS Signer where relevant to the artifact type.
- [ ] Document trust models, key management, verification, operational overhead, and CI/CD integration.
- [ ] Sign a container image and verify its signature before deployment.
- [ ] Configure deployment verification against an explicit trust policy.
- [ ] Test rejection of an invalid or untrusted artifact.

**Completion criteria:** Your pipeline verifies a signed artifact and rejects one that fails the trust policy.

**Deliverable:** `artifact-signing/` with a comparison matrix, implementation, verification steps, and threat model.

## Task 6.3 — TLS and Endpoint Hardening

**Actions**
- [ ] Inventory endpoints and integrations in a sample architecture.
- [ ] Identify TLS requirements and compatibility constraints.
- [ ] Configure supported TLS policies for ALB/NLB listeners and relevant endpoints.
- [ ] Prefer TLS 1.3 where supported and compatible; enforce a suitable TLS 1.2 minimum where required.
- [ ] Remove obsolete or weak cryptographic options using supported security policies.
- [ ] Test certificates, protocol versions, and cipher negotiation.
- [ ] Document compatibility risks and rollback considerations.

**Completion criteria:** You have an endpoint inventory, documented compatibility decisions, and reproducible verification results.

**Deliverable:** `tls-hardening/` with policy matrix, configuration, test commands, and rollback considerations.

## Task 6.4 — Secrets and SSH Key Governance

**Actions**
- [ ] Inventory secrets and SSH key usage in a test environment.
- [ ] Design migration to a managed secret store such as AWS Secrets Manager, using KMS encryption and appropriately scoped access.
- [ ] Implement rotation for a test credential where supported by its consumers.
- [ ] Audit access and rotation activity using CloudTrail and relevant service logs.
- [ ] Assess AWS Systems Manager Session Manager as an alternative to routine direct SSH access.
- [ ] Document emergency access and credential revocation.

**Completion criteria:** Demonstrate controlled access, a tested rotation or revocation process, and auditable credential use.

**Deliverable:** `secrets-governance/` with architecture, example policies, rotation workflow, and incident runbook. Never commit real secrets or private keys.

## Task 6.5 — Security Testing and Compliance Evidence

**Actions**
- [ ] Map representative tests to relevant OWASP and CWE categories.
- [ ] Create unit or integration security tests using the application's language and framework.
- [ ] Add security tests to CI.
- [ ] Document findings, remediation, exceptions, and evidence retention.
- [ ] Explain how controls support relevant ISO 27001 or SOC 2 objectives without implying that tooling alone establishes compliance.

**Completion criteria:** An intentional test defect is caught by an automated test or quality gate, and the corrected version passes.

**Deliverable:** `security-test-framework/` with tests, mappings, pipeline integration, and sample reports.

**Interview gate:** Explain least privilege, threat modeling, secret rotation, TLS hardening, container signing, vulnerability prioritization, false positives, and balancing security with delivery speed.

---

# 📈 Phase 7 — Observability, Reliability, and Incident Response

## Task 7.1 — Implement Monitoring

**Actions**
- [ ] Deploy Prometheus and Grafana or an equivalent monitoring stack.
- [ ] Collect application and infrastructure metrics.
- [ ] Build dashboards for latency, traffic, errors, and resource saturation.
- [ ] Define actionable alerts with severity levels.
- [ ] Document the meaning and limitations of each metric.

**Completion criteria:** A deliberately introduced failure produces a useful alert, and the dashboard helps identify the affected component.

**Deliverable:** `observability-stack/` with dashboards, alert rules, deployment configuration, and screenshots.

## Task 7.2 — Centralize Logs and Investigate Failures

**Actions**
- [ ] Collect application and infrastructure logs centrally.
- [ ] Use structured logs and correlation identifiers where practical.
- [ ] Build queries for common failures.
- [ ] Define retention, access control, and sensitive-data handling.
- [ ] Correlate logs with metrics and deployment events.

**Completion criteria:** Starting from an alert, you can find relevant logs, identify the likely root cause, and document corrective action.

**Deliverable:** `centralized-logging/` with architecture, sample logs, investigation queries, and runbooks.

## Task 7.3 — Practice Incident Response

Simulate these incidents:
1. A failed application release.
2. A compromised or overprivileged test credential.
3. Resource exhaustion or a connectivity failure.

For each incident:
- [ ] Establish impact and severity.
- [ ] Gather evidence while preserving useful logs.
- [ ] Contain the issue safely.
- [ ] Restore service or revoke access.
- [ ] Identify the root cause.
- [ ] Define corrective and preventive actions.

**Completion criteria:** Each incident has a timeline, evidence, remediation, and a blameless post-incident review.

**Deliverable:** `incident-response-labs/` with three incident reports and operational runbooks.

---

# 🏗️ Phase 8 — End-to-End Capstone Project

## Capstone: Secure Cloud-Native Delivery Platform on AWS

Build one strong, integrated project instead of many shallow projects. Start with a small working version and add capabilities incrementally.

### Required Components

- [ ] **Infrastructure:** AWS VPC, subnet design, IAM, load balancing, and Terraform modules.
- [ ] **Application:** Containerized frontend and API, with a database or suitable managed data service.
- [ ] **Orchestration:** EKS or a clearly documented local Kubernetes equivalent for the initial build.
- [ ] **Delivery:** CI pipeline, image registry, automated validation, and Argo CD GitOps deployment.
- [ ] **Security:** IaC and image scanning, secret management, artifact verification, and least-privilege access.
- [ ] **Observability:** Metrics, dashboards, logs, actionable alerts, and incident runbooks.
- [ ] **Reliability:** Health checks, resource limits, rollout verification, rollback, and a documented recovery strategy.

### Capstone Completion Criteria

- [ ] A new user can follow the README to reproduce the deployment.
- [ ] A code change travels through the automated pipeline.
- [ ] An invalid configuration or failing test blocks promotion.
- [ ] A trusted artifact can be verified before deployment.
- [ ] Application health and key metrics are observable.
- [ ] At least two failure scenarios are reproduced and resolved.
- [ ] Teardown, cost controls, and security limitations are documented.
- [ ] The architecture and key trade-offs can be explained in an interview.

**Deliverable:** `capstone/` containing a professional README, architecture diagram, Terraform, application code, CI/CD configuration, Kubernetes or Helm manifests, security controls, monitoring configuration, incident reports, and sanitized proof of execution.

**Cost and safety:** Use AWS budgets, small environments, and teardown procedures. Do not leave billable resources running unnecessarily. Do not use production credentials or sensitive data in the public project.

---

# 🎤 Phase 9 — Interview Preparation

Begin interview preparation during the first job applications, not after finishing all technical tasks.

## Task 9.1 — Prepare Project Walkthroughs

For every major project, prepare a 5–10 minute explanation covering:

1. The business or operational problem.
2. The architecture and why you chose it.
3. Your individual responsibilities.
4. The most difficult failure you encountered.
5. Security, reliability, and cost trade-offs.
6. What you would improve in production.

**Completion criteria:** You can explain the project without reading the README and defend your decisions under follow-up questions.

## Task 9.2 — Practice Senior-Level Scenarios

Practice answering these questions aloud or in a written interview notebook:

- A resource is deleted manually in AWS. How does Terraform respond?
- A Kubernetes deployment succeeds, but users receive HTTP 502. How do you investigate?
- How would you prevent a vulnerable or unsigned container from reaching production?
- How would you rotate an SSH key without causing an outage?
- How would you migrate an application to private subnets without breaking dependencies?
- A release causes a production incident. What is your rollback and incident-response plan?
- How would you design monitoring and alerting for a multi-tier application?
- How would you balance security enforcement, developer productivity, and delivery speed?

**Completion criteria:** Each answer includes a structured process, concrete evidence, trade-offs, and a safe remediation plan.

## Task 9.3 — Use Interview Feedback to Choose the Next Task

After every technical interview:
- [ ] Record questions you could not answer confidently.
- [ ] Classify the gap as conceptual, practical, or communication-related.
- [ ] Complete the smallest hands-on task that closes the gap.
- [ ] Add a sanitized example or note to your learning repository.
- [ ] Practice answering the question again.

**Completion criteria:** Interview feedback directly informs your next learning task.

---

# 📋 Task Tracker

Mark a task complete only when you can demonstrate its completion criteria.

## Job Search
- [ ] Task 1.1 — Create role requirements matrix
- [ ] Task 1.2 — Prepare both targeted resumes
- [ ] Task 1.3 — Upgrade GitHub profile
- [ ] Task 1.4 — Start job applications and maintain tracker

## Core Engineering
- [ ] Task 2.1 — Linux troubleshooting
- [ ] Task 2.2 — Bash automation
- [ ] Task 2.3 — Git and GitHub workflows
- [ ] Task 2.4 — Networking troubleshooting

## AWS and Terraform
- [ ] Task 3.1 — Secure AWS infrastructure baseline
- [ ] Task 3.2 — Reusable Terraform modules
- [ ] Task 3.3 — Terraform drift and recovery lab
- [ ] Task 3.4 — AWS security controls

## Docker and Kubernetes
- [ ] Task 4.1 — Production-quality Docker images
- [ ] Task 4.2 — Multi-component Kubernetes application
- [ ] Task 4.3 — Kubernetes troubleshooting lab
- [ ] Task 4.4 — Helm, scaling, and cluster operations

## CI/CD and GitOps
- [ ] Task 5.1 — Complete CI/CD pipeline
- [ ] Task 5.2 — Argo CD GitOps
- [ ] Task 5.3 — Release safety controls

## Cloud Security and DevSecOps
- [ ] Task 6.1 — Shift-left security gates
- [ ] Task 6.2 — Artifact signing
- [ ] Task 6.3 — TLS hardening
- [ ] Task 6.4 — Secrets and SSH governance
- [ ] Task 6.5 — Security testing and compliance evidence

## Observability and Reliability
- [ ] Task 7.1 — Monitoring
- [ ] Task 7.2 — Centralized logging
- [ ] Task 7.3 — Incident response

## Capstone and Interviews
- [ ] Phase 8 — End-to-end capstone
- [ ] Task 9.1 — Project walkthroughs
- [ ] Task 9.2 — Senior-level scenario practice
- [ ] Task 9.3 — Interview feedback loop

---

# 📁 Suggested GitHub Repository Structure

```text
devops-job-readiness/
├── README.md
├── job-readiness/
│   └── role-requirements-matrix.md
├── linux-troubleshooting/
├── automation/
├── git-workflows/
├── networking/
├── aws-secure-baseline/
├── terraform-aws-modules/
├── terraform-drift-lab/
├── aws-cloud-security/
├── docker-production/
├── kubernetes-production/
├── kubernetes-incident-labs/
├── helm-app-chart/
├── cicd-pipeline/
├── argocd-gitops/
├── release-engineering/
├── devsecops-security-gates/
├── artifact-signing/
├── tls-hardening/
├── secrets-governance/
├── security-test-framework/
├── observability-stack/
├── centralized-logging/
├── incident-response-labs/
└── capstone/
```

You can also keep separate repositories for major projects. Use this structure as a guide, not a requirement to create every directory immediately.

---

# ⚡ Recommended Execution Order

To move toward employment as quickly as possible:

1. Complete the job-targeting matrix.
2. Finalize both targeted resumes.
3. Improve your GitHub profile and select your strongest existing work.
4. Start applying to relevant vacancies immediately.
5. Build the Terraform drift and recovery lab.
6. Build the Kubernetes troubleshooting lab.
7. Implement a CI/CD pipeline with security checks.
8. Build the capstone incrementally.
9. Practice interviews throughout and close the gaps revealed by recruiters.

## Final Principle

DevOps is not about collecting tools or completing a fixed number of days. It is about ownership, automation, reliability, security, and the ability to diagnose and solve real problems. 
#TrainWithSubham

**Validate what you know. Build what you cannot yet demonstrate. Document what you build. Apply while you learn.**

One task at a time. One verified result at a time. One step closer to your next role.
