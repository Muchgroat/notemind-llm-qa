# NoteMind: Large Language Model Interface for Course Notes

NoteMind is an academic question-answering system that allows students to upload
course notes and ask natural language questions. The system uses semantic retrieval
with vector embeddings and a Large Language Model to generate accurate answers.

## Features
- Upload academic notes (PDF/Text)
- Semantic search using vector embeddings
- Context-aware question answering
- Retrieval-Augmented Generation (RAG)

## Tech Stack
- Python
- Flask
- FAISS (Vector Database)
- OpenAI / HuggingFace LLM
- Streamlit / HTML frontend

## Architecture
1. Notes are chunked into smaller sections
2. Each chunk is converted into embeddings
3. Embeddings are stored in a FAISS vector index
4. User questions retrieve relevant chunks
5. LLM generates answers using retrieved context

## How to Run
```bash
pip install -r backend/requirements.txt
python backend/app.py
