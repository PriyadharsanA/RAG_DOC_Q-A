📄 RAG-based Document Question Answering App:

This project implements a Retrieval-Augmented Generation (RAG) system that allows users to upload a PDF document and ask natural language questions.

The system retrieves relevant document chunks using vector similarity search and generates context-grounded answers using a Large Language Model (LLM).

🚀 Features

📄 Upload any PDF document

✂️ Automatic text chunking

🔎 Semantic retrieval using embeddings + FAISS

🧠 LLM-based generative answering

🚫 Hallucination-safe (answers restricted to retrieved context)

🌐 Interactive Streamlit web interface

☁️ Deployable on Google Colab

🧠 System Architecture (RAG Pipeline)
1. PDF Ingestion: Extract text from uploaded PDF.
2. Chunking: Split document text into overlapping chunks.
3. Embedding: Generate vector embeddings using a sentence-transformer model.
4. Vector Search: Store embeddings in FAISS and retrieve top-k relevant chunks for a query.
5. LLM Answering: Pass retrieved context to an LLM and generate a grounded, natural language answer.

🛠️ Tech Stack

Python

Streamlit – UI

Sentence-Transformers – Text embeddings

FAISS – Vector similarity search

OpenAI API – LLM-based answering

PyPDF – PDF text extraction

Google Colab – Execution & deployment

## How to Run
1. Install dependencies given in requirements.txt
2. Set the OpenAI API key
3. Run the Streamlit app using:
   streamlit run app.py

The full logic is implemented in the notebook, just copy the first cell from the notebook, and create app.py.
