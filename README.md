# 📄 Document-Based Question Answering (RAG) Application

A **Retrieval-Augmented Generation (RAG)** application built using **Streamlit**, **LangChain**, **FAISS**, and **Mistral AI**.  
This app allows users to upload a PDF document and ask questions whose answers are generated **strictly from the document content**, with support for **multiple output languages**.

---

## 🚀 Features

- Upload and process **PDF documents**
- Semantic search using **FAISS vector database**
- Context-aware question answering using **Mistral Large LLM**
- Multilingual answer generation
- Predefined questions + custom user queries
- Hallucination-safe (answers only from source document)

---

## 🧠 RAG Pipeline

1. **PDF Loading** – `PyPDFLoader`
2. **Text Chunking** – `RecursiveCharacterTextSplitter`
3. **Embeddings** – Sentence Transformers (`all-MiniLM-L6-v2`)
4. **Vector Store** – FAISS
5. **Similarity Retrieval**
6. **Answer Generation** – `ChatMistralAI`

---

## 🛠️ Tech Stack

- **Frontend:** Streamlit  
- **LLM:** Mistral (`mistral-large-latest`)  
- **Framework:** LangChain  
- **Embeddings:** Sentence Transformers  
- **Vector Database:** FAISS  
- **Env Management:** python-dotenv  

---

## 📦 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/document-rag-app.git
cd document-rag-app
