# 🚀 90 Tasks of DevOps
### Learn • I build • I practice • Document

A self-paced, hands-on DevOps learning roadmap organized into **90 technical tasks**. I complete each task in sequence, at my own pace. There is no daily schedule or fixed deadline.

The roadmap covers Linux, Bash scripting, networking, Git, AWS, Terraform, Docker, Kubernetes, CI/CD, GitOps, DevSecOps, observability, reliability, and an end-to-end capstone.

> I use the relevant TrainWithShubham training lessons and reference materials for the corresponding topics. I use the [TrainWithShubham #90DaysOfDevOps repository](https://github.com/TrainWithShubham/90DaysOfDevOps) as my reference for this practical, task-based learning roadmap.

## 📌 How to I use This Roadmap

- I complete tasks in order, or validate a task quickly if I already know the topic.
- I perform the practical work instead of only watching lessons.
- I document commands, configurations, test results, troubleshooting steps, and lessons learned.
- I never commit real credentials, private keys, access tokens, or sensitive infrastructure information.
- I use test environments and clean up billable cloud resources after practice.

### Definition of Done

For each task, I confirm that:
- [ ] I complete the hands-on exercise.
- [ ] I validate the result with appropriate commands or tests.
- [ ] I record the steps, result, and any troubleshooting performed.
- [ ] I save the relevant code, configuration, diagram, or notes in GitHub.

---

# 🐧 Module 1 — Linux Fundamentals and Troubleshooting

## Task 01 — Linux Environment and Filesystem
I explore the Linux directory structure, navigation, file creation, copying, moving, and deletion.

**My GitHub deliverable:** `task-01-linux-filesystem/README.md` with commands and examples.

## Task 02 — Users, Groups, and Permissions
I practice user and group management, ownership, `chmod`, `chown`, and `umask`.

**My GitHub deliverable:** Permission examples and a short troubleshooting guide.

## Task 03 — Processes and Services
I inspect processes using `ps`, `top`, and `pgrep`; manage services with `systemctl`.

**My GitHub deliverable:** Commands and evidence for starting, stopping, and diagnosing a service.

## Task 04 — I package Management
Install, update, inspect, and remove packages using the package manager available on your Linux distribution.

**My GitHub deliverable:** A package-management reference for my environment.

## Task 05 — Logs and Troubleshooting
I inspect system and application logs using `journalctl`, `dmesg`, and tools such as `grep`, `tail`, and `less`.

**My GitHub deliverable:** A documented example of diagnosing a service failure from logs.

## Task 06 — Disk and Filesystem Management
I use `df`, `du`, `lsblk`, and `find` to inspect disk usage and locate large files.

**My GitHub deliverable:** A disk-space troubleshooting runbook.

## Task 07 — CPU, Memory, and Resource Analysis
I inspect resource usage with `free`, `vmstat`, `uptime`, `top`, and related tools.

**My GitHub deliverable:** A sample resource investigation with findings and safe remediation.

## Task 08 — Linux Networking Commands
I practice `ip`, `ss`, `ping`, `curl`, `dig` or `nslookup`, and route inspection.

**My GitHub deliverable:** A networking command reference with sample outputs.

## Task 09 — SSH Administration
I configure SSH access, use key-based authentication, inspect permissions, and troubleshoot connection failures.

**My GitHub deliverable:** An SSH troubleshooting guide. Never upload private keys.

## Task 10 — Linux Incident Simulation
I create a safe test failure such as a stopped service, full test filesystem, or incorrect permission and diagnose it.

**My GitHub deliverable:** An incident report containing symptoms, evidence, root cause, fix, and verification.

---

# 🐚 Module 2 — Bash Scripting and Automation

## Task 11 — Bash Script Basics
I practice variables, arguments, quoting, exit codes, conditionals, and loops.

**My GitHub deliverable:** A collection of small, tested Bash scripts.

## Task 12 — File and Directory Automation
I write a script to organize files, check directory contents, and handle missing paths safely.

**My GitHub deliverable:** A reusable file-management script with usage instructions.

## Task 13 — Logging and Error Handling
I use functions, logging, exit codes, and safe shell options where appropriate.

**My GitHub deliverable:** A script that reports errors clearly and exits with meaningful status codes.

## Task 14 — System Health Check Script
I collect disk, memory, CPU, service, and filesystem information.

**My GitHub deliverable:** `system-health-check.sh` with sample output and test instructions.

## Task 15 — Backup and Retention Script
I create timestamped compressed backups and implement a configurable local retention policy.

**My GitHub deliverable:** `backup.sh` with validation, logging, failure handling, and restore instructions.

## Task 16 — AWS S3 Backup Automation
I extend a test backup workflow to upload archives to S3 and remove expired remote backups according to a documented retention policy.

**My GitHub deliverable:** Script, required IAM permissions, test evidence, and cleanup instructions. Protect the bucket and verify retention behavior before enabling deletion.

## Task 17 — Scheduling Automation
I schedule a test script using cron or an appropriate systemd timer.

**My GitHub deliverable:** Scheduling configuration, logs, and verification steps.

## Task 18 — API and HTTP Automation
I use `curl` to call a public or local test endpoint, check HTTP status codes, and handle failed requests.

**My GitHub deliverable:** A script that validates an endpoint and reports failures.

## Task 19 — Input Validation and Script Testing
I test missing arguments, invalid paths, permission failures, and command failures.

**My GitHub deliverable:** A test checklist and corrected scripts.

## Task 20 — Automation Capstone
I combine health checks, logging, backups, retention, and optional S3 integration into one maintainable workflow.

**My GitHub deliverable:** `linux-automation-capstone/` with scripts, documentation, test cases, and recovery instructions.

---

# 🌐 Module 3 — Networking Fundamentals

## Task 21 — IP Addressing and Subnetting
I practice IPv4 addresses, CIDR notation, subnet masks, network ranges, and usable addresses.

**My GitHub deliverable:** Subnetting examples and a small reference sheet.

## Task 22 — DNS Resolution
I inspect DNS records and diagnose incorrect or failed name resolution.

**My GitHub deliverable:** A DNS troubleshooting lab with evidence.

## Task 23 — TCP, UDP, and Ports
I explore connection behavior, listening ports, and common protocols.

**My GitHub deliverable:** A protocol and port reference with practical tests.

## Task 24 — Routing and Connectivity
I inspect routes and diagnose connectivity between test hosts or network namespaces.

**My GitHub deliverable:** A routing troubleshooting walkthrough.

## Task 25 — HTTP and HTTPS
I inspect request methods, response codes, headers, redirects, and TLS certificates using `curl` and browser or command-line tools.

**My GitHub deliverable:** HTTP/HTTPS test results and explanations.

## Task 26 — TLS and Certificate Validation
I inspect certificate chains, expiration, hostnames, and supported TLS versions using appropriate tools.

**My GitHub deliverable:** A TLS troubleshooting guide using test endpoints.

## Task 27 — Firewall Rules
I configure and validate host firewall rules in a safe environment.

**My GitHub deliverable:** A minimal firewall configuration and connectivity tests.

## Task 28 — Reverse Proxy and Load Balancing
I deploy a simple reverse proxy or load balancer for a test application.

**My GitHub deliverable:** Configuration, architecture diagram, and routing tests.

## Task 29 — Network Troubleshooting Scenarios
I diagnose test cases involving DNS failure, blocked ports, incorrect routes, and HTTP errors.

**My GitHub deliverable:** A scenario-based troubleshooting playbook.

## Task 30 — Networking Mini Project
I deploy a small application with a reverse proxy, DNS or host-based routing as appropriate, and restricted network access.

**My GitHub deliverable:** Architecture diagram, configuration, tests, and teardown instructions.

---

# 🔀 Module 4 — Git and GitHub

## Task 31 — Git Basics
I practice repositories, staging, commits, status, logs, and diffs.

**My GitHub deliverable:** A repository showing a clear, meaningful commit history.

## Task 32 — Branching and Merging
I create feature branches, merge changes, and resolve a deliberate conflict.

**My GitHub deliverable:** A documented branch and merge exercise.

## Task 33 — Remote Repositories
I practice clone, fetch, pull, push, and upstream tracking.

**My GitHub deliverable:** A workflow reference with example commands.

## Task 34 — Undo and Recovery
I practice safe use of `git restore`, `git revert`, and reset in a disposable repository.

**My GitHub deliverable:** Recovery scenarios explaining when each command is appropriate.

## Task 35 — Pull Requests and Code Review
I create a feature branch, open a pull request, review changes, and merge them.

**My GitHub deliverable:** A documented pull-request workflow.

## Task 36 — `.gitignore` and Secret Prevention
Exclude generated files, local configuration, and sensitive files. I practice secret scanning with safe test values.

**My GitHub deliverable:** A secure repository template and prevention checklist.

## Task 37 — Git Tags and Releases
Tag a release and document versioning and release notes.

**My GitHub deliverable:** A sample release with a tag and changelog.

## Task 38 — GitHub Actions Basics
I create a workflow that runs automatically on a push or pull request.

**My GitHub deliverable:** A working workflow file with execution evidence.

## Task 39 — Repository Documentation
I write a professional README with prerequisites, setup, commands, validation, troubleshooting, and cleanup.

**My GitHub deliverable:** A reusable README template.

## Task 40 — Git Workflow Mini Project
I build a repository workflow with branches, review, automated checks, release tags, and documentation.

**My GitHub deliverable:** A sample project showing the complete workflow.

---

# ☁️ Module 5 — AWS and Cloud Infrastructure

## Task 41 — AWS IAM
I practice users, roles, policies, trust policies, and least-privilege access in a test account.

**My GitHub deliverable:** Example policies with explanations and permission-validation steps.

## Task 42 — VPC and Subnets
I design a VPC with public and private subnets, CIDR ranges, and availability-zone considerations.

**My GitHub deliverable:** Network architecture diagram and configuration.

## Task 43 — Routing and Internet Access
I configure route tables, Internet Gateway, and NAT access where required.

**My GitHub deliverable:** Routing design and connectivity verification.

## Task 44 — EC2 and Secure Access
Launch a test EC2 instance using appropriate IAM, security groups, and secure administrative access.

**My GitHub deliverable:** Deployment instructions, validation evidence, and teardown steps.

## Task 45 — S3 Security
I configure bucket access, Block Public Access, encryption, and appropriate bucket policies.

**My GitHub deliverable:** A secure test bucket configuration and access tests.

## Task 46 — Load Balancing and Auto Scaling
I deploy a test application behind an ALB and explore health checks and scaling behavior.

**My GitHub deliverable:** Architecture, health-check evidence, and cost-aware cleanup steps.

## Task 47 — RDS and Data Protection
I explore a test database deployment, subnet placement, security groups, backups, and restore concepts.

**My GitHub deliverable:** Database architecture and data-protection notes. I avoid unnecessary long-running resources.

## Task 48 — CloudWatch and CloudTrail
I configure relevant metrics, logs, alarms, and audit-event investigation.

**My GitHub deliverable:** A monitoring and audit walkthrough with sample evidence.

## Task 49 — AWS Security Findings
I explore applicable security services and investigate a safe test finding or sample finding.

**My GitHub deliverable:** Finding analysis, risk explanation, remediation, and verification.

## Task 50 — Secure AWS Architecture Mini Project
I deploy a small application using controlled network access, IAM roles, encryption, logging, and documented teardown.

**My GitHub deliverable:** Terraform or deployment configuration, diagram, security decisions, and test results.

---

# 🏗️ Module 6 — Terraform and Infrastructure as Code

## Task 51 — Terraform Setup and Workflow
Install Terraform, configure the AWS provider, and practice `init`, `fmt`, `validate`, `plan`, and `apply`.

**My GitHub deliverable:** A minimal working Terraform configuration and command reference.

## Task 52 — Variables and Outputs
I use variables, outputs, locals, types, and validation.

**My GitHub deliverable:** A reusable configuration with documented inputs and outputs.

## Task 53 — Resources and Data Sources
I create resources and use data sources to reference existing infrastructure.

**My GitHub deliverable:** A small infrastructure configuration with explanations.

## Task 54 — Modules
I create reusable modules for networking, security groups, IAM, or compute.

**My GitHub deliverable:** Module source, example usage, and validation steps.

## Task 55 — Remote State and State Protection
I configure an S3 remote backend with appropriate encryption, access restrictions, and supported state locking.

**My GitHub deliverable:** Backend setup guide and state-security checklist. Do not commit state files containing sensitive data.

## Task 56 — Environments and Reuse
Organize environment-specific values and shared modules using a deliberate repository and state strategy.

**My GitHub deliverable:** Example development and test configurations.

## Task 57 — Terraform Drift
Change a disposable resource manually in AWS and inspect what `terraform plan` detects.

**My GitHub deliverable:** Before-and-after plans and an explanation of configuration, state, and actual infrastructure.

## Task 58 — Deleted Resource Recovery
Delete a Terraform-managed test resource through the AWS console, review the plan, and safely recreate or recover the desired state.

**My GitHub deliverable:** A recovery runbook. Explain when import or state repair is appropriate; do not modify production state.

## Task 59 — Terraform Quality and Security
I add formatting, validation, linting, and IaC security scanning to a test workflow.

**My GitHub deliverable:** A validation pipeline and sample results.

## Task 60 — Terraform AWS Infrastructure Project
Provision a small, reusable AWS environment with networking, IAM, compute, logging, and safe teardown.

**My GitHub deliverable:** `terraform-aws-project/` with modules, examples, architecture, validation, and recovery instructions.

---

# 🐳 Module 7 — Docker and Containerization

## Task 61 — Docker Fundamentals
I practice images, containers, ports, environment variables, volumes, and container lifecycle commands.

**My GitHub deliverable:** A Docker command reference and working examples.

## Task 62 — Dockerfile Design
I build an application image with appropriate layers, caching, and a clear startup command.

**My GitHub deliverable:** Dockerfile, build instructions, and application verification.

## Task 63 — Multi-Stage Builds
I use a multi-stage Dockerfile to separate build dependencies from the runtime image.

**My GitHub deliverable:** Dockerfile and comparison of image size or contents.

## Task 64 — Container Networking
I practice bridge networks, port publishing, name resolution, and service-to-service connectivity.

**My GitHub deliverable:** A multi-container networking example.

## Task 65 — Volumes and Persistence
Persist application data using Docker volumes or suitable bind mounts.

**My GitHub deliverable:** Persistence and recovery demonstration.

## Task 66 — Docker Compose
I deploy a multi-container application using Docker Compose.

**My GitHub deliverable:** Compose configuration, environment template, and startup/cleanup instructions.

## Task 67 — Container Security
I run as non-root, minimize image contents, avoid embedding secrets, and scan images for vulnerabilities.

**My GitHub deliverable:** Security improvements and scan results.

## Task 68 — Image Registry and Versioning
I tag and push an image to a registry, then pull and run a specific version.

**My GitHub deliverable:** Registry workflow and image-versioning documentation. Do not commit registry credentials.

## Task 69 — Container Troubleshooting
I diagnose a failed build, exited container, port conflict, health-check failure, and storage issue.

**My GitHub deliverable:** A troubleshooting guide with reproducible cases.

## Task 70 — Containerized Application Project
I package a small application with a secure image, persistent data where needed, Compose, health checks, and documentation.

**My GitHub deliverable:** `docker-application/` with source, Dockerfiles, configuration, tests, and cleanup instructions.

---

# ☸️ Module 8 — Kubernetes, Helm, and GitOps

## Task 71 — Kubernetes Cluster and Workloads
I use a local Kind cluster or an appropriate test cluster to inspect nodes, namespaces, Pods, and Deployments.

**My GitHub deliverable:** Cluster setup and workload deployment guide.

## Task 72 — Services and Internal DNS
I create ClusterIP and NodePort Services and verify selectors, endpoints, ports, and DNS.

**My GitHub deliverable:** Service networking lab with connectivity tests.

## Task 73 — Configuration and Secrets
I use ConfigMaps and Kubernetes Secrets appropriately, and explain their security limitations and encryption requirements.

**My GitHub deliverable:** Example application configuration without real credentials.

## Task 74 — Probes and Resource Controls
I configure readiness, liveness, and startup probes, along with resource requests and limits.

**My GitHub deliverable:** Working manifests and tests demonstrating the behavior.

## Task 75 — Ingress and HTTP Routing
I configure an Ingress controller or supported gateway, route traffic to multiple services, and troubleshoot path-based routing.

**My GitHub deliverable:** Ingress configuration, request tests, and a routing troubleshooting guide.

## Task 76 — Persistent Storage
I practice PersistentVolumes, PersistentVolumeClaims, StorageClasses, and storage troubleshooting.

**My GitHub deliverable:** A stateful workload example with persistence validation.

## Task 77 — Kubernetes Security
I configure service accounts, RBAC, security contexts, and network restrictions where supported.

**My GitHub deliverable:** Least-privilege examples and authorization tests.

## Task 78 — Autoscaling and Availability
I explore metrics availability, Horizontal Pod Autoscaler, disruption budgets, and scheduling behavior.

**My GitHub deliverable:** Scaling experiment with prerequisites, evidence, and limitations documented.

## Task 79 — Helm and Argo CD
I package an application as a Helm chart and deploy it through Argo CD GitOps.

**My GitHub deliverable:** Helm chart, environment values, Argo CD application configuration, and rollout evidence.

## Task 80 — Kubernetes Troubleshooting Project
I reproduce at least five issues, such as `CrashLoopBackOff`, `ImagePullBackOff`, Pending Pods, failed Ingress routing, or unavailable metrics. Diagnose, fix, and verify each.

**My GitHub deliverable:** `kubernetes-troubleshooting/` with manifests, commands, findings, and recovery runbooks.

---

# 🔐 Module 9 — CI/CD, DevSecOps, and Observability

## Task 81 — CI Pipeline
I build a Jenkins or GitHub Actions pipeline that runs linting and tests on pull requests.

**My GitHub deliverable:** Pipeline configuration, test output, and failure-handling notes.

## Task 82 — Automated Container Delivery
I extend the pipeline to build, scan, tag, and publish a container image to a registry.

**My GitHub deliverable:** Pipeline with versioned artifacts and documented credentials handling.

## Task 83 — Continuous Deployment and Rollback
I deploy an application to a test environment, verify its health, and test a controlled rollback.

**My GitHub deliverable:** Deployment pipeline, validation evidence, and rollback runbook.

## Task 84 — DevSecOps Security Gates
I integrate suitable source, dependency, secret, IaC, and image scanning. Generate an SBOM where appropriate.

**My GitHub deliverable:** Security pipeline, sample findings, remediation evidence, and documented gate thresholds.

## Task 85 — Artifact Signing and Verification
I compare relevant signing approaches, sign a test container image, and verify it before deployment.

**My GitHub deliverable:** Signing implementation, trust policy, verification commands, and a comparison matrix.

## Task 86 — TLS and Secrets Governance
I document endpoint TLS requirements, test supported protocol and certificate settings, and build a safe test secret-rotation workflow.

**My GitHub deliverable:** TLS policy matrix, verification results, secret-access design, and rotation runbook.

## Task 87 — Metrics, Dashboards, and Alerts
I deploy Prometheus and Grafana or an equivalent monitoring solution, build useful dashboards, and configure actionable alerts.

**My GitHub deliverable:** Monitoring configuration, dashboards, alert rules, and failure-test evidence.

## Task 88 — Centralized Logging and Incident Response
I collect test application logs centrally, investigate a simulated failure, and write an incident report.

**My GitHub deliverable:** Logging configuration, queries, incident timeline, root cause, remediation, and preventive actions.

---

# 🏆 Module 10 — Integrated Capstone

## Task 89 — I build a Secure Cloud-Native Delivery Platform

I integrate the strongest components from the earlier tasks into one end-to-end project.

**Required components**
- [ ] AWS networking and least-privilege IAM
- [ ] Terraform-managed infrastructure
- [ ] A containerized application
- [ ] Kubernetes deployment using EKS or a clearly documented local implementation for the initial version
- [ ] CI pipeline with tests and security checks
- [ ] Image registry and artifact verification
- [ ] GitOps deployment where supported
- [ ] Metrics, dashboards, logs, and alerts
- [ ] Failure testing, recovery instructions, and cleanup steps

**Completion criteria**
- [ ] A reader can follow my documentation to reproduce the deployment.
- [ ] A code change passes through the documented pipeline.
- [ ] Invalid changes or failed tests are blocked by the relevant gates.
- [ ] Application health can be verified.
- [ ] At least two failure scenarios are reproduced and resolved.
- [ ] Cost controls, security limitations, and teardown are documented.

**My GitHub deliverable:** `capstone/` with application code, Terraform, container files, pipeline configuration, Kubernetes or Helm manifests, security checks, architecture diagram, monitoring, incident reports, and setup instructions.

## Task 90 — Validate, Document, and Improve the Capstone

**My tasks**
- [ ] I test the documented setup from a clean environment where practical.
- [ ] I validate the expected application behavior.
- [ ] I review IAM permissions, exposed endpoints, secret handling, and image security.
- [ ] I test deployment failure and rollback.
- [ ] Verify monitoring, logs, and incident instructions.
- [ ] I remove temporary resources and document teardown.
- [ ] Improve the README, architecture diagram, and troubleshooting guide.
- [ ] I record limitations and sensible next improvements.

**My completion criteria:** The project is reproducible, documented, security-conscious, and explainable from architecture through incident recovery.

**My GitHub deliverable:** A final capstone README with architecture, prerequisites, deployment instructions, validation evidence, security decisions, troubleshooting, cleanup, and future improvements.

---

# 📁 Suggested Repository Structure

```text
devops-90-tasks/
├── README.md
├── task-01-linux-filesystem/
├── task-02-linux-permissions/
├── task-03-processes-services/
├── ...
├── task-10-linux-incident/
├── task-11-bash-basics/
├── ...
├── task-20-automation-capstone/
├── task-21-ip-subnetting/
├── ...
├── task-30-networking-project/
├── task-31-git-basics/
├── ...
├── task-40-git-workflow-project/
├── task-41-aws-iam/
├── ...
├── task-50-aws-security-project/
├── task-51-terraform-basics/
├── ...
├── task-60-terraform-project/
├── task-61-docker-basics/
├── ...
├── task-70-docker-project/
├── task-71-kubernetes-workloads/
├── ...
├── task-80-kubernetes-troubleshooting/
├── task-81-ci-pipeline/
├── ...
├── task-88-incident-response/
├── task-89-capstone/
└── task-90-capstone-validation/
```

I create folders as I start each task; I do not need to create every directory in advance.

---

# ✅ Progress Tracker

## Linux and Automation
- [ ] 01 Linux filesystem
- [ ] 02 Users, groups, and permissions
- [ ] 03 Processes and services
- [ ] 04 I package management
- [ ] 05 Logs and troubleshooting
- [ ] 06 Disk and filesystems
- [ ] 07 CPU and memory analysis
- [ ] 08 Linux networking commands
- [ ] 09 SSH administration
- [ ] 10 Linux incident simulation
- [ ] 11 Bash basics
- [ ] 12 File automation
- [ ] 13 Logging and error handling
- [ ] 14 System health script
- [ ] 15 Backup and retention
- [ ] 16 S3 backup automation
- [ ] 17 Scheduling
- [ ] 18 HTTP automation
- [ ] 19 Script testing
- [ ] 20 Automation capstone

## Networking and Git
- [ ] 21 IP addressing and subnetting
- [ ] 22 DNS
- [ ] 23 TCP, UDP, and ports
- [ ] 24 Routing
- [ ] 25 HTTP and HTTPS
- [ ] 26 TLS certificates
- [ ] 27 Firewall rules
- [ ] 28 Reverse proxy and load balancing
- [ ] 29 Network troubleshooting
- [ ] 30 Networking mini project
- [ ] 31 Git basics
- [ ] 32 Branching and merging
- [ ] 33 Remote repositories
- [ ] 34 Undo and recovery
- [ ] 35 Pull requests and code review
- [ ] 36 `.gitignore` and secret prevention
- [ ] 37 Tags and releases
- [ ] 38 GitHub Actions basics
- [ ] 39 Repository documentation
- [ ] 40 Git workflow project

## AWS and Terraform
- [ ] 41 AWS IAM
- [ ] 42 VPC and subnets
- [ ] 43 Routing and Internet access
- [ ] 44 EC2 and secure access
- [ ] 45 S3 security
- [ ] 46 Load balancing and Auto Scaling
- [ ] 47 RDS and data protection
- [ ] 48 CloudWatch and CloudTrail
- [ ] 49 AWS security findings
- [ ] 50 Secure AWS mini project
- [ ] 51 Terraform workflow
- [ ] 52 Variables and outputs
- [ ] 53 Resources and data sources
- [ ] 54 Modules
- [ ] 55 Remote state
- [ ] 56 Environments and reuse
- [ ] 57 Terraform drift
- [ ] 58 Deleted-resource recovery
- [ ] 59 Terraform quality and security
- [ ] 60 Terraform AWS project

## Docker and Kubernetes
- [ ] 61 Docker fundamentals
- [ ] 62 Dockerfile design
- [ ] 63 Multi-stage builds
- [ ] 64 Container networking
- [ ] 65 Volumes and persistence
- [ ] 66 Docker Compose
- [ ] 67 Container security
- [ ] 68 Image registry and versioning
- [ ] 69 Container troubleshooting
- [ ] 70 Containerized application
- [ ] 71 Kubernetes cluster and workloads
- [ ] 72 Services and internal DNS
- [ ] 73 ConfigMaps and Secrets
- [ ] 74 Probes and resource controls
- [ ] 75 Ingress and routing
- [ ] 76 Persistent storage
- [ ] 77 Kubernetes security
- [ ] 78 Autoscaling and availability
- [ ] 79 Helm and Argo CD
- [ ] 80 Kubernetes troubleshooting project

## CI/CD, Security, and Capstone
- [ ] 81 CI pipeline
- [ ] 82 Automated container delivery
- [ ] 83 Deployment and rollback
- [ ] 84 DevSecOps security gates
- [ ] 85 Artifact signing
- [ ] 86 TLS and secrets governance
- [ ] 87 Monitoring and alerting
- [ ] 88 Logging and incident response
- [ ] 89 Secure cloud-native capstone
- [ ] 90 Capstone validation and documentation

---

## 🎯 Final Principle

DevOps is not about collecting tools or finishing a fixed number of days. It is about automation, reliability, security, repeatability, and solving real operational problems.

**One task at a time. One verified result at a time.**
