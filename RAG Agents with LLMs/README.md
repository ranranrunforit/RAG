# RAG Agents with LLMs

This folder contains a collection of notebooks and related files that walk through building and evaluating Retrieval-Augmented Generation (RAG) systems using large language models (LLMs). The materials cover topics ranging from the course environment and microservices through to document processing, vectorstore integration, evaluation, serving, and even semantic guardrails. Below is a brief description of each file in the folder:

- [**01_microservices.ipynb**](./01_microservices.ipynb)  
  Introduces the course environment and covers the various microservices that underpin the RAG system. It outlines background services (such as data loading, proxy, and assessment management) and provides context on how these services integrate into the overall pipeline.

- [**02_llms.ipynb**](./02_llms.ipynb)  
  Focuses on foundation models and LLM endpoints. This notebook demonstrates how to interact with models (for example, via ChatNVIDIA) and discusses strategies for LLM orchestration. It also lists available models and gives examples of making requests to the LLM service.

- [**03_langchain_intro.ipynb**](./03_langchain_intro.ipynb)  
  Provides an introduction to LangChain as a framework for building LLM workflows. It explains chain-based abstractions, including constructing and manipulating chains, and bridges the gap between raw LLM requests and higher-level orchestration frameworks.

- [**04_running_state.ipynb**](./04_running_state.ipynb)  
  Demonstrates how to maintain and update the conversation “running state” using a chain approach. This notebook shows methods for slot-filling using RExtract and includes examples of handling schema conformant outputs.

- [**05_documents.ipynb**](./05_documents.ipynb)  
  Explores working with large documents including document splitting, processing, and integration with LLMs. It details how to generate summaries, handle sliding windows for token context, and process document chains for consistent dialog management.

- [**07_vectorstores.ipynb**](./07_vectorstores.ipynb)  
  Focuses on integrating scalable vector databases for fast retrieval of document chunks. It covers embedding generation, document chunking, and vectorstore querying to build an efficient retrieval component for the RAG system.

- [**08_evaluation.ipynb**](./08_evaluation.ipynb)  
  Contains evaluation components and assessment exercises for your RAG system. This notebook guides you through examining outputs, benchmark evaluations, and considerations for productionalizing your retrieval-augmented workflow.

- [**09_langserve.ipynb**](./09_langserve.ipynb)  
  Shows how to deploy the RAG chain via a simple API using LangServe. It details setting up endpoints to expose chain functionality and demonstrates a basic frontend integration for running the chatbot in a production-like setting.

- [**64_guardrails.ipynb**](./64_guardrails.ipynb)  
  Focuses on semantic guardrailing for filtering out harmful or irrelevant chatbot responses. It covers techniques for generating synthetic input data, embedding queries asynchronously, training classifiers (using deep learning or logistic regression), and integrating these components into a chatbot event loop to alter system prompts based on evaluated message quality.

Each notebook builds on previous concepts, guiding you from setting up the basic infrastructure to implementing advanced semantic safety features. 
