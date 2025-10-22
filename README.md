


# 🧠 ASKpdf — Indian Budget Q&A System

ASKpdf is an AI-powered **Retrieval-Augmented Generation (RAG)** system that allows users to ask natural language questions directly from **Indian Budget PDF documents**.  
It combines **semantic search** and **large language models** for accurate, context-aware answers — all delivered with **sub-second latency** ⚡.

---

## 🚀 Key Features

- 📄 **PDF Understanding:** Extracts and preprocesses information from complex government budget documents.  
- 🔍 **Semantic Search:** Uses embeddings for meaning-based retrieval instead of keyword matching.  
- ⚡ **Ultra-Low Latency:** Powered by **Groq API** for lightning-fast responses.  
- 🧩 **RAG Pipeline:** Built with **LangChain**, **Pinecone**, and **Hugging Face embeddings**.  
- 💬 **Context-Aware Answers:** Combines retrieved budget context with LLM reasoning.  
- 🖥️ **Simple Interface:** Can be extended with FastAPI or Streamlit for real-time querying.

---

## 🏗️ System Architecture

```

PDF Documents
│
▼
Text Preprocessing
│
▼
Hugging Face Embeddings ──► Pinecone Vector Database
│
▼
LangChain Retriever ──► Groq LLM Inference
│
▼
User Query ──► Context Retrieval ──► Final Answer

````

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-------------|
| **Language** | Python |
| **LLM Inference** | Groq API |
| **Framework** | LangChain |
| **Embeddings** | Hugging Face Sentence Transformers |
| **Vector Store** | Pinecone |
| **Interface (optional)** | Streamlit / FastAPI |
| **PDF Handling** | PyPDF2, LangChain DocumentLoaders |

---

## ⚙️ Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/<your-username>/ASKpdf.git
   cd ASKpdf
````

2. **Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**

   Create a `.env` file in your project root and add:

   ```env
   GROQ_API_KEY=your_groq_api_key
   PINECONE_API_KEY=your_pinecone_api_key
   PINECONE_ENV=your_pinecone_environment
   ```

5. **Run the app**

   ```bash
   python app.py
   ```

---

## 💡 Example Query

**User Input:**

> What is the total allocation for the Ministry of Agriculture in Union Budget 2024?

**System Output:**

> The Ministry of Agriculture has been allocated ₹1.52 lakh crore, reflecting a 5.6% increase from the previous fiscal year.

---

## 📊 Performance Metrics

| Metric                         | Result                                                       |
| ------------------------------ | ------------------------------------------------------------ |
| **Response Time**              | ~700 ms per query                                            |
| **Context Retrieval Accuracy** | >90%                                                         |
| **Scalability**                | Handles multiple queries simultaneously via Groq parallelism |

---

## 🔮 Future Enhancements

* [ ] Support for multiple PDF uploads
* [ ] Integration with OpenAI / Mistral models
* [ ] Query analytics dashboard
* [ ] Web-based interface for uploading and querying documents

---



⭐ *If you found this project useful, consider giving it a star!*

```


