# AWS Cost Management & Cleanup Checklist

AWS pricing and free-offer eligibility can change and vary by account, Region and usage. Check the [AWS Free Tier page](https://aws.amazon.com/free/) and current service pricing before each lab. Do not assume every service is free.

## Before deploying

- [ ] Choose a single learning Region unless the lab specifically needs multiple Regions.
- [ ] Check current free offer terms, quotas and pricing for each resource.
- [ ] Set an AWS Budget and notifications; consider a small threshold. Budget alerts are not a hard spend cap.
- [ ] Use tags such as `Project`, `Owner`, `Environment`, and `ExpiresOn` where supported.
- [ ] Prefer small, short-lived resources and stop/delete them immediately after the lab.
- [ ] Avoid deploying EKS, NAT Gateways, RDS, load balancers, SageMaker endpoints or large AI workloads without a clear need and cleanup plan.

## Common cost sources to inspect

- EC2 instances, EBS volumes and snapshots
- NAT Gateways and data processing/transfer
- Public IPv4 addresses, load balancers and endpoints
- RDS/Aurora instances, storage, I/O and backups
- EKS control plane, worker capacity and networking
- CloudWatch log ingestion, metrics and retention
- S3 storage, requests, replication and retrieval
- Bedrock inference, SageMaker endpoints and other metered AI services

## Teardown checklist

- [ ] Delete or destroy resources created by the lab's IaC stack first, where appropriate.
- [ ] Delete EC2 instances and unused EBS volumes/snapshots according to retention needs.
- [ ] Delete load balancers, target groups, NAT Gateways, unattached Elastic IPs and unneeded VPC endpoints.
- [ ] Delete RDS databases and snapshots only when no longer required; confirm final-snapshot choice deliberately.
- [ ] Delete ECS services/tasks, EKS clusters/node groups and ECR images when appropriate.
- [ ] Delete Lambda, API Gateway, Step Functions and EventBridge resources created for the lab.
- [ ] Inspect S3 buckets, replication rules, object versions and incomplete multipart uploads before deleting.
- [ ] Delete temporary SageMaker endpoints/configurations and AI resources after validation.
- [ ] Review CloudWatch log groups, custom metrics and retained logs.
- [ ] Check AWS Billing/Cost Explorer later for delayed or continuing charges.

## Useful official references

- [AWS Free Tier and current free offers](https://aws.amazon.com/free/)
- [CloudWatch billing alarms](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html)
- [AWS Budgets](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-managing-costs.html)
- [AWS Pricing Calculator](https://calculator.aws/)
- [AWS Billing and Cost Management](https://docs.aws.amazon.com/cost-management/)

> Deleting a resource can permanently remove data. Check retention and recovery requirements before deleting backups, snapshots, buckets or databases.
