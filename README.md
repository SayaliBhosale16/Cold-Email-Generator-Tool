# Cold Email Generator

An AI-powered tool designed to help Software and AI Services companies generate personalized cold emails using the Llama 3.1 Large Language Model (LLM), ChromaDB for vector storage, LangChain for orchestration, and Streamlit for a user-friendly interface.

## Table of Contents

- [Project Overview](#project-overview)
- [Tech Architecture](#tech-architecture)
  - [Llama 3.1 and Groq](#llama-31-and-groq)
  - [ChromaDB](#chromadb)
  - [LangChain](#langchain)
  - [Streamlit](#streamlit)
- [Notebook for Email Generation](#notebook-for-email-generation)
- [Project Structure](#project-structure)


## Project Overview

The **Cold Email Generator** is a tool aimed at simplifying the process of creating personalized cold emails for outreach by Software and AI Service companies. By leveraging advanced AI technologies, this project generates high-quality email content tailored to target audiences, significantly reducing the time and effort involved in cold outreach.

---

## Tech Architecture

### Llama 3.1 and Groq

**Llama 3.1** is an advanced open-source language model developed by Meta, known for its exceptional language comprehension and text generation capabilities. It serves as the backbone of our email generation, ensuring high-quality and contextually relevant outputs.

**Groq** is a high-performance hardware-accelerated inference platform that integrates seamlessly with Llama 3.1, enhancing speed and efficiency in generating email content.

### ChromaDB

**ChromaDB** is utilized as a vector store for managing embeddings and retrieving relevant information based on vector similarity. By using ChromaDB, the Cold Email Generator can quickly access job descriptions and company attributes, ensuring that generated emails are rich in context and highly personalized.

### LangChain

**LangChain** acts as the middleware, orchestrating interactions between the LLM, ChromaDB, and the email generation prompts. It simplifies the process of chaining prompts and outputs, enabling efficient handling of user requests.

### Streamlit

**Streamlit** is the chosen framework for developing an interactive web interface, allowing users to easily input details and receive generated emails in real-time. Its simplicity and effectiveness make it ideal for this application.

---

## Notebook for Email Generation

A Jupyter notebook is included to experiment with various email generation prompts and fine-tune the model's output. This notebook serves as a testing ground for different configurations, helping to optimize the quality of generated emails.

---

## Project Structure

```plaintext
Cold_Email_Generator/
│
├── app/
│   ├── main.py          # Streamlit app for user interaction
│   ├── chains.py        # LLM chain management (prompt generation, output parsing)
│   ├── utils.py         # Utility functions for text processing
│   └── resource/
│       └── .env         # Environment variables for API keys
│
├── models/
│   └── llama3.1/        # Placeholder for Llama model files
│
├── vector_store/
│   └── chromadb/        # Directory for ChromaDB storage
│
├── notebooks/
│   └── email_generation_notebook.ipynb  # Notebook for testing and prompt engineering
│
├── requirements.txt      # List of project dependencies
└── README.md             # Project README file



