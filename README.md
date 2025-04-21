
# 🧠 Mental Health Chatbot using LLM + RAG

This project implements a Mental Health Chatbot that uses **Retrieval-Augmented Generation (RAG)** with **LangChain**, **Groq API**, **Hugging Face Embeddings**, and **Astra DB (Vector Store)**. The chatbot provides context-aware responses through a Gradio interface using documents ingested into a vector database.

---

## 🧪 Features

- 📚 Uses your own mental health data as knowledge base
- ⚡ Groq for ultra-fast LLM inference
- 🔍 Hugging Face for embeddings
- 🗃️ Astra DB for vector search
- 🧠 LangChain for chaining LLM + Retriever
- 💬 Gradio UI for interactive chatbot experience

---

## 📁 Files

- `MAIN LLM_RAG.ipynb` – Main Jupyter Notebook containing entire implementation
- `.env` – Contains API keys and secrets
- `README.md` – Project documentation

---

## 🔧 Setup and Installation

### 1. Clone the Repository

```bash
git clone https://github.com/<nishithraut>/<mental-health-chatbot>.git
cd <mental-health-chatbot>
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. Install Dependencies

If you don't have `requirements.txt`, install manually:

```bash
pip install langchain cassio gradio groq python-dotenv openai transformers
```

Or use this `requirements.txt` content:

```txt
langchain
cassio
gradio
groq
python-dotenv
openai
transformers
```

Then run:

```bash
pip install -r requirements.txt
```

---

## 🔐 Environment Setup

Create a `.env` file in the root directory and add:

```env
ASTRA_DB_APPLICATION_TOKEN=your_astra_db_application_token
ASTRA_DB_ID=your_astra_db_id
HUGGINGFACEHUB_API_TOKEN=your_huggingface_token
GROQ_API_KEY=your_groq_api_key
```

If running in Colab or without `.env`, set them manually using:

```python
import os
os.environ["ASTRA_DB_APPLICATION_TOKEN"] = "your_token"
os.environ["ASTRA_DB_ID"] = "your_db_id"
os.environ["HUGGINGFACEHUB_API_TOKEN"] = "your_token"
os.environ["GROQ_API_KEY"] = "your_key"
```

---

