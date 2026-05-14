# LangChain RAG From Scratch

A hands-on repository of Jupyter notebooks demonstrating how to build Retrieval-Augmented Generation (RAG) applications from scratch using LangChain, Ollama, and related tooling.

## Project Contents

- `rag_from_scratch_1_to_4.ipynb`
  - Introduction to RAG concepts, environment setup, and a first end-to-end retrieval + generation pipeline.
  - Demonstrates web document loading, text splitting, embedding with HuggingFace, Chroma vector stores, and a simple RAG chain.

- `rag_from_scratch_5_to_9.ipynb`
  - Query transformation including multi-query, RAG-fusion, decomposition, step-back and HyDE techniques.

- `rag_from_scratch_10_and_11.ipynb`
  - Routing patterns for RAG, including semantic routing and structured output.
  - Query construction into a form of metadata filter.

- `rag_from_scratch_12_to_14.ipynb`
  - Indexing strategies including multi-representation indexing, RAPTOR (Recursive Abstractive Processing for Tree-Organized Retrieval) and ColBERT.

- `rag_from_scratch_15_to_19.ipynb`
  - Retrieval improvements by re-ranking (RAG fusion) and corrective RAG (CRAG).
  - Generation improvement by self-reflective RAG and adaptive RAG using LangGraph.

## Environment and Requirements

This repository is designed for interactive use in Jupyter notebooks.

Key dependencies used across the notebooks include:

- `langchain-community`
- `langchain-classic`
- `langchain-core`
- `langchain-text-splitters`
- `langchain-ollama`
- `langchain-huggingface`
- `langchain-chroma`
- `sentence-transformers`
- `pydantic`
- `python-dotenv`
- `beautifulsoup4`
- `bs4`
- `youtube-transcript-api`
- `pytube`

The notebooks also reference:

- `LangSmith` tracing and API integration
- local Ollama models such as `qwen3.5:2b`, `deepseek-r1:1.5b`, and `nomic-embed-text`

## Setup

1. Create or activate a Python virtual environment.
2. Install the packages used in the notebooks. Each notebook contains the install commands for its required packages.
3. Create a `.env` file with any required API keys, for example:

```env
LANGSMITH_API_KEY=your_langsmith_api_key_here
```

4. Start Jupyter and open the notebooks:

```bash
jupyter notebook
```

## Notes

- The notebooks are organized as a stepped tutorial from introductory RAG concepts to advanced retrieval and reranking techniques.
- Some workflows assume local Ollama and model downloads are available.

## License

This project is licensed under the Apache License 2.0. See `LICENSE` for details.
