# RAG-FAISS-quickstart

## Overview
This mini project implements a simple Retrieval-Augmented Generation (RAG) pipeline in Google Colab.
A text is embedded using a sentence-transformer (MiniLM), indexed in FAISS,
and used to answer questions by retrieving the most relevant chunks and passing them as context to an open LLM (Llama-3 via Hugging Face Inference API).

## Tech Stack
- Google Colab
- `sentence-transformers/all-MiniLM-L6-v2` for embeddings
- `faiss-cpu` for vector search
- `huggingface_hub.InferenceClient` for LLM calls (`meta-llama/Meta-Llama-3-8B-Instruct`)
