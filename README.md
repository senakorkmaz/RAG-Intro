# RAG-Intro

This repository provides a simple and effective implementation of Retrieval-Augmented Generation (RAG) using LangChain and OpenAI APIs. The RAG architecture enriches the context of language models by retrieving relevant documents and incorporating them into the generation process.

## Features

- Loads and splits documents using LangChain text splitters.
- Stores vector representations using FAISS.
- Utilizes OpenAI API for answering questions based on retrieved context.

## Requirements

Install dependencies using the provided `requirements.txt`:

```bash
pip install -r requirements.txt
```

### Key Packages

- `langchain`, `langchain-core`, `langchain-openai`
- `openai`, `faiss-cpu`
- `bs4`, `httpx`, `tqdm`, `python-dotenv`
- `tiktoken`, `langchainhub`, `langchain_chroma`

## Usage

Before running the script, make sure to:

1. Set your OpenAI API key in a `.env` file:
   ```env
   OPENAI_API_KEY=your_openai_api_key
   LANGCHAIN_API_KEY=your_langchain_api_key
   (Optional for tracing)
   LANGCHAIN_TRACING_V2=true
   LANGCHAIN_PROJECT=RAGCHATBOT
   ```

2. Run the main script:
   ```bash
   python main.py
   ```

The script will prompt you for a question and retrieve the most relevant documents from the vector store to provide an answer.

## File Structure

```
.
├── main.py              # Main script implementing RAG workflow
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

## Author

Developed by [Senanur Korkmaz](https://github.com/senakorkmaz)
