# Bucket 4 — Networking & Content Delivery

> AWS Master Vault learning tracker. This category uses AWS-native services, identity models, networking and governance terminology.

## Category architecture

![Bucket 4 — Networking & Content Delivery architecture](architecture.svg)

- [Editable category diagram](architecture.drawio)
- [Mermaid source](architecture.mmd)
- [Visual architecture library](../../VISUAL-DIAGRAMS.md)
- [Enterprise reference architecture](../../AWS-ENTERPRISE-REFERENCE-ARCHITECTURE.md)

## Component checklist

| Topic | Learning guide | Diagram (SVG) | Editable diagram |
|---|---|---|---|
| Amazon VPC | [Open guide](../../services/amazon-vpc.md) | [View](../../services/amazon-vpc/architecture.svg) | [draw.io](../../services/amazon-vpc/architecture.drawio) |
| Security Groups vs Network ACLs | [Open guide](../../services/security-groups-vs-network-acls.md) | [View](../../services/security-groups-vs-network-acls/architecture.svg) | [draw.io](../../services/security-groups-vs-network-acls/architecture.drawio) |
| Application Load Balancer | [Open guide](../../services/application-load-balancer.md) | [View](../../services/application-load-balancer/architecture.svg) | [draw.io](../../services/application-load-balancer/architecture.drawio) |
| Network Load Balancer | [Open guide](../../services/network-load-balancer.md) | [View](../../services/network-load-balancer/architecture.svg) | [draw.io](../../services/network-load-balancer/architecture.drawio) |
| Amazon Route 53 | [Open guide](../../services/amazon-route-53.md) | [View](../../services/amazon-route-53/architecture.svg) | [draw.io](../../services/amazon-route-53/architecture.drawio) |
| Amazon CloudFront | [Open guide](../../services/amazon-cloudfront.md) | [View](../../services/amazon-cloudfront/architecture.svg) | [draw.io](../../services/amazon-cloudfront/architecture.drawio) |
| Amazon API Gateway | [Open guide](../../services/amazon-api-gateway.md) | [View](../../services/amazon-api-gateway/architecture.svg) | [draw.io](../../services/amazon-api-gateway/architecture.drawio) |
| AWS NAT Gateway | [Open guide](../../services/aws-nat-gateway.md) | [View](../../services/aws-nat-gateway/architecture.svg) | [draw.io](../../services/aws-nat-gateway/architecture.drawio) |
| AWS Transit Gateway | [Open guide](../../services/aws-transit-gateway.md) | [View](../../services/aws-transit-gateway/architecture.svg) | [draw.io](../../services/aws-transit-gateway/architecture.drawio) |
| AWS PrivateLink and VPC endpoints | [Open guide](../../services/aws-privatelink-and-vpc-endpoints.md) | [View](../../services/aws-privatelink-and-vpc-endpoints/architecture.svg) | [draw.io](../../services/aws-privatelink-and-vpc-endpoints/architecture.drawio) |

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
