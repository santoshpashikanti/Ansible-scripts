1) Pre-requisites you should decide upfront (avoid rework later)
A. Engine & workload

Engine: PostgreSQL / MySQL / MariaDB / SQL Server / Oracle / Aurora (separate service family).

Workload type: dev/test vs prod (drives HA, backups, monitoring, sizing).

B. Network placement

Choose VPC and subnets (best practice: private subnets across 2+ AZs).

Decide access:

Private (recommended): app connects from within VPC (EKS/ECS/EC2) via security groups.

Public (not recommended for prod): accessible from internet with strict IP allowlist.

C. Availability & resilience

Single-AZ (cheaper) vs Multi-AZ (recommended for prod).

Optional: read replicas for scale/read-heavy workloads.

D. Security & compliance defaults

KMS encryption at rest (enable).

TLS in transit (enforce).

Authentication: password + (optional) IAM DB authentication (engine-dependent).

Secrets: store in AWS Secrets Manager (recommended).

E. Operations

Backups retention (7–35 days typical; prod often 14–35).

Maintenance window.

Monitoring: Enhanced Monitoring, Performance Insights, CloudWatch alarms.
