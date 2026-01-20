# AI-Assisted SOP Search System (RAG)

## Status
🚧 **In Progress** — actively building toward a production-ready, compliance-aware RAG system for regulated SOP search.

## Overview
This project implements an AI-assisted SOP search system using a Retrieval-Augmented Generation (RAG) architecture. The goal is to enable semantic search and grounded question answering across SOP documentation while supporting regulated environment needs (GxP), including traceability, explainability, and validation readiness.

## Planned Architecture
1. **Ingestion**: parse documents, extract metadata, chunk text
2. **Embedding & Indexing**: generate embeddings and store in a vector database
3. **Retrieval**: top-k similarity search + metadata filtering
4. **Generation**: grounded responses constrained to retrieved context
5. **Deployment**: containerized service with audit-friendly logging

## Tech Stack (Target)
- Python
- Docker
- GCP Cloud Run (deployment target)
- Vector DB (Milvus or equivalent)
- Transformer embeddings + RAG pipeline

## Milestones
- [ ] Define document schema + metadata strategy
- [ ] Build ingestion + chunking pipeline
- [ ] Implement embedding + vector indexing
- [ ] Add retrieval evaluation (precision@k / recall@k)
- [ ] Add grounded generation with citations to source chunks
- [ ] Containerize and deploy to Cloud Run
- [ ] Add monitoring hooks + audit logging

## Validation & Governance (Design Goals)
- Traceability from answer → retrieved chunks → source document
- Explainability through surfaced retrieval results
- Controlled model/version changes aligned with change management
- Audit-friendly logs and reproducible retrieval behavior

## Next Steps
Initial scaffolding and architecture documentation are underway. Code and deployment artifacts will be added as core milestones are completed.
