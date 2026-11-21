# Grounding AI With Your Own Data (RAG Project)

A step-by-step RAG pipeline built with **LangChain**, **OpenAI** and **Qdrant**, using dummy data for a fictional company, *BrightCart*.

## Pipeline
PDF load -> RecursiveCharacterTextSplitter -> OpenAI embeddings -> Qdrant (index) -> Retriever -> ChatGPT answer

## Files
- `rag.ipynb`: the full notebook with explanations
- `brightcart_handbook.pdf`: dummy company data
- `requirements.txt`: Python packages
- `.env.example`: template for the keys (copy it to `.env` and fill in your own)
- `.gitignore`: keeps `.env` and other private files out of GitHub

## How to run
1. `pip install -r requirements.txt`
2. Copy `.env.example` to `.env` and add your `OPENAI_API_KEY`, `QDRANT_URL`, `QDRANT_API_KEY`
3. Open `rag.ipynb` and run all cells
