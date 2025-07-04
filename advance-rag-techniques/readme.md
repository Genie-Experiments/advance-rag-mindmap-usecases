# 📚 RAG Pipeline Optimization with LangChain & LLMs

This project consists of a series of Jupyter notebooks that guide you through optimizing a Retrieval-Augmented Generation (RAG) pipeline. Each notebook focuses on a specific component essential for building efficient, accurate, and scalable RAG systems.

---

## 📘 Notebook Summaries

* **`document indexing.ipynb`**
  Prepares, chunks, and indexes your document corpus into a vector store for fast and accurate retrieval using different chunking and indexing strategies combined with metadata enrichment.

* **`query optimization.ipynb`**
  Refines user queries using rewriting and enhancement techniques to improve semantic similarity.

* **`embeddings optimization.ipynb`**
  Compares and tunes different embedding models to boost similarity matching and vector search relevance.

* **`postretrieval reranking.ipynb`**
  Applies reranking strategies falling under two main domains—cross-encoders or LLMs—to sort retrieved documents by true semantic relevance.

* **`postretriveal context expanders.ipynb`**
  Expands or enriches retrieved results with related context to provide better grounding for LLM responses.

---

## 🔧 Setup

Before running the notebooks, it's recommended to create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Then install the required dependencies using:

```bash
pip install -r requirements.txt
```

## 🚀 How to Use

* Run any notebook independently depending on your focus, or start with `document indexing.ipynb`.
* Each notebook builds on a foundational RAG pipeline—documents are loaded, indexed, queries are run, and results are evaluated.

You can:

* Input your own queries.
* Load PDF/text documents or link to a GitHub repo containing code for indexing and retrieval.
* Swap embedding models or reranking methods to test different configurations.

---

## 🧠 Pipeline Architecture

All experiments are built on top of a base RAG pipeline:

1. **Data Preparation** – Load any documents, codebases, or datasets.
2. **Indexing** – Chunk and store data in a vector database.
3. **Querying** – Enter questions or prompts to retrieve relevant chunks.
4. **Response Generation** – Use an LLM to generate answers grounded in the retrieved context.
5. **Evaluation & Optimization** – Apply reranking, query tuning, and context expansion strategies to improve quality.

This design allows you to test how each enhancement (query rewriting, reranking, embedding tuning, etc.) impacts retrieval performance and LLM output quality.



