# Bucket 6 — AI & Machine Learning

> Build AI/ML workflows with controlled data access, evaluation, observability and cost management.

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
| [Amazon Bedrock](../../services/amazon-bedrock.md) | Build generative AI applications using supported foundation models. | [Official docs](https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html) |
| [Amazon Bedrock API and SDK](../../services/amazon-bedrock-api-and-sdk.md) | Call supported model APIs with authorized SDK credentials. | [Official docs](https://docs.aws.amazon.com/bedrock/latest/userguide/getting-started-api.html) |
| [Amazon SageMaker AI](../../services/amazon-sagemaker-ai.md) | Build, train, deploy and operate supported machine-learning models. | [Official docs](https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html) |
| [SageMaker AI endpoints](../../services/sagemaker-ai-endpoints.md) | Serve supported models through managed endpoints. | [Official docs](https://docs.aws.amazon.com/sagemaker/latest/dg/realtime-endpoints.html) |
| [Amazon Textract](../../services/amazon-textract.md) | Extract supported text and structured information from documents. | [Official docs](https://docs.aws.amazon.com/textract/latest/dg/what-is.html) |
| [Amazon Rekognition](../../services/amazon-rekognition.md) | Analyze supported image and video content. | [Official docs](https://docs.aws.amazon.com/rekognition/latest/dg/what-is.html) |
| [Amazon Comprehend](../../services/amazon-comprehend.md) | Analyze supported text for sentiment, entities and language signals. | [Official docs](https://docs.aws.amazon.com/comprehend/latest/dg/what-is.html) |
| [Amazon Q Developer](../../services/amazon-q-developer.md) | Assist supported software development and AWS workflows. | [Official docs](https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/what-is.html) |
| [Retrieval-augmented generation (RAG)](../../services/retrieval-augmented-generation-rag.md) | Ground model responses in authorized enterprise knowledge. | [Official docs](https://docs.aws.amazon.com/bedrock/latest/userguide/knowledge-base.html) |
| [AI document-processing workflow](../../services/ai-document-processing-workflow.md) | Explore a sample architecture for document ingestion and analysis; validate the repository before reuse. | [Official docs](https://github.com/aws-samples/aws-ai-intelligent-document-processing) |

## AI architecture controls

- Verify model availability, quotas, data handling and pricing in the selected Region.
- Keep prompts and retrieved documents within authorized access boundaries.
- Do not log sensitive payloads unnecessarily; evaluate retention and redaction.
- Evaluate output quality and failure behavior; human review may be required for consequential decisions.
- Add budgets and teardown checks for inference endpoints and other metered resources.

## Hands-on labs

1. Call a supported Amazon Bedrock model through an SDK with explicit IAM permissions; verify model access, Region and pricing first.
2. Deploy a small SageMaker AI endpoint only if needed; endpoints may accrue ongoing cost, so delete them immediately after validation.
3. Build an S3 upload → Lambda → Textract → persistence workflow for a non-sensitive sample document.
4. Use Comprehend to analyze sentiment or entities in sample text; record input limits, output handling and cost assumptions.
5. Optional: build a RAG proof of concept and evaluate retrieval quality, access boundaries, citations, hallucinations and prompt injection handling.

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
