# PDF Assistant

## 📌 Project Overview
PDF Assistant is an AI-powered tool that helps users retrieve relevant information from PDF documents based on user queries. It leverages **LangChain**, **RAG (Retrieval-Augmented Generation)**, and the **Groq API** to provide accurate and contextually relevant responses. This assistant can be used for document analysis, resume screening, research, and more.

## 🚀 Features
- Loads and processes PDFs using **LangChain's PyPDFLoader**
- Splits text into manageable chunks for better retrieval
- Embeds and stores documents in a **FAISS vector database**
- Uses a **Hugging Face embedding model** for efficient semantic search
- Retrieves relevant document sections using **RAG**
- Generates accurate responses using the **Groq API** with the **Llama-3.3-70b** model

## 🔧 Installation & Setup
### Prerequisites
- Python 3.8+
- Pip
- Groq API Key

### Steps to Install
1. Clone the repository:
```bash
   git clone https://github.com/MuhammadSheesShoaib/PDF-Ai-agent.git
   cd PDF-Ai-agent
```
2. Install dependencies:
```bash
  pip install -r requirements.txt
```
3. Create a .env file and add your Groq API key:
```env
  GROQ_API_KEY=your_api_key_here
```
4. Place your PDF document in the project directory and update the filename in `loader = PyPDFLoader("your-document.pdf").`

## 🛠 Usage
Run the Script
```bash
  python main.py
```
It will prompt you to enter a query, and the assistant will retrieve relevant information from the PDF and provide an answer.

## 📌 Technologies Used
- LangChain – For document processing and retrieval
- FAISS – Vector database for efficient search
- Hugging Face Embeddings – For document similarity search
- Groq API – To generate responses using Llama-3.3-70b
