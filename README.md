# PaperGen AI - AI Based Question Paper Generator

PaperGen AI is a full-stack web application designed to automatically generate high-quality question papers based on syllabi, difficulty levels, subject blueprints, and question types.

## 🏗️ Project Architecture

```text
PaperGen-AI/
 ├── frontend/      # Next.js 15 + TypeScript + Tailwind CSS + Shadcn UI
 ├── backend/       # Python FastAPI REST API
 ├── database/      # PostgreSQL initialization & schema scripts
 ├── uploads/       # Directory for syllabus and document uploads
 └── exports/       # Directory for generated PDF/DOCX question paper exports
```

## 🚀 Quick Start

### Prerequisites
- Node.js (v18+) & npm
- Python (v3.10+)
- Docker & Docker Compose (Optional, for database)
- PostgreSQL (if running locally without Docker)

---

### 1. Database Setup (Docker)
Start the PostgreSQL container:
```bash
docker-compose up -d
```
The database will be initialized using `database/init.sql`.

---

### 2. Backend Setup (FastAPI)
```bash
cd backend
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Linux/macOS:
source venv/bin/activate

pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000
```
Backend API will be running at: `http://localhost:8000`  
API Docs (Swagger): `http://localhost:8000/docs`

---

### 3. Frontend Setup (Next.js 15)
```bash
cd frontend
npm install
npm run dev
```
Frontend Web App will be running at: `http://localhost:3000`

---

## 🛠️ Tech Stack
- **Frontend**: Next.js 15 (App Router), React 19, TypeScript, Tailwind CSS, Shadcn UI, Lucide Icons
- **Backend**: FastAPI, Python 3.10+, SQLAlchemy, Pydantic v2
- **Database**: PostgreSQL 16
