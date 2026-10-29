# Bucket 1 — Foundation & Security

> Establish a safe AWS account baseline, identity controls, secrets handling and account-level guardrails.

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
| [AWS account and root MFA](../../services/aws-account-and-root-mfa.md) | Secure the account root user; enable MFA and avoid root access keys. | [Official docs](https://docs.aws.amazon.com/accounts/latest/reference/root-user.html) |
| [AWS IAM roles and policies](../../services/aws-iam-roles-and-policies.md) | Grant least-privilege access using roles, trust policies and permissions policies. | [Official docs](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html) |
| [IAM service roles: EC2 to S3](../../services/iam-service-roles-ec2-to-s3.md) | Let an EC2 workload access S3 using an instance profile instead of embedded credentials. | [Official docs](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use_switch-role-ec2.html) |
| [AWS Secrets Manager](../../services/aws-secrets-manager.md) | Store, retrieve and rotate supported application secrets. | [Official docs](https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html) |
| [Systems Manager Parameter Store](../../services/systems-manager-parameter-store.md) | Store application configuration and supported parameter types. | [Official docs](https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html) |
| [AWS Organizations and SCPs](../../services/aws-organizations-and-scps.md) | Organize accounts and set permission guardrails across an organization. | [Official docs](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_introduction.html) |
| [AWS Control Tower](../../services/aws-control-tower.md) | Establish and govern a multi-account landing zone. | [Official docs](https://docs.aws.amazon.com/controltower/latest/userguide/what-is-control-tower.html) |
| [AWS Budgets and billing alarms](../../services/aws-budgets-and-billing-alarms.md) | Create cost thresholds and notifications; alerts do not automatically stop spend. | [Official docs](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-managing-costs.html) |
| [AWS KMS](../../services/aws-kms.md) | Manage encryption keys and supported cryptographic operations. | [Official docs](https://docs.aws.amazon.com/kms/latest/developerguide/overview.html) |
| [AWS IAM Identity Center](../../services/aws-iam-identity-center.md) | Provide centralized workforce access to accounts and supported applications. | [Official docs](https://docs.aws.amazon.com/singlesignon/latest/userguide/what-is.html) |

## Day-one setup

- [ ] Create the AWS account and confirm account recovery details.
- [ ] Enable MFA for the root user; do not create root access keys.
- [ ] Configure a named administrator path using IAM Identity Center where appropriate.
- [ ] Set a budget and billing notifications. Billing alarms are alerts, not spending caps.
- [ ] Select a Region for learning and check service availability and pricing.
- [ ] Create a least-privilege role for the first workload; do not embed credentials.

## Design checks

- Root user: MFA, no access keys, tightly controlled recovery.
- Human access: prefer federation/Identity Center where feasible; avoid shared users.
- Workload access: temporary role credentials and least privilege.
- Secrets: never commit them; avoid logging secret values; rotate where supported and justified.
- Organization controls: SCPs set maximum permissions and do not grant permissions by themselves.

## Hands-on labs

1. Create a role with a narrowly scoped trust policy and permissions policy; explain both.
2. Configure an EC2 instance profile and allow the instance to read only a designated S3 prefix.
3. Store a sample non-production secret in Secrets Manager and retrieve it through an authorized SDK call.
4. Store non-secret configuration in Parameter Store; compare standard and advanced parameter considerations.
5. Set a budget and test notifications. Do not assume alerts stop resource creation.

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
