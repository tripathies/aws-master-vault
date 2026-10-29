# Bucket 7 — Monitoring & Cost

> Observe health, audit actions, respond to incidents and keep usage and cost under control.

[← Back to AWS learning tracker](../../README.md) · [Master architecture](../../AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md) · [Portfolio projects](../../PORTFOLIO-PROJECTS.md)

## Bucket tracker

- [ ] Explain the purpose and placement of each component.
- [ ] Describe alternatives and decision trade-offs.
- [ ] Explain IAM, network and data protection requirements.
- [ ] Complete at least one hands-on lab and capture validation evidence.
- [ ] Explain availability, failure behavior, monitoring and cost.
- [ ] Delete lab resources and confirm cleanup.
- [ ] Answer scenario-based interview questions.

## Core topics

| Topic | Purpose | Official reference |
|---|---|---|
| [Amazon CloudWatch metrics, logs and alarms](../../services/amazon-cloudwatch-metrics-logs-and-alarms.md) | Collect telemetry, query logs and alert on supported conditions. | [Official docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) |
| [CloudWatch dashboards](../../services/cloudwatch-dashboards.md) | Visualize operational signals. | [Official docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Dashboards.html) |
| [AWS Cost Explorer](../../services/aws-cost-explorer.md) | Analyze historical cost and usage. | [Official docs](https://docs.aws.amazon.com/cost-management/latest/userguide/ce-what-is.html) |
| [AWS Budgets](../../services/aws-budgets.md) | Set budget thresholds and notifications. | [Official docs](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-managing-costs.html) |
| [AWS CloudTrail](../../services/aws-cloudtrail.md) | Record supported AWS API activity for audit and investigation. | [Official docs](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-user-guide.html) |
| [AWS Config](../../services/aws-config.md) | Record configuration changes and evaluate supported rules. | [Official docs](https://docs.aws.amazon.com/config/latest/developerguide/WhatIsConfig.html) |
| [AWS Trusted Advisor](../../services/aws-trusted-advisor.md) | Review eligible best-practice checks. | [Official docs](https://docs.aws.amazon.com/awssupport/latest/user/trusted-advisor.html) |
| [AWS Compute Optimizer](../../services/aws-compute-optimizer.md) | Review supported rightsizing recommendations. | [Official docs](https://docs.aws.amazon.com/compute-optimizer/latest/ug/what-is-compute-optimizer.html) |
| [AWS Service Quotas](../../services/aws-service-quotas.md) | Review service quotas and request supported increases. | [Official docs](https://docs.aws.amazon.com/servicequotas/latest/userguide/intro.html) |
| [AWS Free Tier and free offers](../../services/aws-free-tier-and-free-offers.md) | Check current account eligibility, offer terms and usage limits before labs. | [Official docs](https://aws.amazon.com/free/) |

## Operational design

Define service-level indicators, alert owners, actionable thresholds, log retention and escalation paths. Monitor security events and audit trails separately from application health. Cost optimization must preserve workload reliability and security requirements.

## Hands-on labs

1. Create a CloudWatch alarm for an appropriate CPU, error-rate or application metric; verify the notification path.
2. Enable CloudTrail for the intended scope and verify delivery to a protected S3 destination when configured.
3. Create a monthly budget and notifications; understand that budgets alert rather than impose a hard cap.
4. Use Cost Explorer to inspect the lab account and tag resources for ownership.
5. Build a cleanup checklist and confirm there are no orphaned volumes, snapshots, addresses, load balancers, endpoints or log groups you no longer need.

## Scenario questions

1. **How would you choose between the services in this bucket?** Start with workload requirements, constraints, operational responsibility and failure tolerance. Compare two viable options and explain why one is a better fit.
2. **How do you secure the design?** Describe identity, least privilege, network/data boundaries, encryption, logging and configuration guardrails.
3. **How do you make the design reliable and cost-aware?** Identify failure domains, monitoring, backup/recovery requirements, scaling behavior and material cost drivers.
4. **What would you validate before production?** Confirm current service behavior, quotas, Region availability, IAM permissions, network paths, observability, rollback and teardown.

## Official learning resources

- [AWS documentation](https://docs.aws.amazon.com/)
- [AWS Skill Builder](https://skillbuilder.aws/)
- [AWS samples](https://github.com/aws-samples)
- [AWS re:Post](https://repost.aws/)
- [AWS Free Tier and current offers](https://aws.amazon.com/free/)
