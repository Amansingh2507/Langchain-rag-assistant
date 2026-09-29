# Langchain-rag-assistant
A Retrieval-Augmented Generation (RAG) document assistant built with LangChain, ChromaDB, and Groq. Implements document chunking, embeddings, vector similarity search, and context-aware LLM responses for intelligent document-based question answering.
# LangChain RAG Document Assistant

This project demonstrates the development of a **Retrieval-Augmented Generation (RAG) based document question-answering system** using Python, LangChain, ChromaDB, and Groq. The objective is to build an AI assistant that can understand and retrieve relevant information from user-provided documents and generate accurate, context-aware responses.

The project begins with **document ingestion**, where source documents are loaded and processed. Large documents are divided into smaller, meaningful chunks using LangChain's **RecursiveCharacterTextSplitter**. Chunking makes the information easier to process and allows the retrieval system to identify specific sections that are relevant to a user's query.

The document chunks are then converted into numerical representations called **embeddings**. These embeddings capture the semantic meaning of the text and are stored in **ChromaDB**, a vector database. When a user submits a question, the query is also converted into an embedding. ChromaDB performs a similarity search between the query vector and stored document vectors to retrieve the most relevant chunks.

The retrieved information is then passed to a **Groq-powered Large Language Model (LLM)** through LangChain. The model uses the retrieved context along with the user's question to generate a natural-language response. This approach allows the system to answer questions using information contained within the provided documents rather than relying solely on the model's pre-trained knowledge.

The project also demonstrates the use of **Python-dotenv and environment variables** for securely managing API credentials and configuration.

### Key Concepts Demonstrated

* Retrieval-Augmented Generation (RAG)
* Document loading and preprocessing
* Recursive text splitting and chunking
* Text embeddings
* Vector databases and ChromaDB
* Cosine similarity and semantic search
* LangChain components
* Groq LLM integration
* Environment variable and API key management
* Context-aware question answering

This project provides a practical foundation for building more advanced **AI-powered document assistants, knowledge bases, and enterprise RAG applications**.
