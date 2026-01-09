# RAG with n8n

- [RAG with n8n](#rag-with-n8n)
  - [Overview](#overview)
  - [Before you start](#before-you-start)
  - [Installation](#installation)
    - [n8n](#n8n)
    - [Qdrant](#qdrant)
    - [Ollama](#ollama)
  - [RAG Workflow](#rag-workflow)
    - [Data ingestion](#data-ingestion)
    - [Chatbot](#chatbot)
  - [See also](#see-also)


## Overview

This guide explains how to implement a RAG (Retrieval Augmented Generation) on your laptop.

![nvidia RAG](./assets/RAG.png)

## Before you start

Before you put the RAG in place, ensure you already have:

* Docker
* Ollama
* pdf files

## Installation


### n8n
> n8n is a workflow automation platform that gives technical teams the flexibility of code with the speed of no-code.

**Run locally**

```sh
docker volume create n8n_data
docker run -it --rm --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```

### Qdrant
> Qdrant (read: quadrant) is a vector similarity search engine and vector database. It provides a production-ready service with a convenient API to store, search, and manage points—vectors with an additional payload Qdrant is tailored to extended filtering support. 

**Run localy**

```sh
docker volume create qdrant_data
docker run -p 6333:6333 -v qdrant_data:/qdrant/storage qdrant/qdrant
```

[qdrant Dashboard](http://localhost:6333/dashboard)



### Ollama



## RAG Workflow

![RAG perso](./assets/n8n-RAG-Qdrant.png)

### Data ingestion


### Chatbot



## See also

* [n8n link](https://github.com/n8n-io/n8n)
* [qdrant link](https://github.com/qdrant/qdrant)
* [Ollama](https://github.com/ollama/ollama)
