# DevOps & Automation

> Category learning tracker for AWS Master Vault. Service names and examples in this folder are AWS-specific.

## Category architecture

![DevOps & Automation architecture](architecture.svg)

- [Editable category diagram](architecture.drawio)
- [Mermaid source](architecture.mmd)
- [Full visual library](../../VISUAL-DIAGRAMS.md)
- [Master architecture](../../AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md)

## Component tracker

| Topic guide | SVG diagram | Editable draw.io |
|---|---|---|
| [AWS CloudFormation](../../services/aws-cloudformation.md) | [SVG](../../services/aws-cloudformation/architecture.svg) | [draw.io](../../services/aws-cloudformation/architecture.drawio) |
| [AWS CDK with Python](../../services/aws-cdk-with-python.md) | [SVG](../../services/aws-cdk-with-python/architecture.svg) | [draw.io](../../services/aws-cdk-with-python/architecture.drawio) |
| [AWS CDK with TypeScript](../../services/aws-cdk-with-typescript.md) | [SVG](../../services/aws-cdk-with-typescript/architecture.svg) | [draw.io](../../services/aws-cdk-with-typescript/architecture.drawio) |
| [AWS Systems Manager Session Manager](../../services/aws-systems-manager-session-manager.md) | [SVG](../../services/aws-systems-manager-session-manager/architecture.svg) | [draw.io](../../services/aws-systems-manager-session-manager/architecture.drawio) |
| [AWS CodePipeline](../../services/aws-codepipeline.md) | [SVG](../../services/aws-codepipeline/architecture.svg) | [draw.io](../../services/aws-codepipeline/architecture.drawio) |
| [AWS CodeBuild](../../services/aws-codebuild.md) | [SVG](../../services/aws-codebuild/architecture.svg) | [draw.io](../../services/aws-codebuild/architecture.drawio) |
| [AWS CodeDeploy](../../services/aws-codedeploy.md) | [SVG](../../services/aws-codedeploy/architecture.svg) | [draw.io](../../services/aws-codedeploy/architecture.drawio) |
| [Amazon EventBridge](../../services/amazon-eventbridge.md) | [SVG](../../services/amazon-eventbridge/architecture.svg) | [draw.io](../../services/amazon-eventbridge/architecture.drawio) |
| [Terraform on AWS](../../services/terraform-on-aws.md) | [SVG](../../services/terraform-on-aws/architecture.svg) | [draw.io](../../services/terraform-on-aws/architecture.drawio) |
| [GitHub Actions with AWS OIDC](../../services/github-actions-with-aws-oidc.md) | [SVG](../../services/github-actions-with-aws-oidc/architecture.svg) | [draw.io](../../services/github-actions-with-aws-oidc/architecture.drawio) |

## Practice workflow
1. Read the official documentation for each selected service.
2. Map its account/project boundary, identity, network and data flows.
3. Complete a sandbox lab and capture validation evidence.
4. Test one denied-access or failure scenario.
5. Record cost, teardown proof and design trade-offs.

## Official references
- [AWS documentation](https://docs.aws.amazon.com/)
- [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
- [AWS pricing](https://aws.amazon.com/pricing/)

> Diagram files are conceptual learning resources, not production-certified designs. Validate current service capabilities, permissions, routing, quotas, regional availability and prices before deployment.
