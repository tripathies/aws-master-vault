# Bucket 1 — Foundation & Security

> AWS Master Vault learning tracker. This category uses AWS-native services, identity models, networking and governance terminology.

## Category architecture

![Bucket 1 — Foundation & Security architecture](architecture.svg)

- [Editable category diagram](architecture.drawio)
- [Mermaid source](architecture.mmd)
- [Visual architecture library](../../VISUAL-DIAGRAMS.md)
- [Enterprise reference architecture](../../AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md)

## Component checklist

| Topic | Learning guide | Diagram (SVG) | Editable diagram |
|---|---|---|---|
| AWS account and root MFA | [Open guide](../../services/aws-account-and-root-mfa.md) | [View](../../services/aws-account-and-root-mfa/architecture.svg) | [draw.io](../../services/aws-account-and-root-mfa/architecture.drawio) |
| AWS IAM roles and policies | [Open guide](../../services/aws-iam-roles-and-policies.md) | [View](../../services/aws-iam-roles-and-policies/architecture.svg) | [draw.io](../../services/aws-iam-roles-and-policies/architecture.drawio) |
| IAM service roles: EC2 to S3 | [Open guide](../../services/iam-service-roles-ec2-to-s3.md) | [View](../../services/iam-service-roles-ec2-to-s3/architecture.svg) | [draw.io](../../services/iam-service-roles-ec2-to-s3/architecture.drawio) |
| AWS Secrets Manager | [Open guide](../../services/aws-secrets-manager.md) | [View](../../services/aws-secrets-manager/architecture.svg) | [draw.io](../../services/aws-secrets-manager/architecture.drawio) |
| Systems Manager Parameter Store | [Open guide](../../services/systems-manager-parameter-store.md) | [View](../../services/systems-manager-parameter-store/architecture.svg) | [draw.io](../../services/systems-manager-parameter-store/architecture.drawio) |
| AWS Organizations and SCPs | [Open guide](../../services/aws-organizations-and-scps.md) | [View](../../services/aws-organizations-and-scps/architecture.svg) | [draw.io](../../services/aws-organizations-and-scps/architecture.drawio) |
| AWS Control Tower | [Open guide](../../services/aws-control-tower.md) | [View](../../services/aws-control-tower/architecture.svg) | [draw.io](../../services/aws-control-tower/architecture.drawio) |
| AWS Budgets and billing alarms | [Open guide](../../services/aws-budgets-and-billing-alarms.md) | [View](../../services/aws-budgets-and-billing-alarms/architecture.svg) | [draw.io](../../services/aws-budgets-and-billing-alarms/architecture.drawio) |
| AWS KMS | [Open guide](../../services/aws-kms.md) | [View](../../services/aws-kms/architecture.svg) | [draw.io](../../services/aws-kms/architecture.drawio) |
| AWS IAM Identity Center | [Open guide](../../services/aws-iam-identity-center.md) | [View](../../services/aws-iam-identity-center/architecture.svg) | [draw.io](../../services/aws-iam-identity-center/architecture.drawio) |

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
