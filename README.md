# Emma RAG with Ollama 🤖

A lightweight local Retrieval-Augmented Generation (RAG) project built with Google Colab, Ollama, sentence-transformers, and ChromaDB. The project loads a PDF document, converts it into searchable embeddings, and answers questions using a local LLM — without relying on external paid APIs.

## ✨ Overview

This repository demonstrates how to build a document-based Q&A assistant using:

- Ollama for local LLM inference
- sentence-transformers for embeddings
- ChromaDB for vector storage and retrieval
- PDF documents as the knowledge source
- Google Colab as the execution environment

The example uses a PDF about Emma Watson and allows the model to answer questions grounded in the document content.

## 🚀 Key Features

- Local, private AI workflow
- Document-based retrieval using vector search
- No cloud API dependency required
- Easy to run in Google Colab
- Suitable for experimentation and learning RAG pipelines
- Great base for extensions such as chat interfaces, multi-document search, and custom knowledge bases

## 🧠 How It Works

1. A PDF is loaded into the notebook.
2. The text is split into smaller chunks.
3. Each chunk is converted into embeddings using sentence-transformers.
4. The embeddings are stored in ChromaDB.
5. A user question is embedded and matched against the stored vectors.
6. The most relevant passages are retrieved and passed to Ollama's local model.
7. The model generates a contextual answer based on the retrieved content.

## 📁 Repository Structure

```text
Emma_Rag_Ollama/
├── Emma_rag_colab.ipynb      # Main Colab notebook for the RAG workflow
├── rag_colab.ipynb           # Additional notebook version
├── docs/                     # Supporting documentation or notes
├── emma_watson.pdf           # Sample PDF used as the knowledge base
├── .gitignore                # Git ignore rules
├── README.md                 # Project documentation
└── .config/                  # Local configuration files
```

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Google Colab
- Ollama
- Llama 3.2
- sentence-transformers
- ChromaDB
- PDF parsing

## ⚙️ Prerequisites

Before running the notebook, make sure you have:

- A Google Colab environment or local Jupyter setup
- Python 3.10+
- Ollama installed and running locally
- The Llama 3.2 model pulled in Ollama

Example:

```bash
ollama pull llama3.2
```

## ▶️ Getting Started

1. Clone the repository:

```bash
git clone https://github.com/VigneshA7MSD/Emma_Rag_Ollama.git
cd Emma_Rag_Ollama
```

2. Open the notebook in Colab or Jupyter:

- `Emma_rag_colab.ipynb`

3. Run the cells in sequence.

4. When prompted, ensure Ollama is available and the model is loaded.

5. Ask questions related to the embedded PDF content to see the RAG workflow in action.

## 🧪 Example Use Cases

- Querying a PDF document with natural language
- Building a local document assistant
- Learning how RAG pipelines work in practice
- Experimenting with embeddings and retrieval-quality improvements

## 📌 Notes

This project is designed for educational and experimental purposes. It is an excellent starting point for building more advanced document Q&A systems, enterprise knowledge assistants, or custom local AI apps.

## 🙌 Project Status

The repository is currently focused on a functional local RAG demo and serves as a practical reference for building retrieval-based question answering systems using open-source tools.

If you want, I can also help you add:

- a more detailed installation guide
- a requirements.txt file
- screenshots or architecture diagrams
- a polished project badge section
- a version with a proper MIT license
