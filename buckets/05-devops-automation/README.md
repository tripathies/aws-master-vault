# Bucket 5 — DevOps & Automation

> Make infrastructure repeatable, deployments controlled, access auditable and operational tasks automated.

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
| [AWS CloudFormation](../../services/aws-cloudformation.md) | Provision and manage AWS infrastructure declaratively. | [Official docs](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html) |
| [AWS CDK with Python](../../services/aws-cdk-with-python.md) | Define supported infrastructure using Python constructs. | [Official docs](https://docs.aws.amazon.com/cdk/v2/guide/work-with-cdk-python.html) |
| [AWS CDK with TypeScript](../../services/aws-cdk-with-typescript.md) | Define supported infrastructure using TypeScript constructs. | [Official docs](https://docs.aws.amazon.com/cdk/v2/guide/work-with-cdk-typescript.html) |
| [AWS Systems Manager Session Manager](../../services/aws-systems-manager-session-manager.md) | Access supported instances without exposing SSH/RDP ports or managing bastion hosts. | [Official docs](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager.html) |
| [AWS CodePipeline](../../services/aws-codepipeline.md) | Orchestrate supported continuous delivery workflows. | [Official docs](https://docs.aws.amazon.com/codepipeline/latest/userguide/welcome.html) |
| [AWS CodeBuild](../../services/aws-codebuild.md) | Build and test application artifacts. | [Official docs](https://docs.aws.amazon.com/codebuild/latest/userguide/welcome.html) |
| [AWS CodeDeploy](../../services/aws-codedeploy.md) | Deploy supported application revisions to eligible targets. | [Official docs](https://docs.aws.amazon.com/codedeploy/latest/userguide/welcome.html) |
| [Amazon EventBridge](../../services/amazon-eventbridge.md) | Route events and trigger automation. | [Official docs](https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html) |
| [Terraform on AWS](../../services/terraform-on-aws.md) | Manage AWS infrastructure using Terraform configuration and state. | [Official docs](https://developer.hashicorp.com/terraform/tutorials/aws-get-started) |
| [GitHub Actions with AWS OIDC](../../services/github-actions-with-aws-oidc.md) | Use short-lived federated credentials for CI/CD rather than long-lived keys. | [Official docs](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_providers_create_oidc.html) |

## Delivery controls

Use reviewed code, separated environments, protected secrets, least-privilege deployment roles, artifact provenance, approval gates where needed, drift detection and rollback procedures. Infrastructure-as-code state and pipeline credentials must not be committed to the repository.

## Hands-on labs

1. Deploy a small stack with CloudFormation or CDK; review the generated resources before deploying.
2. Use Session Manager to access an eligible EC2 instance without opening inbound SSH, after configuring the required IAM and instance permissions.
3. Create a pipeline from GitHub to build a container, push to ECR and deploy to ECS. Use OIDC/temporary credentials where supported.
4. Create an EventBridge rule that triggers Lambda and validate permission, event matching, retries and dead-letter/error handling.
5. Add deployment validation and rollback expectations to the pipeline.

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
