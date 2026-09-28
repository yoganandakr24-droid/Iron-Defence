# Iron Defence 🛡️

**An Explainable Social-Engineering Firewall for Campus Communities** (ASYNC 2026)

Iron Defence detects, analyzes, and mitigates social engineering and phishing attacks across mobile notifications, SMS, text messages, URLs, screenshots, and QR codes using local deterministic checks and AI threat analysis engines.

---

## 🏗️ Repository Architecture

Designed to support modular execution across 3 development streams:

```text
irondef/
├── backend/    # FastAPI Backend + Threat Analysis Engines (Python 3.10+)
├── frontend/   # React + Vite Web Threat Analysis Dashboard (TypeScript)
└── android/    # Android Protection Application (Kotlin)
```

---

## 🚀 Development Phases

- [x] **Phase 1**: FastAPI backend + React web application (Health check & manual message analysis).
- [ ] **Phase 2**: AI Message analysis using Gemini Flash.
- [ ] **Phase 3**: Deterministic URL analysis + explainable risk engine.
- [ ] **Phase 4**: Android protection application.
- [ ] **Phase 5**: Automatic SMS/Notification URL extraction.
- [ ] **Phase 6**: Automatic URL analysis & Android notification warnings.
- [ ] **Phase 7**: Screenshot & OCR threat analysis.
- [ ] **Phase 8**: QR-code decoding & security analysis.
- [ ] **Phase 9**: Campus dashboard, threat history & Attack Story visualizer.
- [ ] **Phase 10**: Local Ollama + Gemma fallback integration.

---

## ⚙️ Quick Start (Phase 1)

### Backend Setup (FastAPI)

```bash
cd backend
python -m venv .venv
# Windows PowerShell:
.venv\Scripts\Activate.ps1
# Linux/macOS:
# source .venv/bin/activate

pip install -r requirements.txt
python -m uvicorn app.main:app --reload --port 8000
```

Backend API will be available at:
- Health Check: `http://localhost:8000/api/v1/health`
- Interactive API Docs: `http://localhost:8000/docs`

### Frontend Setup (React + Vite)

```bash
cd frontend
npm install
npm run dev
```

Frontend dashboard will be running at `http://localhost:5173`.
