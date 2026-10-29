# Bucket 2 — Compute & Containers

> Choose and operate virtual machines, functions and containers according to workload control, scaling and operational effort.

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
| [Amazon EC2](../../services/amazon-ec2.md) | Run virtual machines with selected instance types, storage and network controls. | [Official docs](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) |
| [EC2 Auto Scaling](../../services/ec2-auto-scaling.md) | Maintain desired capacity and scale eligible EC2 fleets. | [Official docs](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html) |
| [AWS Lambda](../../services/aws-lambda.md) | Run event-driven code without managing the server fleet. | [Official docs](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html) |
| [Amazon ECS](../../services/amazon-ecs.md) | Orchestrate containers using AWS-native tasks and services. | [Official docs](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html) |
| [AWS Fargate](../../services/aws-fargate.md) | Run eligible containers without managing EC2 worker hosts. | [Official docs](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html) |
| [Amazon ECR](../../services/amazon-ecr.md) | Store and distribute container images. | [Official docs](https://docs.aws.amazon.com/AmazonECR/latest/userguide/what-is-ecr.html) |
| [Amazon EKS](../../services/amazon-eks.md) | Run Kubernetes workloads on AWS; understand its additional operational complexity. | [Official docs](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html) |
| [Amazon EC2 GPU instances](../../services/amazon-ec2-gpu-instances.md) | Evaluate accelerated compute for ML, graphics and parallel workloads. | [Official docs](https://aws.amazon.com/ec2/instance-types/) |
| [AWS Batch](../../services/aws-batch.md) | Schedule and execute batch computing jobs. | [Official docs](https://docs.aws.amazon.com/batch/latest/userguide/what-is-batch.html) |
| [AWS App Runner](../../services/aws-app-runner.md) | Deploy supported web applications and APIs with managed operations. | [Official docs](https://docs.aws.amazon.com/apprunner/latest/dg/what-is-apprunner.html) |

## Choose the compute model

- EC2: highest OS/runtime control; patching and capacity remain operational responsibilities.
- Lambda: event-driven, bounded execution model; review quotas, concurrency, timeout and cold-start trade-offs.
- ECS/Fargate: managed container scheduling without managing worker hosts.
- EKS: Kubernetes compatibility and ecosystem, with greater platform complexity.
- GPU instances: use only when a workload needs acceleration; check availability and cost before launch.

## Hands-on labs

1. Launch a small EC2 instance in a selected Region and connect using a secure method. Prefer Session Manager when configured; if using SSH, restrict inbound sources and remove the rule after the lab.
2. Attach an IAM role to EC2 and verify the instance can access only the intended S3 object/prefix.
3. Deploy a Lambda function and connect one trigger; inspect logs, retries, timeout and permissions.
4. Build a container image, push it to ECR, and deploy it to ECS/Fargate.
5. Optional advanced path: deploy a small EKS cluster only after reviewing cost, IAM, networking and cleanup requirements.

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
