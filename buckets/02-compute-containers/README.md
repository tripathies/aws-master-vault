# Compute & Containers

> Category learning tracker for AWS Master Vault. Service names and examples in this folder are AWS-specific.

## Category architecture

![Compute & Containers architecture](architecture.svg)

- [Editable category diagram](architecture.drawio)
- [Mermaid source](architecture.mmd)
- [Full visual library](../../VISUAL-DIAGRAMS.md)
- [Master architecture](../../AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md)

## Component tracker

| Topic guide | SVG diagram | Editable draw.io |
|---|---|---|
| [Amazon EC2](../../services/amazon-ec2.md) | [SVG](../../services/amazon-ec2/architecture.svg) | [draw.io](../../services/amazon-ec2/architecture.drawio) |
| [EC2 Auto Scaling](../../services/ec2-auto-scaling.md) | [SVG](../../services/ec2-auto-scaling/architecture.svg) | [draw.io](../../services/ec2-auto-scaling/architecture.drawio) |
| [AWS Lambda](../../services/aws-lambda.md) | [SVG](../../services/aws-lambda/architecture.svg) | [draw.io](../../services/aws-lambda/architecture.drawio) |
| [Amazon ECS](../../services/amazon-ecs.md) | [SVG](../../services/amazon-ecs/architecture.svg) | [draw.io](../../services/amazon-ecs/architecture.drawio) |
| [AWS Fargate](../../services/aws-fargate.md) | [SVG](../../services/aws-fargate/architecture.svg) | [draw.io](../../services/aws-fargate/architecture.drawio) |
| [Amazon ECR](../../services/amazon-ecr.md) | [SVG](../../services/amazon-ecr/architecture.svg) | [draw.io](../../services/amazon-ecr/architecture.drawio) |
| [Amazon EKS](../../services/amazon-eks.md) | [SVG](../../services/amazon-eks/architecture.svg) | [draw.io](../../services/amazon-eks/architecture.drawio) |
| [Amazon EC2 GPU instances](../../services/amazon-ec2-gpu-instances.md) | [SVG](../../services/amazon-ec2-gpu-instances/architecture.svg) | [draw.io](../../services/amazon-ec2-gpu-instances/architecture.drawio) |
| [AWS Batch](../../services/aws-batch.md) | [SVG](../../services/aws-batch/architecture.svg) | [draw.io](../../services/aws-batch/architecture.drawio) |
| [AWS App Runner](../../services/aws-app-runner.md) | [SVG](../../services/aws-app-runner/architecture.svg) | [draw.io](../../services/aws-app-runner/architecture.drawio) |

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
