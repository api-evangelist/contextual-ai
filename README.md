# Contextual AI (contextual-ai)

Contextual AI is an enterprise RAG platform built around a Grounded Language Model (GLM) engineered to minimize hallucinations. Its REST API exposes end-to-end RAG agents (create, configure, query) plus standalone component APIs - Generate, Rerank, Parse, and LMUnit - over datastores of ingested documents, all authenticated with a Bearer API key.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/apis.yml)

## Tags

- AI
- RAG
- LLM
- Grounded Language Model
- Enterprise

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Contextual AI Agents API

Create, configure, edit, copy, reset, and delete enterprise RAG agents, including system prompts, suggested queries, templates, and associated datastores.

- **Human URL:** [https://docs.contextual.ai/api-reference/agents/create-agent](https://docs.contextual.ai/api-reference/agents/create-agent)
- **Base URL:** `https://api.contextual.ai/v1`

#### Tags

- Agents
- RAG
- Configuration

#### Properties

- [Documentation](https://docs.contextual.ai/user-guides/beginner-guide)
- [API Reference](https://docs.contextual.ai/api-reference/agents/create-agent)
- [OpenAPI](openapi/contextual-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/contextual-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contextual-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Contextual AI Agent Query API

Query an agent for grounded responses with inline attributions, retrieval contents, and groundedness scores; supports SSE token streaming via stream=true, retrievals-only mode, conversation continuity, and feedback.

- **Human URL:** [https://docs.contextual.ai/api-reference/agents-query/query](https://docs.contextual.ai/api-reference/agents-query/query)
- **Base URL:** `https://api.contextual.ai/v1`

#### Tags

- Query
- RAG
- Grounded
- Streaming

#### Properties

- [Documentation](https://docs.contextual.ai/api-reference/agents-query/query)
- [API Reference](https://docs.contextual.ai/api-reference/agents-query/query)
- [OpenAPI](openapi/contextual-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/contextual-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/contextual-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contextual-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Contextual AI Datastores & Documents API

Create and manage datastores and ingest documents (PDF, HTML, DOC(X), PPT(X), images) with custom metadata; list, retrieve, update, and delete documents and their parsed chunks.

- **Human URL:** [https://docs.contextual.ai/api-reference/datastores/create-datastore](https://docs.contextual.ai/api-reference/datastores/create-datastore)
- **Base URL:** `https://api.contextual.ai/v1`

#### Tags

- Datastores
- Documents
- Ingestion

#### Properties

- [Documentation](https://docs.contextual.ai/api-reference/datastores/create-datastore)
- [API Reference](https://docs.contextual.ai/api-reference/datastores-documents/ingest-document)
- [OpenAPI](openapi/contextual-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/contextual-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contextual-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Contextual AI Generate API

Standalone grounded generation with the Grounded Language Model (GLM v1/v2) - responses are grounded in supplied knowledge to minimize hallucinations, with a 32,000-token request limit.

- **Human URL:** [https://docs.contextual.ai/api-reference/generate/generate](https://docs.contextual.ai/api-reference/generate/generate)
- **Base URL:** `https://api.contextual.ai/v1`

#### Tags

- Generate
- Grounded Language Model
- Generation

#### Properties

- [Documentation](https://docs.contextual.ai/api-reference/generate/generate)
- [API Reference](https://docs.contextual.ai/api-reference/generate/generate)
- [OpenAPI](openapi/contextual-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/contextual-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contextual-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Contextual AI Rerank API

Instruction-following reranker (ctxl-rerank-v2 multilingual / mini and v1) that reorders retrieved passages by relevance, steerable with natural-language instructions on recency, document type, or source.

- **Human URL:** [https://docs.contextual.ai/api-reference/rerank/rerank](https://docs.contextual.ai/api-reference/rerank/rerank)
- **Base URL:** `https://api.contextual.ai/v1`

#### Tags

- Rerank
- Retrieval
- Instruction Following

#### Properties

- [Documentation](https://docs.contextual.ai/how-to-guides/rerank)
- [API Reference](https://docs.contextual.ai/api-reference/rerank/rerank)
- [OpenAPI](openapi/contextual-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/contextual-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contextual-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Contextual AI Parse API

Asynchronous document parsing that converts PDFs, Office files, and images into AI-ready markdown with inferred hierarchy and positional metadata; submit a job, then poll status and results (basic text or standard multimodal).

- **Human URL:** [https://docs.contextual.ai/api-reference/parse/parse-file](https://docs.contextual.ai/api-reference/parse/parse-file)
- **Base URL:** `https://api.contextual.ai/v1`

#### Tags

- Parse
- Document Parsing
- OCR

#### Properties

- [Documentation](https://docs.contextual.ai/how-to-guides/parse)
- [API Reference](https://docs.contextual.ai/api-reference/parse/parse-file)
- [OpenAPI](openapi/contextual-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/contextual-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contextual-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Contextual AI LMUnit Evaluation API

Evaluate model responses with fine-grained natural-language unit tests, returning a continuous 1-5 score for criteria such as conciseness, technical precision, and groundedness.

- **Human URL:** [https://docs.contextual.ai/api-reference/lmunit/lmunit](https://docs.contextual.ai/api-reference/lmunit/lmunit)
- **Base URL:** `https://api.contextual.ai/v1`

#### Tags

- LMUnit
- Evaluation
- Unit Testing

#### Properties

- [Documentation](https://docs.contextual.ai/how-to-guides/lmunit)
- [API Reference](https://docs.contextual.ai/api-reference/lmunit/lmunit)
- [OpenAPI](openapi/contextual-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/contextual-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contextual-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/ContextualAI)
- [LinkedIn](https://www.linkedin.com/company/contextual-ai)
- [Website](https://contextual.ai/)
- [Documentation](https://docs.contextual.ai)
- [Plans](plans/contextual-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/contextual-ai-rate-limits.yml)
- [Fin Ops](finops/contextual-ai-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
