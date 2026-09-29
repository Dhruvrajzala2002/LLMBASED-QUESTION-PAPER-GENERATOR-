<div align="center">

# 📝 PaperGen AI

### **Next-Gen Autonomous Question Paper & Examination Generator**

[![Next.js](https://img.shields.io/badge/Next.js-15.0-black?style=for-the-badge&logo=next.js&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.0-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.110+-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16.0-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

<p align="center">
  <b>Transform course syllabi into academic-grade, Bloom's Taxonomy-aligned examination papers in seconds.</b><br>
  Built with high-precision AI blueprints, interactive live editing, multi-format export (PDF & DOCX), and modern glassmorphic aesthetics.
</p>

[Explore Features](#-core-features) • [System Architecture](#-system-architecture) • [Quick Start](#-quick-start) • [API Documentation](#-api-endpoints) • [Roadmap](#-future-roadmap)

---

</div>

## 🌟 Overview

**PaperGen AI** is an enterprise-ready examination design system crafted for universities, schools, and academic coordinators. It eliminates hours of manual test drafting by combining **NLP syllabus topic extraction**, **Bloom's Cognitive Taxonomy rules**, and **mark-distribution blueprints** into a seamless workflow.

Whether you need a quick 20-mark class test, a 50-mark midterm, or a comprehensive 100-mark final semester examination with custom marking rubrics and answer keys, PaperGen AI generates balanced, deduplicated question papers in one click.

---

## ✨ Core Features

<table>
  <tr>
    <td width="50%">
      <h3>📄 Smart Syllabus Parser</h3>
      <ul>
        <li>Upload <b>PDF, DOCX, or TXT</b> syllabus documents.</li>
        <li>Automatic extraction and deduplication of key units, modules, and sub-topics.</li>
        <li>Intelligent filtering of administrative boilerplate and non-topic content.</li>
      </ul>
    </td>
    <td width="50%">
      <h3>🎯 Bloom's Taxonomy Cognitive Engine</h3>
      <ul>
        <li>Maps questions across all 6 cognitive domains: <b>Remember, Understand, Apply, Analyze, Evaluate, Create</b>.</li>
        <li>Action-verb enforcement tailored to academic difficulty standards.</li>
        <li>Enforces balanced cognitive distribution per exam blueprint.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>⚖️ Granular Blueprint & Difficulty Control</h3>
      <ul>
        <li>Configurable difficulty ratios (<b>% Easy, % Medium, % Hard</b>).</li>
        <li>Multi-section architecture (Section A, B, C, etc.) with custom instructions.</li>
        <li>Custom marks per question, optional choice configurations, and total mark validation.</li>
      </ul>
    </td>
    <td width="50%">
      <h3>🧩 Multi-Format Question Types</h3>
      <ul>
        <li><b>MCQs</b>: Realistic distractors with single unambiguous correct answers.</li>
        <li><b>Short Answers & Long Essays</b>: Complete with step-by-step marking rubrics.</li>
        <li><b>True/False, Fill in the Blanks & Numerical/Problem Solving</b>.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>✏️ Live Interactive Paper Studio</h3>
      <ul>
        <li>Inline text and mark editing with instant real-time synchronization.</li>
        <li><b>AI Single-Question Regeneration</b> with custom prompt hints & difficulty overrides.</li>
        <li>Section reordering, question deletion, and answer key inspector.</li>
      </ul>
    </td>
    <td width="50%">
      <h3>🖨️ Academic-Grade PDF & Word Export</h3>
      <ul>
        <li>Publication-ready PDF generation powered by <b>ReportLab</b>.</li>
        <li>Fully editable Microsoft Word (<b>.docx</b>) generation via <b>python-docx</b>.</li>
        <li>Custom institution headers, watermark options, and detachable <b>Answer Keys / Rubrics</b>.</li>
      </ul>
    </td>
  </tr>
</table>

---

## 🧠 Bloom's Taxonomy Cognitive Matrix

PaperGen AI strictly adheres to educational taxonomy guidelines to ensure test integrity and depth:

```text
               ▲  [CREATE]      - Design, Formulate, Construct, Propose
              / \
             /   \  [EVALUATE]   - Assess, Validate, Critique, Justify
            /     \
           /       \  [ANALYZE]    - Compare & Contrast, Differentiate, Deconstruct
          /         \
         /           \  [APPLY]      - Implement, Calculate, Solve, Execute
        /             \
       /               \  [UNDERSTAND]- Explain, Summarize, Classify, Illustrate
      /                 \
     /═══════════════════\  [REMEMBER]  - Define, List, State, Recall, Identify
```

| Cognitive Level | Action Verbs | Typical Question Formats | Weightage Target |
| :--- | :--- | :--- | :--- |
| **Remember (L1)** | *Define, List, State, Identify, Recall, Name* | MCQ, Fill in the Blanks, 2-Mark Short | ~20% - 30% |
| **Understand (L2)** | *Explain, Describe, Summarize, Distinguish, Discuss* | Short Answer (3-5 Marks), Concept MCQs | ~30% - 40% |
| **Apply (L3)** | *Demonstrate, Calculate, Apply, Implement, Solve* | Numerical Problems, Scenario MCQs | ~20% - 30% |
| **Analyze (L4)** | *Analyze, Compare & Contrast, Differentiate* | Long Answer (5-10 Marks), Case Studies | ~10% - 20% |
| **Evaluate (L5)** | *Evaluate, Assess, Validate, Critique, Justify* | Essay Questions, Design Critiques | Optional / Advanced |
| **Create (L6)** | *Design, Develop, Formulate, Propose Frameworks* | Comprehensive Long Form (10-15 Marks) | Optional / Advanced |

---

## 🏛️ System Architecture

```mermaid
flowchart TB
    subgraph Client ["Client Tier (Next.js 15 + TypeScript)"]
        A[Next.js App Router] --> B[Syllabus Upload & Parser UI]
        A --> C[Blueprint & Section Builder]
        A --> D[Live Paper Studio & Editor]
        A --> E[Export Manager PDF / Word]
    end

    subgraph API ["Application Tier (FastAPI REST Service)"]
        F[FastAPI Gateway] --> G[JWT Auth & RBAC Middleware]
        G --> H[Syllabus Extraction Service]
        G --> I[AI Generation & Deduplication Engine]
        G --> J[Export Engine: ReportLab & Python-docx]
    end

    subgraph Storage ["Data & Persistence Tier"]
        K[(PostgreSQL 16 / SQLite)]
        L[Local Uploads / Exports Storage]
    end

    B -->|Upload PDF/DOCX| F
    C -->|Generate Paper Request| F
    D -->|Inline Update / Single Regen| F
    E -->|Download Stream| F

    H --> L
    I --> K
    J --> L
```

---

## 📁 Repository Structure

```text
PaperGen-AI/
├── backend/
│   ├── app/
│   │   ├── api/                    # Route handlers & dependency injection
│   │   │   ├── deps.py             # Auth dependencies & token decoders
│   │   │   └── v1/
│   │   │       ├── endpoints/
│   │   │       │   ├── auth.py     # Login, register, profile
│   │   │       │   ├── papers.py   # Question paper generation & CRUD
│   │   │       │   └── syllabi.py  # Syllabus upload & topic extraction
│   │   │       └── router.py       # API v1 centralized router
│   │   ├── core/                   # App configuration & DB session factories
│   │   │   ├── config.py           # Pydantic BaseSettings & env loaders
│   │   │   ├── db.py               # SQLAlchemy declarative base & session engine
│   │   │   └── security.py         # Passlib bcrypt & JWT token handlers
│   │   ├── models/                 # SQLAlchemy ORM database models
│   │   │   ├── paper.py            # Syllabus, QuestionPaper, Section, Question models
│   │   │   └── user.py             # User model with role hierarchy
│   │   ├── schemas/                # Pydantic v2 validation schemas & DTOs
│   │   │   ├── paper.py            # Paper request, response, and blueprint schemas
│   │   │   └── user.py             # Auth & user schemas
│   │   ├── services/               # Core business & processing logic
│   │   │   ├── export_service.py   # ReportLab PDF & python-docx exporters
│   │   │   ├── llm_service.py      # Bloom's taxonomy generation & deduplication engine
│   │   │   └── parser_service.py   # PDF / DOCX syllabus text extraction
│   │   └── main.py                 # FastAPI application root & middleware
│   ├── requirements.txt            # Python dependencies
│   ├── .env.example                # Sample environment configuration
│   └── test_all_endpoints.py       # Comprehensive API test suite
│
├── frontend/
│   ├── src/
│   │   ├── app/                    # Next.js 15 App Router pages
│   │   │   ├── dashboard/          # Exam papers management hub
│   │   │   ├── generate/           # Interactive 4-step Paper Generator wizard
│   │   │   ├── papers/             # Live Paper Studio & editor
│   │   │   ├── syllabi/            # Syllabus repository manager
│   │   │   ├── login/              # Authentication view
│   │   │   ├── layout.tsx          # Root layout with dark mode tokens
│   │   │   └── page.tsx            # Modern landing page
│   │   ├── components/             # Reusable UI components & Radix primitives
│   │   ├── context/                # React state context (Auth, Paper state)
│   │   └── lib/                    # API client, Axios interceptors, utilities
│   ├── package.json                # Frontend package manifest
│   └── tailwind.config.ts          # Tailwind CSS styling configuration
│
├── database/
│   └── init.sql                    # Initial PostgreSQL schema & seed definitions
├── docker-compose.yml              # Multi-container orchestration (PostgreSQL)
└── README.md                       # Project documentation
```

---

## 🚀 Quick Start

### Prerequisites
Make sure you have the following installed on your machine:
- **Node.js** `v18.0+` & **npm** `v9.0+`
- **Python** `v3.10+` & **pip**
- **Docker & Docker Compose** (Optional, for containerized PostgreSQL)

---

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/PaperGen-AI.git
cd PaperGen-AI
```

---

### 2️⃣ Database Setup (Choose One Option)

#### Option A: Docker Compose (Recommended)
Spin up the isolated PostgreSQL 16 container with preloaded schemas:
```bash
docker-compose up -d
```

#### Option B: Local SQLite / PostgreSQL
The backend is configured with automatic SQLite fallback if PostgreSQL is not active. No extra setup required!

---

### 3️⃣ Backend Setup (FastAPI)

```bash
# Navigate to the backend directory
cd backend

# Create and activate a Python virtual environment
python -m venv venv

# Windows (Command Prompt / PowerShell)
venv\Scripts\activate

# Linux / macOS
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Create your .env file
cp .env.example .env

# Run the backend development server
uvicorn app.main:app --reload --port 8000
```

> 🌐 **Backend API:** `http://localhost:8000`  
> 📖 **Interactive Swagger Docs:** `http://localhost:8000/docs`  
> 📑 **ReDoc Documentation:** `http://localhost:8000/redoc`

---

### 4️⃣ Frontend Setup (Next.js 15)

```bash
# In a new terminal, navigate to the frontend directory
cd frontend

# Install Node dependencies
npm install

# Launch the Next.js development server
npm run dev
```

> 💻 **Frontend Web App:** `http://localhost:3000`

---

## ⚙️ Environment Variables

### Backend Configuration (`backend/.env`)

```env
PROJECT_NAME="PaperGen AI API"
VERSION="1.0.0"
API_V1_STR="/api/v1"

# Database Configuration (PostgreSQL)
POSTGRES_SERVER=localhost
POSTGRES_PORT=5432
POSTGRES_USER=papergen_user
POSTGRES_PASSWORD=papergen_password
POSTGRES_DB=papergen_db
DATABASE_URL=postgresql://papergen_user:papergen_password@localhost:5432/papergen_db

# Security & CORS
SECRET_KEY="super-secret-production-key-replace-this"
BACKEND_CORS_ORIGINS=["http://localhost:3000"]
```

---

## 📡 API Endpoints

### 🔐 Authentication (`/api/v1/auth`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/v1/auth/register` | Register a new educator or coordinator account |
| `POST` | `/api/v1/auth/login` | Authenticate and obtain JWT bearer access token |
| `GET` | `/api/v1/auth/me` | Fetch authenticated user profile and roles |

### 📚 Syllabus Management (`/api/v1/syllabi`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/v1/syllabi/` | List all uploaded course syllabi for current user |
| `POST` | `/api/v1/syllabi/upload` | Upload PDF/DOCX syllabus and auto-extract topics |
| `GET` | `/api/v1/syllabi/{id}` | Retrieve syllabus content, metadata, and extracted units |
| `DELETE`| `/api/v1/syllabi/{id}` | Delete a syllabus file and associated records |

### 📝 Question Paper Operations (`/api/v1/papers`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/v1/papers/generate` | Generate a full exam paper from blueprint & syllabus |
| `GET` | `/api/v1/papers/` | List all created question papers with status & metadata |
| `GET` | `/api/v1/papers/{id}` | Fetch full paper schema (sections, questions, answers) |
| `PUT` | `/api/v1/papers/{id}` | Save modifications, instructions, marks, and content |
| `POST` | `/api/v1/papers/{id}/regenerate-question` | AI-regenerate a single question with custom hint |
| `GET` | `/api/v1/papers/{id}/export/pdf` | Export publication-ready PDF with optional Answer Key |
| `GET` | `/api/v1/papers/{id}/export/docx` | Export editable Microsoft Word `.docx` paper |
| `DELETE`| `/api/v1/papers/{id}` | Remove a question paper from storage |

---

## 🧪 Testing & Verification

PaperGen AI comes with automated test suites for validation:

```bash
cd backend
python test_all_endpoints.py
```

```text
============================================================
             PAPERGEN AI - TEST VERIFICATION
============================================================
[✓] Authentication (Register / Login / Profile) -> PASS
[✓] Syllabus Ingestion & Topic Extraction       -> PASS
[✓] Bloom's Taxonomy Question Generation        -> PASS
[✓] Section & Question Deduplication Check       -> PASS
[✓] Single-Question AI Regeneration Engine      -> PASS
[✓] PDF & DOCX Binary Export Streaming          -> PASS
============================================================
RESULT: ALL TESTS PASSED (100% SUCCESS RATE)
============================================================
```

---

## 🔮 Future Roadmap

- [ ] **Multi-Model LLM Gateway**: Plug-and-play toggle between Gemini 1.5 Pro, OpenAI GPT-4o, Anthropic Claude 3.5, and Local Ollama (DeepSeek/Llama 3).
- [ ] **LaTeX & Math Formula Support**: Native KaTeX / MathJax rendering for complex mathematical & scientific expressions.
- [ ] **Diagram & Image Question Generation**: Auto-attachment of technical schematic questions.
- [ ] **LMS Integrations**: One-click export to Moodle, Google Classroom, and Canvas QTI formats.
- [ ] **Automated Difficulty Scoring**: Real-time student performance simulation and readability indexing.

---

## 🤝 Contributing

Contributions are welcome! Follow these steps:
1. **Fork the Repository**
2. **Create a Feature Branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit Your Changes** (`git commit -m "Add AmazingFeature"`)
4. **Push to the Branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for details.

<div align="center">
  <sub>Built with ❤️ for Educators, Institutions, and Academic Innovators.</sub>
</div>
