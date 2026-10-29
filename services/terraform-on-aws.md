# Terraform on AWS

> Manage AWS infrastructure using Terraform configuration and state.

[← Bucket 5: DevOps & Automation](../buckets/05-devops-automation/README.md) · [AWS master tracker](../README.md) · [Enterprise reference architecture](../AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md)

## Purpose and architecture placement

Manage AWS infrastructure using Terraform configuration and state. In an enterprise design, place this service in the context of its caller, dependencies, security boundary, failure domain and operational owner. Confirm the required service capabilities and regional availability before selecting it.

## Core design questions

- What requirement does this service satisfy, and what is explicitly out of scope?
- What are the supported deployment models, interfaces, quotas and important limits?
- Which alternative services could meet the same need, and what trade-offs matter?
- Which account, Region, VPC/subnet, resource policy or trust boundary applies?

## Identity and security

- Prefer temporary credentials and IAM roles over long-lived access keys.
- Apply least privilege to identity policies and resource policies; distinguish permissions granted from organization guardrails that only restrict permissions.
- Enable encryption and logging using service-supported controls and organizational requirements.
- Protect secrets and sensitive data; avoid placing credentials in source code, user data or logs.
- Validate public exposure, resource policies, cross-account access and deletion protection where relevant.

## Network and data flow

Document the caller, destination, protocol/port, DNS name, route, endpoint and expected response. If private connectivity is required, validate service support, VPC endpoint/PrivateLink configuration, DNS, routing and resource policies together. Do not assume a private subnet alone creates private service access.

## Availability, scaling and recovery

Define the expected failure cases, health signals, scaling mechanism and recovery objectives. Determine whether the service is regional or global, how it handles AZ/Region failure, what must be backed up, and how restoration/failover will be tested. Service-specific behavior must be confirmed in the official documentation below.

## Cost and operations

Identify the principal billing dimensions, idle-resource costs, data transfer/requests/storage costs, log retention and quota risks. Add useful metrics, logs, alarms, dashboards and runbooks. Assign an owner to alerts and establish an actionable response.

## Hands-on learning checklist

- [ ] Read the official service overview and getting-started guide.
- [ ] Draw the service in a real request/data flow with dependencies.
- [ ] Deploy a minimal non-production example using a reviewed template or console steps.
- [ ] Validate permissions, network reachability, expected behavior and failure handling.
- [ ] Capture evidence without including secrets or sensitive data.
- [ ] Estimate costs and verify budgets/notifications.
- [ ] Delete lab resources and verify no billable resources remain.

## Interview practice

**Q: Why would you choose Terraform on AWS?**

**Model answer:** I would begin with the workload's functional and non-functional requirements, data and traffic patterns, security boundary, availability targets and operating model. I would compare viable alternatives, state the assumptions, identify the main failure and cost drivers, and validate service-specific limits before recommending a design.

**Q: What would you review before production?**

**Model answer:** IAM and resource policies, network and DNS paths, encryption and data handling, logging and alert ownership, quotas and regional support, backup/failover behavior, deployment rollback, and a tested cleanup/recovery procedure.

## Official reference

[Terraform on AWS — AWS documentation](https://developer.hashicorp.com/terraform/tutorials/aws-get-started)

## Learning status

- [ ] Purpose and alternatives understood
- [ ] Architecture diagram reviewed or created
- [ ] Security/network design reviewed
- [ ] Lab validated
- [ ] Cost and cleanup checked
- [ ] Interview scenario answered

> **Quality note:** This page is a structured learning guide, not a claim that a deployment sample has been production-tested. Verify the current AWS documentation and test all configuration in a non-production account.
