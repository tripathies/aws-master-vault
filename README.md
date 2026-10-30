# AWS Master Vault

> **AWS Solution Architect learning portal** — track your learning, explore the enterprise reference design, and open focused guides for cloud-native topics.

[![Learning tracker](https://img.shields.io/badge/Learning%20tracker-open%20checklist-FF9900?style=for-the-badge)](#your-aws-learning-tracker)
[![Reference architecture](https://img.shields.io/badge/Reference%20architecture-open%20design-107C10?style=for-the-badge)](AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md)
[![Visual library](https://img.shields.io/badge/Diagrams-SVG%20%7C%20draw.io-7F56D9?style=for-the-badge)](VISUAL-DIAGRAMS.md)

## Start here

| <div align="center">📚 Learning tracker</div> | <div align="center">🏗️ End-to-end design</div> | <div align="center">🗺️ Diagram library</div> |
|---|---|---|
| Work through the catalogue by category. Each topic links to its guide. | Explore how governance, identity, networking, workloads, data, security and operations fit together. | Preview architecture diagrams and open editable draw.io sources. |
| [**Track topics below ↓**](#your-aws-learning-tracker) | [**Open reference design →**](AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md) | [**Open visual library →**](VISUAL-DIAGRAMS.md) |

![AWS Master Vault architecture overview](architecture.svg)

## Catalogue overview

**Catalogue size:** 70 service/topic guides across 7 learning categories.

| Domain | Category | Topics | Tracker |
|---|---|---:|---|
| **01** | [Foundation & Security](buckets/01-foundation-security/README.md) | 10 | [Open tracker](buckets/01-foundation-security/README.md) |
| **02** | [Compute & Containers](buckets/02-compute-containers/README.md) | 10 | [Open tracker](buckets/02-compute-containers/README.md) |
| **03** | [Storage & Databases](buckets/03-storage-databases/README.md) | 10 | [Open tracker](buckets/03-storage-databases/README.md) |
| **04** | [Networking & Content Delivery](buckets/04-networking-content-delivery/README.md) | 10 | [Open tracker](buckets/04-networking-content-delivery/README.md) |
| **05** | [DevOps & Automation](buckets/05-devops-automation/README.md) | 10 | [Open tracker](buckets/05-devops-automation/README.md) |
| **06** | [AI & Machine Learning](buckets/06-ai-machine-learning/README.md) | 10 | [Open tracker](buckets/06-ai-machine-learning/README.md) |
| **07** | [Monitoring & Cost](buckets/07-monitoring-cost/README.md) | 10 | [Open tracker](buckets/07-monitoring-cost/README.md) |


## Your AWS learning tracker

**Learning loop:** understand the purpose and trade-offs → inspect the diagram → complete a lab → validate the result → clean up resources → explain the design.

Progress checkboxes are Markdown checklist items, not a synced personal dashboard. Use your own branch/fork to track your progress.

<details>
<summary><strong>Bucket 1 — Foundation & Security</strong> · 10 topics</summary>

- [ ] [AWS account and root MFA](services/aws-account-and-root-mfa.md)
- [ ] [AWS IAM roles and policies](services/aws-iam-roles-and-policies.md)
- [ ] [IAM service roles: EC2 to S3](services/iam-service-roles-ec2-to-s3.md)
- [ ] [AWS Secrets Manager](services/aws-secrets-manager.md)
- [ ] [Systems Manager Parameter Store](services/systems-manager-parameter-store.md)
- [ ] [AWS Organizations and SCPs](services/aws-organizations-and-scps.md)
- [ ] [AWS Control Tower](services/aws-control-tower.md)
- [ ] [AWS Budgets and billing alarms](services/aws-budgets-and-billing-alarms.md)
- [ ] [AWS KMS](services/aws-kms.md)
- [ ] [AWS IAM Identity Center](services/aws-iam-identity-center.md)

[Open bucket guide](buckets/01-foundation-security/README.md)

</details>

<details>
<summary><strong>Bucket 2 — Compute & Containers</strong> · 10 topics</summary>

- [ ] [Amazon EC2](services/amazon-ec2.md)
- [ ] [EC2 Auto Scaling](services/ec2-auto-scaling.md)
- [ ] [AWS Lambda](services/aws-lambda.md)
- [ ] [Amazon ECS](services/amazon-ecs.md)
- [ ] [AWS Fargate](services/aws-fargate.md)
- [ ] [Amazon ECR](services/amazon-ecr.md)
- [ ] [Amazon EKS](services/amazon-eks.md)
- [ ] [Amazon EC2 GPU instances](services/amazon-ec2-gpu-instances.md)
- [ ] [AWS Batch](services/aws-batch.md)
- [ ] [AWS App Runner](services/aws-app-runner.md)

[Open bucket guide](buckets/02-compute-containers/README.md)

</details>

<details>
<summary><strong>Bucket 3 — Storage & Databases</strong> · 10 topics</summary>

- [ ] [Amazon S3](services/amazon-s3.md)
- [ ] [Amazon EBS](services/amazon-ebs.md)
- [ ] [Amazon EFS](services/amazon-efs.md)
- [ ] [Amazon RDS](services/amazon-rds.md)
- [ ] [Amazon Aurora](services/amazon-aurora.md)
- [ ] [Amazon DynamoDB](services/amazon-dynamodb.md)
- [ ] [Amazon ElastiCache](services/amazon-elasticache.md)
- [ ] [AWS Backup](services/aws-backup.md)
- [ ] [S3 events and Lambda](services/s3-events-and-lambda.md)
- [ ] [AWS Database Migration Service](services/aws-database-migration-service.md)

[Open bucket guide](buckets/03-storage-databases/README.md)

</details>

<details>
<summary><strong>Bucket 4 — Networking & Content Delivery</strong> · 10 topics</summary>

- [ ] [Amazon VPC](services/amazon-vpc.md)
- [ ] [Security Groups vs Network ACLs](services/security-groups-vs-network-acls.md)
- [ ] [Application Load Balancer](services/application-load-balancer.md)
- [ ] [Network Load Balancer](services/network-load-balancer.md)
- [ ] [Amazon Route 53](services/amazon-route-53.md)
- [ ] [Amazon CloudFront](services/amazon-cloudfront.md)
- [ ] [Amazon API Gateway](services/amazon-api-gateway.md)
- [ ] [AWS NAT Gateway](services/aws-nat-gateway.md)
- [ ] [AWS Transit Gateway](services/aws-transit-gateway.md)
- [ ] [AWS PrivateLink and VPC endpoints](services/aws-privatelink-and-vpc-endpoints.md)

[Open bucket guide](buckets/04-networking-content-delivery/README.md)

</details>

<details>
<summary><strong>Bucket 5 — DevOps & Automation</strong> · 10 topics</summary>

- [ ] [AWS CloudFormation](services/aws-cloudformation.md)
- [ ] [AWS CDK with Python](services/aws-cdk-with-python.md)
- [ ] [AWS CDK with TypeScript](services/aws-cdk-with-typescript.md)
- [ ] [AWS Systems Manager Session Manager](services/aws-systems-manager-session-manager.md)
- [ ] [AWS CodePipeline](services/aws-codepipeline.md)
- [ ] [AWS CodeBuild](services/aws-codebuild.md)
- [ ] [AWS CodeDeploy](services/aws-codedeploy.md)
- [ ] [Amazon EventBridge](services/amazon-eventbridge.md)
- [ ] [Terraform on AWS](services/terraform-on-aws.md)
- [ ] [GitHub Actions with AWS OIDC](services/github-actions-with-aws-oidc.md)

[Open bucket guide](buckets/05-devops-automation/README.md)

</details>

<details>
<summary><strong>Bucket 6 — AI & Machine Learning</strong> · 10 topics</summary>

- [ ] [Amazon Bedrock](services/amazon-bedrock.md)
- [ ] [Amazon Bedrock API and SDK](services/amazon-bedrock-api-and-sdk.md)
- [ ] [Amazon SageMaker AI](services/amazon-sagemaker-ai.md)
- [ ] [SageMaker AI endpoints](services/sagemaker-ai-endpoints.md)
- [ ] [Amazon Textract](services/amazon-textract.md)
- [ ] [Amazon Rekognition](services/amazon-rekognition.md)
- [ ] [Amazon Comprehend](services/amazon-comprehend.md)
- [ ] [Amazon Q Developer](services/amazon-q-developer.md)
- [ ] [Retrieval-augmented generation (RAG)](services/retrieval-augmented-generation-rag.md)
- [ ] [AI document-processing workflow](services/ai-document-processing-workflow.md)

[Open bucket guide](buckets/06-ai-machine-learning/README.md)

</details>

<details>
<summary><strong>Bucket 7 — Monitoring & Cost</strong> · 10 topics</summary>

- [ ] [Amazon CloudWatch metrics, logs and alarms](services/amazon-cloudwatch-metrics-logs-and-alarms.md)
- [ ] [CloudWatch dashboards](services/cloudwatch-dashboards.md)
- [ ] [AWS Cost Explorer](services/aws-cost-explorer.md)
- [ ] [AWS Budgets](services/aws-budgets.md)
- [ ] [AWS CloudTrail](services/aws-cloudtrail.md)
- [ ] [AWS Config](services/aws-config.md)
- [ ] [AWS Trusted Advisor](services/aws-trusted-advisor.md)
- [ ] [AWS Compute Optimizer](services/aws-compute-optimizer.md)
- [ ] [AWS Service Quotas](services/aws-service-quotas.md)
- [ ] [AWS Free Tier and free offers](services/aws-free-tier-and-free-offers.md)

[Open bucket guide](buckets/07-monitoring-cost/README.md)

</details>

## Seven portfolio projects

1. [Three-Tier Web Application](PORTFOLIO-PROJECTS.md#project-1--three-tier-web-application) — VPC, ALB, EC2, RDS.
2. [Serverless REST API](PORTFOLIO-PROJECTS.md#project-2--serverless-rest-api) — API Gateway, Lambda, DynamoDB.
3. [CI/CD Pipeline](PORTFOLIO-PROJECTS.md#project-3--cicd-pipeline) — CodePipeline, CodeBuild, ECR, ECS.
4. [Event-Driven File Processing](PORTFOLIO-PROJECTS.md#project-4--event-driven-file-processing) — S3, Lambda, EventBridge, SNS, Step Functions.
5. [AI Document Analysis](PORTFOLIO-PROJECTS.md#project-5--ai-document-analysis) — S3, Lambda, Textract, Comprehend, DynamoDB.
6. [Infrastructure as Code with CDK](PORTFOLIO-PROJECTS.md#project-6--infrastructure-as-code-with-cdk) — VPC, ECS, RDS, ALB.
7. [AI Chatbot with Bedrock](PORTFOLIO-PROJECTS.md#project-7--ai-chatbot-with-bedrock) — API Gateway, Lambda, Bedrock, DynamoDB, S3, CloudFront.

## Recommended learning milestones

- **Phase 1 — Foundation:** Bucket 1 + core of Bucket 3. Milestone: secure account, S3, IAM role and SDK scripting.
- **Phase 2 — Infrastructure:** Buckets 2 + 4. Milestone: deploy and explain the three-tier app.
- **Phase 3 — Automation:** Buckets 5 + 7. Milestone: reproducible CI/CD pipeline with monitoring.
- **Phase 4 — AI:** Bucket 6. Milestone: document processing or a Bedrock-powered RAG chatbot.

## Quick-start links

- [AWS Free Tier and current free offers](https://aws.amazon.com/free/)
- [AWS Management Console](https://console.aws.amazon.com/)
- [AWS Skill Builder](https://skillbuilder.aws/)
- [AWS documentation](https://docs.aws.amazon.com/)
- [AWS re:Post](https://repost.aws/)
- [AWS samples on GitHub](https://github.com/aws-samples)
- [Cost and cleanup checklist](COST-AND-CLEANUP.md)
- [Machine-readable catalogue](catalog.json)

## Safety and quality rules

- Enable root MFA; do not create root access keys. Use root only for tasks that require it.
- Prefer IAM roles and temporary credentials over long-lived access keys.
- Never commit credentials, secrets, private keys or Terraform state.
- Check current Free Tier eligibility, Region availability, quotas and prices before deploying.
- Private subnets do not automatically provide private access to every AWS service; validate routes, endpoints, DNS and IAM.
- Every lab must include validation and teardown. NAT Gateways, load balancers, EC2, RDS, EKS, public IPv4, logging and AI inference can incur charges.
- Treat all examples as learning references; validate service behavior and security in a non-production account.

## Licensing and permitted use

This vault is provided for personal learning, research, and other permitted noncommercial purposes.

- Original documentation, learning notes, explanations, and diagrams: [CC BY-NC 4.0](LICENSE-DOCS.md).
- Code, scripts, automation, templates, configuration, and infrastructure-as-code: [PolyForm Noncommercial 1.0.0](LICENSE-CODE.md).
- **Commercial or business use is not permitted without prior written permission.** This includes use in business/organisational operations, paid training or consulting deliverables, commercial resale or redistribution, commercial hosting/managed services, and incorporation into commercial products or services.
- Third-party provider documentation, trademarks, screenshots, excerpts, logos, icons, fonts, images, dependencies, and SDKs are excluded and remain subject to their original terms.

This is source-available, not OSI-approved open source. See the licence files for the full terms and scope.
