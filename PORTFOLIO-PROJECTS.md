# AWS Portfolio Projects

Build projects in increasing order of architectural complexity. Use the linked sample as a starting point, not as a guarantee that its current code, dependencies or costs are production-ready. Review repository activity, license, prerequisites and deployment instructions before running it.

## Project 1 — Three-Tier Web Application

**Services:** VPC, ALB, EC2, RDS  
**Goal:** Build a classic web, application and relational data architecture.  
**Coding/configuration:** Minimal app code; focus on networking and infrastructure.  
**Reference:** [Open sample or official guide](https://github.com/aws-samples/aws-three-tier-web-architecture-workshop)

### Implementation milestones

- [ ] Design VPC CIDRs and public/private subnet placement across Availability Zones.
- [ ] Deploy ALB and healthy targets; keep application instances out of direct public ingress where possible.
- [ ] Place RDS in private database subnets and allow only the app tier's security group.
- [ ] Add CloudWatch metrics/logs and document backup, recovery and cost assumptions.
- [ ] Test failure behavior and delete all billable resources.

### Evidence to capture

- [ ] Architecture diagram and explanation of key decisions
- [ ] Deployment and validation steps, with secrets removed
- [ ] Security and IAM rationale
- [ ] Monitoring and failure-handling evidence
- [ ] Cost notes and successful cleanup


## Project 2 — Serverless REST API

**Services:** API Gateway, Lambda, DynamoDB  
**Goal:** Build a serverless backend with CRUD operations and controlled access.  
**Coding/configuration:** Python or Node.js.  
**Reference:** [Open sample or official guide](https://github.com/aws-samples/serverless-samples)

### Implementation milestones

- [ ] Define API routes and authorization requirements.
- [ ] Implement Lambda handlers with input validation, structured logging and least privilege.
- [ ] Model DynamoDB keys from access patterns; define capacity mode and indexes deliberately.
- [ ] Test errors, throttling, retries and idempotency.
- [ ] Measure latency and cost, then remove resources.

### Evidence to capture

- [ ] Architecture diagram and explanation of key decisions
- [ ] Deployment and validation steps, with secrets removed
- [ ] Security and IAM rationale
- [ ] Monitoring and failure-handling evidence
- [ ] Cost notes and successful cleanup


## Project 3 — CI/CD Pipeline

**Services:** CodePipeline, CodeBuild, ECR, ECS  
**Goal:** Automate build, image publication and application deployment.  
**Coding/configuration:** Dockerfile, buildspec and pipeline configuration.  
**Reference:** [Open sample or official guide](https://github.com/krishnaik06/AWS-CI-CD-Projects)

### Implementation milestones

- [ ] Use a source repository and a controlled pipeline role.
- [ ] Build and test a container image; scan where supported and publish to ECR.
- [ ] Deploy to ECS with health checks and a rollback plan.
- [ ] Use short-lived credentials/OIDC where supported; do not store AWS access keys in source.
- [ ] Capture pipeline evidence and delete running compute/load balancers.

### Evidence to capture

- [ ] Architecture diagram and explanation of key decisions
- [ ] Deployment and validation steps, with secrets removed
- [ ] Security and IAM rationale
- [ ] Monitoring and failure-handling evidence
- [ ] Cost notes and successful cleanup


## Project 4 — Event-Driven File Processing

**Services:** S3, Lambda, EventBridge, SNS, Step Functions  
**Goal:** Process uploaded files asynchronously with clear retry and failure behavior.  
**Coding/configuration:** Lambda code and state machine definition.  
**Reference:** [Open sample or official guide](https://docs.aws.amazon.com/lambda/latest/dg/concepts-event-driven-architectures.html)

### Implementation milestones

- [ ] Upload a sample object to S3 and define the event contract.
- [ ] Trigger a worker through a supported event pattern; avoid recursive triggers.
- [ ] Make processing idempotent and handle duplicate/out-of-order events.
- [ ] Use Step Functions for multi-step orchestration and SNS for notifications where justified.
- [ ] Test retries, failed events, observability and cleanup.

### Evidence to capture

- [ ] Architecture diagram and explanation of key decisions
- [ ] Deployment and validation steps, with secrets removed
- [ ] Security and IAM rationale
- [ ] Monitoring and failure-handling evidence
- [ ] Cost notes and successful cleanup


## Project 5 — AI Document Analysis

**Services:** S3, Lambda, Textract, Comprehend, DynamoDB  
**Goal:** Extract document content and enrich it with supported text analysis.  
**Coding/configuration:** Python workflow and optional basic UI.  
**Reference:** [Open sample or official guide](https://github.com/aws-samples/aws-ai-intelligent-document-processing)

### Implementation milestones

- [ ] Store non-sensitive sample documents in a private S3 bucket.
- [ ] Trigger processing with an authorized role and bounded concurrency.
- [ ] Use Textract for supported extraction and Comprehend for eligible text analysis.
- [ ] Persist only required results; define retention and sensitive-data handling.
- [ ] Measure model/service costs and validate output quality with human review as appropriate.

### Evidence to capture

- [ ] Architecture diagram and explanation of key decisions
- [ ] Deployment and validation steps, with secrets removed
- [ ] Security and IAM rationale
- [ ] Monitoring and failure-handling evidence
- [ ] Cost notes and successful cleanup


## Project 6 — Infrastructure as Code with CDK

**Services:** VPC, ECS, RDS, ALB  
**Goal:** Define a repeatable application environment entirely as code.  
**Coding/configuration:** Python or TypeScript.  
**Reference:** [Open sample or official guide](https://github.com/aws/aws-cdk)

### Implementation milestones

- [ ] Define constructs, environment configuration and naming conventions.
- [ ] Synthesize and review generated CloudFormation templates.
- [ ] Deploy to a sandbox and inspect resources and permissions.
- [ ] Add outputs, tags, tests and environment-specific configuration.
- [ ] Destroy the stack and verify dependent resources were removed.

### Evidence to capture

- [ ] Architecture diagram and explanation of key decisions
- [ ] Deployment and validation steps, with secrets removed
- [ ] Security and IAM rationale
- [ ] Monitoring and failure-handling evidence
- [ ] Cost notes and successful cleanup


## Project 7 — AI Chatbot with Bedrock

**Services:** API Gateway, Lambda, Bedrock, DynamoDB, S3, CloudFront  
**Goal:** Build an end-to-end generative AI app; extend to RAG only when required.  
**Coding/configuration:** Backend plus frontend.  
**Reference:** [Open sample or official guide](https://github.com/aws-samples/bedrock-chat)

### Implementation milestones

- [ ] Verify model access, Region support, quotas and pricing before deployment.
- [ ] Build an API and Lambda backend with narrowly scoped model permissions.
- [ ] Add persistence and authorized document retrieval only when needed.
- [ ] Evaluate answer quality, prompt injection, sensitive-data handling and failure behavior.
- [ ] Add observability, usage limits and teardown of all metered resources.

### Evidence to capture

- [ ] Architecture diagram and explanation of key decisions
- [ ] Deployment and validation steps, with secrets removed
- [ ] Security and IAM rationale
- [ ] Monitoring and failure-handling evidence
- [ ] Cost notes and successful cleanup

