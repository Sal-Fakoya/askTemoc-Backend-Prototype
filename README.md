# Backend Prototype

## File Structure
```
backend-prototype/
├── ingestion_service/
│   └── app.py
├── embed_service/
│   ├── app.py
│   ├── requirements.txt
│   ├── db/
│   │   └── chroma/
│   ├── models/
│   │   └── __init__.py
│   └── utils/
│       └── __init__.py
├── retrieval_service/
│   └── app.py
├── generation_service/
│   └── app.py
├── docker-compose.yml
├── requirements.txt
└── README.md
```


## 👥 From AskTemoc: Team Structure & Responsibilities

### Person A — Ingestion & Parsing (Ingest Team)
- **Web scrapers / document loaders**
- **OCR pipeline** 
- **Chunking strategies**
- **Document metadata management**
- **Raw-document store (SQLite)**

### Person B — Embeddings & Vector Store (Index Team)
- **Embedding pipeline**
- **Local vector DB** (Chroma/FAISS for MVP)
- **Vector index schema design**
- **Vector search API**

### Person C — Retrieval & LLM Orchestration (RAG/LLM Team)
- **Retrieval logic** (hybrid search for future)
- **Reranker integration**
- **Langchain chains** calling Ollama/remote models
- **Generation & prompt engineering**
- **Chat history management**

### Person D — Infra, Evaluation, QA & Dashboard (Ops/Eval Team)
- **CI/CD pipelines**
- **Docker & development environments**
- **OpenAPI/contract testing**
- **RAG evaluation** (DeepEval/RAGAS)
- **Admin dashboard endpoints/CRUD**
- **Deployment documentation**
  

