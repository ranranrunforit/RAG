# Introduction to NVIDIA NIM™ Microservices

This folder contains hands-on notebooks demonstrating how to build Retrieval-Augmented Generation (RAG) applications using NVIDIA NIM microservices and LangChain. The examples focus on leveraging NVIDIA AI Endpoints for document retrieval, embedding generation, and conversational AI, with practical workflows for both cloud-hosted and locally deployed NIM models.

## Contents

### 1. `RAG_for_HTML_docs_with_Langchain_NVIDIA_AI_Endpoints.ipynb`
This notebook walks through building a RAG pipeline for the NVIDIA Triton documentation website using [LangChain NVIDIA AI Endpoints](https://python.langchain.com/docs/integrations/text_embedding/nvidia_ai_endpoints). 
It covers:
- Downloading and chunking HTML documentation.
- Generating embeddings with NVIDIA's NV-Embed-QA model.
- Storing embeddings in a FAISS vector store.
- Building and querying conversational retrieval chains with Mixtral and Llama3 models.
- Example queries and streaming chat responses.

### 2. `RAG_Langchain_with_Local_NIM.ipynb`
This notebook demonstrates how to build a RAG pipeline using a locally hosted NIM microservice (e.g., Llama3-8b-instruct). 
It covers:
- Setting up and running the NIM container locally.
- Generating embeddings using NVIDIA's cloud endpoint.
- Storing and retrieving document embeddings with FAISS.
- Connecting LangChain to the local NIM endpoint for chat and retrieval.
- Example conversational QA flows.

## Getting Started

1. **API Key**: You will need an NVIDIA API key from the [API Catalog](https://build.nvidia.com/). Follow instructions in each notebook for setup.
2. **Dependencies**: Install required Python packages as specified in the notebooks (`langchain`, `langchain-nvidia-ai-endpoints`, `faiss-gpu` or `faiss-cpu`, etc.).
3. **Docker**: For local NIM hosting, ensure Docker is installed and configured for NVIDIA GPU support.

## References

- [LangChain NVIDIA AI Endpoints Documentation](https://python.langchain.com/docs/integrations/text_embedding/nvidia_ai_endpoints)
- [NVIDIA NIM API Catalog](https://build.nvidia.com/)
- [NVIDIA Triton Inference Server Documentation](https://docs.nvidia.com/deeplearning/triton-inference-server/user-guide/docs/index.html)

---
