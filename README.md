# LLM-RAG-Gemma_7b_it

### Introduction

The repo is a demonstration of implementing RAG paradigm using an open-source LLM (Gemma-7B-Instruct). Gemma is Google's open source lightweight LLM model. The work also explores different approaches and techniques (advanced vs naive) to create an end to end RAG pipeline.


### Components

* LLM - ```Gemma-7b-it```
* Embedding Model - ```BAAI/bge-large-en-v1.5```
* Vector DB - ```Pinecone```
* Orchestrator - ```LangChain```
* Re-ranker - ```Cohere```
* Models Source - ```HuggingFace```
* Run-time environment - ```Google Colab T4 GPU```


### Steps

* Load Documents
* Chunk text 
* Create Embeddings using model - ```BAAI/bge-large-en-v1.5```
* Index and load to Vector Store - ```Pinecone```
* Load Quantized LLM model - ```Gemma-7b-it```
* Build Question Answering Chain using ```LangChain```
* RAG w/ Base Retriever -  Similarity search with pre-defined ```Threshold``` and ```Top-k```
* RAG w/ pre-retrieval (metadata filtering) and Re-ranker - ```Cohere```
