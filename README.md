# Banking Policy Question Answering using RAG with Citations

**An AI-powered banking policy assistant using Retrieval-Augmented Generation (RAG) to provide contextual answers with source citations.**

---

## 1. Project Information

| Field | Details |
|---|---|
| Project Title | Banking Policy Question Answering using RAG with Citations |
| Project Number | P13 |
| Domain | Finance / Generative AI |
| Academic Year | 2026–2027 |
| Institution | Koneru Lakshmaiah Education Foundation |
| Project Status | In Development |

## 2. Team Members

| S. No. | Student ID | Name |
|---|---|---|
| 1 | 2520080012 | Saranya Aluru |
| 2 | 2520080069 | Ananya Maroju |
| 3 | 2520090093 | Yuktha Reddy |

## 3. Project Supervisor

**Dr. Dyuti Banerjee**

## 4. Abstract

Banking policies and financial regulations are often distributed across lengthy documents, making it difficult for customers and employees to locate specific information efficiently. Traditional keyword-based search systems may fail to understand the context and intent behind user queries.

This project proposes an AI-powered Banking Policy Question Answering System using Retrieval-Augmented Generation (RAG). The system processes banking policy documents, converts their contents into vector embeddings, and stores them in a vector database for efficient semantic retrieval.

When a user submits a natural-language question, the system retrieves relevant document sections and passes the contextual information to a Large Language Model (LLM) to generate an accurate and understandable response.

A key feature of the proposed system is source-level citations, allowing users to verify generated answers against the original banking documents.

The primary objective is to improve accessibility to banking information, reduce manual document searching, and provide transparent, context-aware responses while minimizing unsupported AI-generated information.

## 5. Objectives

- Develop an AI-powered banking policy question-answering system.
- Implement Retrieval-Augmented Generation for document-based responses.
- Enable semantic search across banking policy documents.
- Generate contextual answers using Large Language Models.
- Provide citations and references to original source documents.
- Reduce hallucinations by grounding responses in retrieved information.
- Improve accessibility and efficiency in retrieving banking information.

## 6. Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| Backend | FastAPI |
| Frontend | React |
| LLM Integration | OpenAI API / Open-Weight LLM |
| RAG Framework | LangChain |
| Embedding Model | Sentence Transformers |
| Vector Database | FAISS / ChromaDB |
| Document Processing | PyMuPDF |
| Database | PostgreSQL |
| Deployment | Docker |

*Final technology selections may be updated during implementation.*

## 7. System Architecture

```text
       Banking Policy Documents
                  |
                  v
          Document Processing
                  |
                  v
             Text Chunking
                  |
                  v
          Embedding Generation
                  |
                  v
            Vector Database
                  |
                  |
User Query ------+
      |
      v
Query Embedding
      |
      v
Semantic Retrieval
      |
      v
Relevant Document Chunks
      |
      v
       Large Language Model
      |
      v
    Contextual Answer
      |
      v
    Source Citations
```

## 8. Key Features

- Document-based question answering.
- PDF document ingestion and processing.
- Semantic search using vector embeddings.
- Context-aware answer generation.
- Source-level citations and references.
- Support for multiple banking policy documents.
- Handling questions with insufficient supporting information.
- Scalable backend architecture.

## 9. Setup and Execution Instructions

### Prerequisites

- Python 3.10 or later
- Node.js and npm
- Git
- VS Code or another code editor
- LLM API key, if using a hosted model

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/banking-policy-rag-assistant.git
cd banking-policy-rag-assistant
```

### Step 2: Backend Setup

```bash
cd backend
python -m venv .venv
```

Activate the environment.

**Windows:**
```powershell
.venv\Scripts\activate
```

**Linux / macOS:**
```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### Step 3: Configure Environment Variables

Create a `.env` file in the backend directory.

```env
LLM_API_KEY=your_api_key
DATABASE_URL=your_database_url
```

Never commit actual API keys or credentials to GitHub.

### Step 4: Run the Backend

```bash
uvicorn app.main:app --reload
```

Backend URL: `http://localhost:8000`

API documentation: `http://localhost:8000/docs`

### Step 5: Frontend Setup

Open another terminal:

```bash
cd frontend
npm install
npm run dev
```

Open the frontend URL displayed in your terminal.

### Step 6: Using the Application

1. Open the application in your browser.
2. Upload banking policy documents.
3. Allow the system to process and index the documents.
4. Enter a banking-related question.
5. View the AI-generated response.
6. Verify the answer using the provided source citations.

*Execution instructions will be updated to match the final implementation.*

## 10. Current Project Phase Status

**Overall Status: In Development**

| Phase | Description | Status |
|---|---|---|
| Phase 1 | Project selection and requirement analysis | To be updated |
| Phase 2 | System architecture and technology selection | To be updated |
| Phase 3 | Document ingestion and preprocessing | Not Started |
| Phase 4 | Embedding generation and vector database integration | Not Started |
| Phase 5 | RAG pipeline and LLM integration | Not Started |
| Phase 6 | Backend and frontend development | Not Started |
| Phase 7 | Testing and evaluation | Not Started |
| Phase 8 | Deployment and documentation | Not Started |

## 11. Evaluation Metrics

- Retrieval Recall@K
- Answer Faithfulness
- Answer Relevance
- Citation Accuracy
- Response Latency

## 12. Future Enhancements

- Hybrid search combining keyword and semantic retrieval.
- Reranking for improved retrieval accuracy.
- Support for multiple banking institutions.
- Multilingual banking question answering.
- Conversation history and contextual follow-up questions.
- Automated document version tracking.
- User authentication and role-based access control.
- Interactive analytics dashboard.
- Cloud deployment and scalability improvements.

## 13. Security and Disclaimer

- Responses should be grounded in available source documents.
- Unsupported questions should not result in fabricated answers.
- Uploaded documents should be handled securely.
- API credentials must be protected.
- Sensitive customer information should not be exposed.

**Disclaimer:** This project is an academic AI application and does not provide official banking, financial or legal advice. Users should verify important information with the relevant financial institution.

---

## Project Credits

**Project:** P13 – Banking Policy Question Answering using RAG with Citations

**Team Members:**
- Saranya Aluru (2520080012)
- Ananya Maroju (2520080069)
- Yuktha Reddy (2520090093)

**Project Supervisor:** Dr. Dyuti Banerjee

**Institution:** Koneru Lakshmaiah Education Foundation

**Academic Year:** 2026–2027

⭐ If you find this project interesting, consider starring the repository!
