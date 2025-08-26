Research Publication RAG System

This notebook demonstrates the implementation of a Retrieval-Augmented Generation (RAG) system for querying research publications. It utilizes Langchain components, Hugging Face embeddings, and ChromaDB as a vector store to build a knowledge base and answer questions based on the provided documents.
Table of Contents

    Overview
    Setup
        Prerequisites
        Installation
        API Keys
        Data Preparation
    How to Run
    Code Explanation
        Step 1: Setting up the Knowledge Base
        Step 2: Loading the Publications
        Step 3: Chunking Publications
        Step 4: Creating Embeddings
        Step 5: Storing in Vector Database
        Step 6: Intelligent Retrieval
        Step 7: Generating Research-Backed Answers

Overview

The notebook implements a RAG pipeline to:

    Initialize a vector database (ChromaDB).
    Load research publications from text files.
    Split the publications into smaller, manageable chunks.
    Generate embeddings for each chunk using a Hugging Face model.
    Store the chunks and their embeddings in the vector database.
    Retrieve relevant chunks based on a user query using semantic search.
    Use a Large Language Model (LLM) (Groq's Llama3) to generate an answer based on the retrieved information.

Setup
Prerequisites

    Google Colab environment or a local Python environment with necessary libraries.
    Access to a Groq API key.

Installation

The required libraries can be installed using pip. The following command installs all necessary packages:
