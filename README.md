
# 📚 PDF Question Answering System using RAG

An AI-powered Retrieval-Augmented Generation (RAG) application that allows users to upload PDF documents and ask natural language questions based on their content. The system retrieves relevant document chunks using semantic search and generates accurate, context-aware responses using Mistral AI.

---

## 🚀 Features

- Upload PDF documents
- Extract and split document text into chunks
- Generate semantic embeddings using Hugging Face Embeddings
- Store embeddings in ChromaDB (Vector Database)
- Retrieve relevant document chunks using MMR (Maximum Marginal Relevance)
- Generate context-aware answers using Mistral AI
- Interactive Streamlit web interface

---

## 🛠️ Tech Stack

- Python
- LangChain
- ChromaDB (Vector Database)
- Hugging Face Embeddings
- Mistral AI
- Streamlit
- PyPDFLoader

---

## 📂 Project Structure

```
pdf-rag-question-answering/
│
├── app.py                 # Streamlit application
├── main.py                # Command-line RAG application
├── create_database.py     # Creates Chroma Vector Database
├── requirements.txt
├── .env.example
├── README.md
```

## 📖 How It Works

1. Upload a PDF document.
2. Extract text from the PDF.
3. Split text into smaller chunks.
4. Generate embeddings using Hugging Face Embeddings.
5. Store embeddings in ChromaDB.
6. Retrieve relevant chunks using MMR.
7. Pass retrieved context to Mistral AI.
8. Generate accurate answers grounded in the uploaded document.

---

## 🏗️ Architecture

```
                PDF
                 │
                 ▼
          PyPDFLoader
                 │
                 ▼
 RecursiveCharacterTextSplitter
                 │
                 ▼
    Hugging Face Embeddings
                 │
                 ▼
      Chroma Vector Database
                 │
        MMR Retriever
                 │
                 ▼
      Retrieved Context
                 │
                 ▼
          Mistral AI
                 │
                 ▼
          Generated Answer
```

---

## 📸 Demo

Add screenshots or a GIF of the application here.

Example:

```
screenshots/home.png
screenshots/output.png
```

---

## 🔮 Future Improvements

- Multiple PDF support
- Chat history
- Source citations with page numbers
- Hybrid Search (BM25 + Vector Search)
- Conversation Memory
- Document summarization
- Docker deployment

---

## 👨‍💻 Author

**Aryan Swain**
