# Bucket 3 — Storage & Databases

> AWS Master Vault learning tracker. This category uses AWS-native services, identity models, networking and governance terminology.

## Category architecture

![Bucket 3 — Storage & Databases architecture](architecture.svg)

- [Editable category diagram](architecture.drawio)
- [Mermaid source](architecture.mmd)
- [Visual architecture library](../../VISUAL-DIAGRAMS.md)
- [Enterprise reference architecture](../../AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md)

## Component checklist

| Topic | Learning guide | Diagram (SVG) | Editable diagram |
|---|---|---|---|
| Amazon S3 | [Open guide](../../services/amazon-s3.md) | [View](../../services/amazon-s3/architecture.svg) | [draw.io](../../services/amazon-s3/architecture.drawio) |
| Amazon EBS | [Open guide](../../services/amazon-ebs.md) | [View](../../services/amazon-ebs/architecture.svg) | [draw.io](../../services/amazon-ebs/architecture.drawio) |
| Amazon EFS | [Open guide](../../services/amazon-efs.md) | [View](../../services/amazon-efs/architecture.svg) | [draw.io](../../services/amazon-efs/architecture.drawio) |
| Amazon RDS | [Open guide](../../services/amazon-rds.md) | [View](../../services/amazon-rds/architecture.svg) | [draw.io](../../services/amazon-rds/architecture.drawio) |
| Amazon Aurora | [Open guide](../../services/amazon-aurora.md) | [View](../../services/amazon-aurora/architecture.svg) | [draw.io](../../services/amazon-aurora/architecture.drawio) |
| Amazon DynamoDB | [Open guide](../../services/amazon-dynamodb.md) | [View](../../services/amazon-dynamodb/architecture.svg) | [draw.io](../../services/amazon-dynamodb/architecture.drawio) |
| Amazon ElastiCache | [Open guide](../../services/amazon-elasticache.md) | [View](../../services/amazon-elasticache/architecture.svg) | [draw.io](../../services/amazon-elasticache/architecture.drawio) |
| AWS Backup | [Open guide](../../services/aws-backup.md) | [View](../../services/aws-backup/architecture.svg) | [draw.io](../../services/aws-backup/architecture.drawio) |
| S3 events and Lambda | [Open guide](../../services/s3-events-and-lambda.md) | [View](../../services/s3-events-and-lambda/architecture.svg) | [draw.io](../../services/s3-events-and-lambda/architecture.drawio) |
| AWS Database Migration Service | [Open guide](../../services/aws-database-migration-service.md) | [View](../../services/aws-database-migration-service/architecture.svg) | [draw.io](../../services/aws-database-migration-service/architecture.drawio) |

## Practice workflow
1. Read the official documentation and note service scope, limits and alternatives.
2. Map identity, network paths, data flows, dependencies and ownership.
3. Complete a sandbox lab and capture validation evidence.
4. Test an access-denied or failure scenario where safe.
5. Record monitoring, cost observations and teardown proof.

## Official references
- [AWS documentation](https://docs.aws.amazon.com/)
- [Architecture framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
- [Pricing](https://aws.amazon.com/pricing/)

> Diagrams are conceptual learning resources, not production-certified designs. Verify service capabilities, IAM permissions, network behavior, quotas, regional availability and pricing before deployment.
