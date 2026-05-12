# 🤖 AI Resume Analyzer RAG (LangChain + LangGraph + Supabase)

An AI-powered **Resume Analyzer system** built using **Retrieval-Augmented Generation (RAG)** that evaluates resumes against job descriptions using **LangChain, LangGraph, OpenAI, and Supabase Vector Database**.

This project simulates a real-world **ATS (Applicant Tracking System)** using modern AI agent architecture.

---

## ✨ Features

- 📄 Resume Upload & Parsing
  - Upload PDF resumes
  - Extract and process text for AI analysis

- 🧠 AI Resume Evaluation (RAG System)
  - Semantic matching between resume and job description
  - AI-generated scoring and feedback
  - Skill gap detection

- 🔁 LangGraph Agent Workflow
  - Structured ingestion pipeline
  - Retrieval-based evaluation pipeline
  - Fully modular graph-based AI architecture

- ⚡ Real-time AI Responses
  - Streaming responses from backend to frontend

- 🗄️ Vector Database (Supabase)
  - Stores embeddings for semantic search
  - Fast similarity-based retrieval

- 🌐 Modern Web Interface
  - Upload resumes easily
  - Chat-style AI feedback system

---

## 🧱 Architecture Overview

Frontend (React / Next.js)
        │
        │ Upload Resume + Job Description
        ▼
Backend (LangGraph Agent System)
        │
        ├── Ingestion Graph
        │     └── Resume → Text → Embeddings → Supabase
        │
        ├── Retrieval Graph
        │     └── Job Query → Vector Search → LLM Analysis
        │
        ▼
OpenAI LLM + Supabase Vector DB

---

## 🛠 Tech Stack

- Frontend: React / Next.js, TailwindCSS  
- Backend: Node.js, TypeScript  
- AI Frameworks: LangChain, LangGraph  
- LLM: OpenAI API  
- Vector Database: Supabase (pgvector)  
- Architecture: RAG (Retrieval Augmented Generation)

---

## 📦 Installation

### 1. Clone the repository
git clone https://github.com/Priyanshu-Patidar/AI-Resume-Analyzer-RAG.git
cd AI-Resume-Analyzer-RAG

### 2. Install dependencies
yarn install

---

## 🔐 Environment Variables

Backend .env
OPENAI_API_KEY=your_openai_api_key
SUPABASE_URL=your_supabase_url
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_key
LANGCHAIN_TRACING_V2=true
LANGCHAIN_PROJECT=ai-resume-analyzer

Frontend .env
NEXT_PUBLIC_LANGGRAPH_API_URL=http://localhost:2024
LANGGRAPH_INGESTION_ASSISTANT_ID=ingestion_graph
LANGGRAPH_RETRIEVAL_ASSISTANT_ID=retrieval_graph
LANGCHAIN_TRACING_V2=true
LANGCHAIN_PROJECT=ai-resume-analyzer

---

## 🚀 Running the Project

### Backend
cd backend
yarn langgraph:dev

Runs at:
http://localhost:2024

### Frontend
cd frontend
yarn dev

Runs at:
http://localhost:3000

---

## ⚙️ How It Works

1. Resume Upload → PDF parsed  
2. Embeddings generated  
3. Stored in Supabase vector DB  
4. Job description matched using similarity search  
5. LLM generates score + feedback  

---

## 🧪 Troubleshooting

- OpenAI error → check API key  
- Supabase error → enable pgvector + table setup  
- Backend not running → use Node v18+  

---

## 🚀 Future Improvements

- Authentication system  
- Resume ranking dashboard  
- Multi-format support  
- Multi-LLM support  
- Cloud deployment  

---

## 👨‍💻 Author

Priyanshu Patidar  
GitHub: https://github.com/Priyanshu-Patidar

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub.
