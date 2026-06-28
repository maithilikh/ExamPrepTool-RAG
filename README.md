# Academic Document Assistant (RAG System)

An AI-powered academic assistant that allows users to upload PDFs and ask questions using a Retrieval-Augmented Generation (RAG) pipeline.

<img width="3200" height="1834" alt="Screenshot 2026-06-28 194324" src="https://github.com/user-attachments/assets/61c116fd-7a39-43ce-b934-3712a6f59d8e" />

## Features

- Multi-PDF support
- OCR support for scanned documents
- Semantic search using BGE embeddings
- Cross-encoder reranking for improved relevance
- Streaming responses via Groq Llama 3
- Multi-mode interaction:
  - Q&A
  - Summarization
  - Quiz generation
- Persistent vector storage using ChromaDB
- Gradio-based interactive UI

## Tech Stack

- Python
- PyMuPDF
- Tesseract OCR
- Sentence Transformers (BGE-base)
- ChromaDB
- Groq API (Llama 3)
- Gradio

## How it works

1. Upload PDFs
2. System extracts and chunks text
3. Embeddings are stored in ChromaDB
4. Query is embedded and retrieved
5. Results are reranked
6. Final context is sent to LLM
7. Response is streamed back to UI

## Setup

1. Install dependencies (run notebook cells)
2. Add Groq API key
3. Run all cells in order
4. Upload PDFs and start asking questions

## Limitations

- OCR can be slow for scanned documents
- Retrieval depends on chunk quality
- Requires internet for Groq API

## Future Improvements

- Table-aware parsing
- Better citation system
- Hybrid search (BM25 + embeddings)
- Evaluation metrics for RAG quality
