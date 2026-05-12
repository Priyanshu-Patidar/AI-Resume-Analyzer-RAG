# 🤖 AI Resume Analyzer RAG (LangChain + LangGraph + Supabase)

An advanced **AI-powered Resume Analyzer system** that uses **Retrieval-Augmented Generation (RAG)** to evaluate resumes against job descriptions using **LangChain, LangGraph, OpenAI, and Supabase Vector Database**.

> 🚀 Built to simulate real-world ATS (Applicant Tracking System) behavior using modern AI agent architecture.

---

## ✨ Features

- 📄 **Resume Parsing & Processing**
  - Upload resumes (PDF format)
  - Extract and chunk text for AI processing

- 🧠 **AI Resume Analysis (RAG)**
  - Compare resumes with job descriptions
  - Semantic matching using embeddings
  - AI-generated scoring and feedback

- 🔁 **LangGraph Agent Workflow**
  - Structured ingestion pipeline
  - Retrieval-based evaluation pipeline
  - Debuggable graph-based AI flow

- ⚡ **Real-time AI Responses**
  - Streaming responses from backend to UI

- 🗄️ **Vector Database (Supabase)**
  - Stores embeddings for semantic search
  - Fast similarity-based retrieval

- 🌐 **Modern Web Interface**
  - Upload resumes easily
  - Chat-style AI feedback system

---

## 🧱 System Architecture
Frontend (Next.js / React)
│
│ Upload Resume + Job Description
▼
Backend (LangGraph Agent System)
│
├── Ingestion Graph
│ └── Resume → Text → Embeddings → Supabase
│
├── Retrieval Graph
│ └── Job Query → Vector Search → AI Evaluation
│
▼
OpenAI LLM + Supabase Vector DB


---

## 🛠 Tech Stack

- **Frontend:** React / Next.js, TailwindCSS  
- **Backend:** Node.js, TypeScript  
- **AI Frameworks:** LangChain, LangGraph  
- **LLM:** OpenAI API  
- **Vector DB:** Supabase (pgvector)  
- **Architecture:** RAG (Retrieval Augmented Generation)

---

## 📦 Installation

### 1. Clone the repository
```bash
git clone https://github.com/Priyanshu-Patidar/AI-Resume-Analyzer-RAG.git
cd AI-Resume-Analyzer-RAG
2. Install dependencies
yarn install
🔐 Environment Variables
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
🚀 Running the Project
▶ Start Backend (LangGraph)
cd backend
yarn langgraph:dev

Backend runs at:

http://localhost:2024
▶ Start Frontend
cd frontend
yarn dev

Frontend runs at:

http://localhost:3000
⚙️ How It Works
1. Resume Upload
Resume is uploaded (PDF)
Text is extracted and chunked
2. Embedding Generation
Text converted into embeddings
Stored in Supabase vector DB
3. Job Matching
Job description is converted into embeddings
Similar resumes/sections retrieved
4. AI Evaluation
LLM analyzes match
Generates:
Score
Feedback
Skill gaps
🧪 Troubleshooting
❌ OpenAI Error
Check API key & billing
❌ Supabase Error
Ensure documents table exists
Ensure vector extension is enabled
❌ Backend not running
Use Node.js v18+
🚀 Future Improvements
🔐 User authentication system
📊 Resume ranking dashboard
📄 Multi-format support (DOCX, TXT)
🤖 Multi-LLM support (Claude, Gemini)
☁️ Deployment (Vercel + Render)
👨‍💻 Author

Priyanshu Patidar

GitHub: https://github.com/Priyanshu-Patidar

⭐ If you like this project

Give it a ⭐ on GitHub to support the project!


---

# 🔥 Done

✔ Your correct project name used  
✔ Single-file README  
✔ Recruiter-ready formatting  
✔ Clean architecture + ATS-friendly description  
✔ No unnecessary repetition  

---

If you want next level upgrade, I can also:
- 🔥 :contentReference[oaicite:0]{index=0}
- 🔥 :contentReference[oaicite:1]{index=1}
- 🔥 :contentReference[oaicite:2]{index=2}
- 🔥 :contentReference[oaicite:3]{index=3}

Just tell me 👍
