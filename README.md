# Juan Pablo Cuervo

**AI Engineer · Backend** · Popayán, Colombia

I put language models into systems you can verify. Since 2022 I have been building backends that turn documents into data for financial and public-sector organisations in Colombia: extraction with LLMs, validation with business rules, and integration with the systems already in place.

**Portfolio:** [0103juan.github.io/portfolio-site](https://0103juan.github.io/portfolio-site/) (Spanish and English)

## Applied AI

Every number below comes from a real run and is explained, with its limits, in the repository's README.

| Project | What it is | Measured |
| --- | --- | --- |
| [consultor-tributario](https://github.com/0103juan/consultor-tributario) | Spanish RAG over Colombia's tax code, answering with article citations | 29 of 33 questions correct, 100% grounded |
| [enterprise-rag](https://github.com/0103juan/enterprise-rag) | RAG with query rewriting, hybrid retrieval, reranking and claim-level hallucination checks | 87.9% correct, 100% grounded; quality gates in CI |
| [secop-analyst](https://github.com/0103juan/secop-analyst) | A LangGraph agent over public contracts: hybrid search on pgvector, model-written SQL contained by Postgres, human approval, two-tier memory on Redis and Postgres, OpenTelemetry, local Kubernetes | One real question so far: 38 figures checked against the database, all correct, for about $0.06 |
| [model-gateway](https://github.com/0103juan/model-gateway) | The Python package the two RAG projects call models through: routing between a small and a large model, fallback, response cache, cost per call and a budget per key | Same evaluation at $0.66 on the large model and $0.27 on the small one, 28 and 27 of 33 correct; a repeated run cost $0.00 |
| [sandboxed-agent](https://github.com/0103juan/sandboxed-agent) | Multi-agent coding system with human approval gates, inside a locked-down Docker sandbox, no agent framework | One full run written up, with its cost |
| [legacy-db-mcp](https://github.com/0103juan/legacy-db-mcp) | MCP server that lets a model query a legacy database: read-only, column-masked and time-boxed by the database engine | Three real sessions with the model written up |
| [secop-mcp](https://github.com/0103juan/secop-mcp) | MCP server over Colombia's public procurement data | A real session showed two failures; both were fixed in the tool, not in the prompt |

## A product on public data

*Contratos a la vista* shows what each Colombian state entity contracts, with whom and how.

- [secop-api](https://github.com/0103juan/secop-api): Node.js and TypeScript with no runtime dependencies. [Live](https://secop-api-i89q.onrender.com) on a free plan, so the first request can take a while.
- [secop-dashboard](https://github.com/0103juan/secop-dashboard): Angular. [Live](https://0103juan.github.io/secop-dashboard/), tested end to end against the real API on every deployment.
- [secop-mobile](https://github.com/0103juan/secop-mobile): Flutter, for Android and the web.

## Backend

- [terraform-aws-platform](https://github.com/0103juan/terraform-aws-platform): Terraform modules for a service on AWS (VPC, EKS, RDS, ElastiCache, pod identity, GitHub OIDC), tested against a mocked provider. Not applied to an account.
- [crediya-microservice-loan](https://github.com/0103juan/crediya-microservice-loan): a reactive hexagonal microservice in Java 21 and Spring WebFlux. Approving a loan publishes to SQS and a Lambda emails the client, checked in CI on LocalStack.
- [crediya-microservice-auth](https://github.com/0103juan/crediya-microservice-auth): users, roles and JWT login, mutation-tested.

## Contact

[0103juan@gmail.com](mailto:0103juan@gmail.com) · [LinkedIn](https://www.linkedin.com/in/juan-pablo-cuervo-dorado-779089256)
