# RAG (Retrieval-augmented generation) ChatBot

[![CI](https://github.com/umbertogriffo/rag-chatbot/workflows/CI/badge.svg)](https://github.com/umbertogriffo/rag-chatbot/actions/workflows/ci.yaml)
[![Code style: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

> **Disclaimer:** This project utilizes advanced AI models and may produce false information or hallucinations. Use with caution.

## Introduction

The RAG ChatBot is an intelligent conversational agent powered by the Retrieval-augmented generation (RAG) system. It provides contextually relevant responses to user queries by retrieving information from a collection of Markdown files.

## Features

- Utilizes RAG system for context-aware responses.
- Integrates advanced AI models for natural language understanding.
- Supports conversation history for improved response accuracy.
- Implements Hierarchical Summarization and Context Synthesis for handling context overflows.

## Prerequisites

- Python 3.10+
- GPU supporting CUDA 12 and up.
- [Poetry](https://python-poetry.org/docs/)

## Installation

1. Clone the repository: `git clone https://github.com/your_username/rag-chatbot.git`
2. Navigate to the project directory: `cd rag-chatbot`
3. Install dependencies with Poetry: `poetry install`

## Usage

### Build the Memory Index

Run the following command to build the memory index:

```
python chat/memory_builder.py --chunk-size 1000
Run the Chatbot
To interact with the RAG Chatbot, run the following command:

streamlit run chatbot/chatbot_app.py -- --model openchat
Run the RAG Chatbot
For the RAG Chatbot, use the following command:

streamlit run chatbot/rag_chatbot_app.py -- --model openchat --k 2 --synthesis-strategy async_tree_summarization

```

Contributing
Contributions are welcome! Please read the CONTRIBUTING.md file for guidelines.

License
This project is licensed under the MIT License.

Acknowledgements
CTransformers
Lama.cpp
LangChain
Chroma
Streamlit
References
RAG: Retrieval-augmented generation
OpenAI GPT
Streamlit Documentation