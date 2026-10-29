# Bucket 4 — Networking & Content Delivery

> Design VPC segmentation, routing, secure ingress, DNS, hybrid connectivity and content delivery.

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
| [Amazon VPC](../../services/amazon-vpc.md) | Create isolated networks with address ranges, subnets, routes and gateways. | [Official docs](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) |
| [Security Groups vs Network ACLs](../../services/security-groups-vs-network-acls.md) | Distinguish stateful interface controls from stateless subnet-level rules. | [Official docs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Security.html) |
| [Application Load Balancer](../../services/application-load-balancer.md) | Route HTTP/HTTPS requests at Layer 7. | [Official docs](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html) |
| [Network Load Balancer](../../services/network-load-balancer.md) | Load-balance supported Layer 4 traffic. | [Official docs](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/introduction.html) |
| [Amazon Route 53](../../services/amazon-route-53.md) | Host DNS zones and route queries using supported routing policies. | [Official docs](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html) |
| [Amazon CloudFront](../../services/amazon-cloudfront.md) | Cache and deliver content and supported application traffic at edge locations. | [Official docs](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| [Amazon API Gateway](../../services/amazon-api-gateway.md) | Publish and govern APIs, often integrated with Lambda. | [Official docs](https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html) |
| [AWS NAT Gateway](../../services/aws-nat-gateway.md) | Provide outbound IPv4 connectivity from eligible private subnets. | [Official docs](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html) |
| [AWS Transit Gateway](../../services/aws-transit-gateway.md) | Connect multiple VPCs and supported hybrid networks. | [Official docs](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html) |
| [AWS PrivateLink and VPC endpoints](../../services/aws-privatelink-and-vpc-endpoints.md) | Access supported services privately and reduce reliance on public paths. | [Official docs](https://docs.aws.amazon.com/vpc/latest/privatelink/what-is-privatelink.html) |

## Network review checklist

- Non-overlapping CIDRs; subnet roles and AZ placement documented.
- Security Groups are stateful; Network ACLs are stateless. Neither replaces IAM.
- NAT Gateways and public IPv4 addresses can incur charges; plan egress and teardown.
- PrivateLink/VPC endpoints require supported service configuration, correct policies, DNS and routes.
- Load balancers need healthy targets, listener rules, TLS strategy and appropriate network permissions.

## Hands-on labs

1. Build a VPC with public and private subnets across at least two AZs for the intended learning design.
2. Add route tables and gateways deliberately; do not place workloads in public subnets without a reason.
3. Add an ALB and target group; test health checks and verify only intended ports are open.
4. Route a test DNS name using Route 53 if you own a domain; DNS hosting and domain registration may have separate costs.
5. Put CloudFront in front of a supported S3 origin or ALB; configure origin access and HTTPS correctly.
6. Create API Gateway endpoints integrated with Lambda and validate authorization, throttling and logs.

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
