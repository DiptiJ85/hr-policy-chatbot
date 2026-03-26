# 🏢 Nestle HR Policy Assistant

RAG-powered chatbot to answer questions about Nestle's HR Policy using Google Gemini, LangChain, ChromaDB and Gradio.

## Tech Stack
- LLM: Google Gemini 1.5 Flash
- Embeddings: Google Generative AI (models/embedding-001)
- Vector Store: ChromaDB
- Framework: LangChain LCEL
- UI: Gradio ChatInterface

## How to Run
1. Add your Google API key to `.env`
2. Run `indexing.ipynb` — builds ChromaDB vector store (once)
3. Run `app.ipynb` — launches Gradio chat UI
4. Open `http://127.0.0.1:7860` and start chatting!

## Architecture
```
PDF → Chunk → Embed → ChromaDB → RAG Chain → Gradio Chat UI
```

## Environment Variables
```bash
GOOGLE_API_KEY=your-key-here
```