# Skincare Expert AI Agent

An AI-powered skincare assistant designed to provide **evidence-based product and ingredient recommendations**, with a focus on **skin of colour**

The system combines:
- Retrieval-Augmented Generation (RAG) over dermatologist-authored documents
- Deterministic ingredient safety analysis (INCI-based)
- Safety-focused agent validation

---

## Key Capabilities

- Dermatologist-guided skincare recommendations
- Ingredient-level irritancy and comedogenicity assessment
- Product lookup and suitability evaluation
- Designed to reduce hallucinations and unsafe advice

---

## Architecture Overview

1. **Ingestion**
   - Private dermatology PDFs and blogs
   - Chunking and preprocessing

2. **Retrieval**
   - Vector-based semantic search
   - Context grounding for LLM responses

3. **Ingredient Analysis**
   - INCI ingredient lookup
   - Rule-based risk scoring

4. **Agent Layer**
   - Planning and reasoning
   - Safety validation before response

5. **Evaluation**
   - Baseline (no-RAG) vs RAG comparisons
   - Safety and hallucination metrics

---

## Project Structure

```plaintext
src/
├── ingestion/ # PDF parsing & chunking
├── retrieval/ # Embeddings & vector search
├── ingredient_analysis/ # INCI lookup & risk scoring
├── agent/ # Agent orchestration & safety
├── evaluation/ # Testing & metrics
├── app/ # User-facing interface
```

---

## Data & Copyright Notice

This repository does **not** include copyrighted documents.

The system is designed to operate on **user-provided, privately owned documents** and returns **summaries and recommendations**, not verbatim excerpts.

---

## Status

🚧 Initial scaffolding complete  
Next steps:
- Implement PDF ingestion
- Build vector retrieval pipeline
- Add ingredient risk scoring logic
