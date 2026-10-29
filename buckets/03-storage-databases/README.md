# Bucket 3 — Storage & Databases

> Choose object, block, file, relational, key-value and caching services based on data access patterns, durability, consistency and recovery.

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
| [Amazon S3](../../services/amazon-s3.md) | Store objects with bucket policies, encryption, lifecycle and versioning controls. | [Official docs](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) |
| [Amazon EBS](../../services/amazon-ebs.md) | Provide block storage for EC2 and supported workloads. | [Official docs](https://docs.aws.amazon.com/ebs/latest/userguide/what-is-ebs.html) |
| [Amazon EFS](../../services/amazon-efs.md) | Provide elastic shared file storage for supported Linux workloads. | [Official docs](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) |
| [Amazon RDS](../../services/amazon-rds.md) | Run managed relational databases. | [Official docs](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) |
| [Amazon Aurora](../../services/amazon-aurora.md) | Run supported cloud-optimized relational workloads. | [Official docs](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html) |
| [Amazon DynamoDB](../../services/amazon-dynamodb.md) | Use a managed key-value and document database with access-pattern-driven design. | [Official docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html) |
| [Amazon ElastiCache](../../services/amazon-elasticache.md) | Cache eligible application data to reduce latency and backend load. | [Official docs](https://docs.aws.amazon.com/AmazonElastiCache/latest/dg/WhatIs.html) |
| [AWS Backup](../../services/aws-backup.md) | Centrally manage supported backup plans and recovery points. | [Official docs](https://docs.aws.amazon.com/aws-backup/latest/devguide/whatisbackup.html) |
| [S3 events and Lambda](../../services/s3-events-and-lambda.md) | Trigger processing from supported S3 object events. | [Official docs](https://docs.aws.amazon.com/lambda/latest/dg/with-s3.html) |
| [AWS Database Migration Service](../../services/aws-database-migration-service.md) | Migrate and replicate supported databases. | [Official docs](https://docs.aws.amazon.com/dms/latest/userguide/Welcome.html) |

## Data design decisions

Choose object vs block vs shared file vs relational vs key-value storage by access pattern, consistency, latency, durability, query needs and operational ownership. Backups, replication, versioning and high availability solve different problems; verify restore procedures rather than assuming a snapshot is a complete DR plan.

## Hands-on labs

1. Create a private S3 bucket, upload/download an object with an SDK, and verify public access is blocked.
2. Enable versioning and lifecycle rules only after deciding retention requirements; test recovery from an overwritten object.
3. Attach an EBS volume to a test EC2 instance, snapshot it, and document restore steps.
4. Mount EFS from two eligible EC2 clients and verify access controls.
5. Create a small RDS database in private subnets, permit access only from the application security group, connect from the app tier, then delete the stack.
6. Create a DynamoDB table based on access patterns; test CRUD and explain partition/sort keys and indexes.
7. Connect S3 events to Lambda with idempotency and failure handling in mind.

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
