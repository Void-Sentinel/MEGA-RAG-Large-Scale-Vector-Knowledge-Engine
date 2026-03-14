# MEGA-RAG-Large-Scale-Vector-Knowledge-Engine
MEGA-RAG is a specialized vector database engine designed to ground AI agents in factual truth. By indexing over 540,000 MCQ entries from diverse academic datasets, it provides a high-precision retrieval layer for validating model outputs in complex reasoning tasks
## Key Features:-
- **Massive Knowledge Base:** Aggregates and preprocesses 540k+ entries from SCIQ, ARC, Exambench, and MMLU.
- **High-Precision Retrieval:** Uses BAAI/bge-m3 embeddings and FAISS for semantic search with a strict similarity threshold of >= 0.85.
- **Confidence-Gated Validation:** Implements a mathematical scoring mechanism (C >= 0.60) to automate decision-making between model 
  internal logic and external retrieved context.
- **Resource Optimized:** Engineered with a "Purge-and-Load" strategy to run high-density vector search on consumer-grade GPUs (T4) without 
  memory overflow.
