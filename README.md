# rag-company-hr-policy-chatbot — Built with n8n
RAG-powered AI chatbot that answers HR policy questions from uploaded PDF documents — built with n8n, Groq, and HuggingFace embeddings

## What it does
- AI chatbot that answers HR policy questions from uploaded PDF documents
- Uses RAG (Retrieval-Augmented Generation) to ensure answers come only from the document, not AI hallucinations

## Tech Stack
- **n8n** — workflow orchestration (no-code)
- **Groq (Qwen 3.8-27B)** — LLM for generating responses
- **HuggingFace** — text embeddings for semantic search
- **In-Memory Vector Store** — stores document chunks for retrieval

## How it works
1. Upload an HR policy PDF via form trigger
2. PDF is chunked, embedded, and stored in vector store
3. Ask questions via chat — AI retrieves relevant sections and answers

## How to run
1. Import the `.json` file into your n8n instance
2. Add your Groq and HuggingFace API keys
3. Upload a PDF and start chatting
