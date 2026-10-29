# AWS Learning Roadmap

## Phase 1 — Foundation (Buckets 1 + core of 3)

**Milestone:** secure the account, understand IAM, create a private S3 bucket and use an SDK/role to access it.

- [ ] Root MFA, budget alerts and Region choice
- [ ] IAM roles and least privilege
- [ ] S3 and safe object access
- [ ] SDK scripting and basic logs

## Phase 2 — Infrastructure (Buckets 2 + 4)

**Milestone:** deploy and explain a three-tier application.

- [ ] EC2/Linux and one managed compute alternative
- [ ] VPC, subnets, routes, Security Groups and NAT cost
- [ ] ALB health checks and DNS
- [ ] RDS private access and backup basics
- [ ] Project 1 evidence and teardown

## Phase 3 — Automation (Buckets 5 + 7)

**Milestone:** repeatable CI/CD with observability and rollback.

- [ ] CloudFormation or CDK
- [ ] Systems Manager Session Manager
- [ ] GitHub-to-ECR-to-ECS pipeline
- [ ] CloudWatch and CloudTrail
- [ ] Budget, tags and teardown

## Phase 4 — AI (Bucket 6)

**Milestone:** complete Project 5 or Project 7.

- [ ] Verify model/service availability and cost first
- [ ] Build a narrow workflow with least privilege
- [ ] Evaluate quality, sensitive-data handling and failure behavior
- [ ] Add monitoring, limits and cleanup

## Weekly practice routine

1. Read the service overview and key security/limits pages.
2. Draw the data/traffic path and list dependencies.
3. Build the smallest useful lab.
4. Test one failure or denied-access case.
5. Capture evidence and explain one alternative.
6. Tear down and review costs.
