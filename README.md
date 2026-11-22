# 🚀 AIFORGE — Empowering Minds Through Artificial Intelligence

[![Python Version](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![React Version](https://img.shields.io/badge/React-18.2-61dafb.svg?logo=react&logoColor=black)](https://react.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-38bdf8.svg?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Flask](https://img.shields.io/badge/Flask-3.0.3-000000.svg?logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-1.6-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas%20%2F%20Local-47A248.svg?logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Gemini AI](https://img.shields.io/badge/Google_Gemini-2.5_Flash-8E75C2.svg?logo=google-gemini&logoColor=white)](https://ai.google.dev/)

> **AIFORGE** is an end-to-end, adaptive artificial intelligence and machine learning education platform. It combines predictive machine learning models, retrieval-augmented generation (RAG), voice-enabled conversational AI, interactive data structures & algorithms (DSA) arenas, spaced-repetition cognitive scheduling, and dynamic technical interview simulators to deliver personalized learning paths for students and engineers.

---

## 📑 Table of Contents
1. [Platform Overview & Core Mission](#-platform-overview--core-mission)
2. [Key Features Breakdown](#-key-features-breakdown)
3. [Technology Stack & Usage Matrix](#-technology-stack--usage-matrix)
4. [System Architecture](#-system-architecture)
5. [Project Directory Structure](#-project-directory-structure)
6. [Getting Started & Local Setup](#-getting-started--local-setup)
7. [Environment Configuration (.env)](#-environment-configuration-env)
8. [API Endpoints Overview](#-api-endpoints-overview)
9. [How to Add & Push this Project to GitHub](#-how-to-add--push-this-project-to-github)
10. [Troubleshooting & FAQ](#-troubleshooting--faq)

---

## 🌟 Platform Overview & Core Mission

Standard online learning platforms treat every student identically, providing static videos and one-size-fits-all quizzes. **AIFORGE** replaces static curricula with a **closed-loop adaptive learning engine**:

- **Real-Time Skill Profiling:** Diagnoses prior background, math affinity, and coding speed.
- **Predictive AutoML Engine:** Runs 7 machine learning models to benchmark student trajectory and predict exam readiness.
- **Voice-Enabled Tutoring:** Uses speech recognition and generative LLMs to answer theoretical questions, derive mathematical proofs, and generate runnable code.
- **Cognitive Retention:** Implements the **SuperMemo SM-2 spaced repetition algorithm** to prevent memory decay.
- **Interview Simulator:** Conducts technical mock interviews with voice interaction, progressive hints, and rubric-based feedback.

---

## 🎯 Key Features Breakdown

### 1. 🔐 Clean Authentication & Secure Session Engine
* **What it does:** Provides secure student onboarding, login, and registration.
* **How it works:** Passwords are never stored as plain text. The backend hashes all credentials using **PBKDF2 with SHA-256** and salt via Werkzeug. Secure HTTP cookies and an initial clean-slate entry guarantee that opening the app presents an unpolluted sign-in screen without leftover credentials.

### 2. 🎯 Goal-Aware Learning Path Generator
* **What it does:** Allows students to select their exact career target and dynamically maps learning modules.
* **Available Tracks:**
  * **ML for Placement:** Technical coding, algorithmic interviews, feature engineering, and model evaluation.
  * **Data Science Specialist:** Exploratory Data Analysis (EDA), statistics, hypothesis testing, and business metrics.
  * **Deep Learning & GenAI:** Neural networks, Transformers, Large Language Models (LLMs), and Diffusion models.
  * **Core AI Foundations:** Search algorithms, heuristics, knowledge representation, and expert systems.

### 3. 🤖 AutoML Predictive & Diagnostic Ensemble
* **What it does:** Benchmarks student quiz scores, study hours, video completion, and practice tasks to predict knowledge mastery.
* **How it works:** Trains and compares 7 distinct machine learning algorithms simultaneously:
  * **Classifiers:** Random Forest, Gradient Boosting, Extra Trees, Support Vector Classifier (SVC), K-Nearest Neighbors (KNN), and Logistic Regression.
  * **Regressors:** Linear Regression, Ridge, Lasso, and Random Forest Regressor.
  * Generates an AutoML Leaderboard showing real-time Accuracy, Mean Absolute Error (MAE), and identifies the best-performing model.

### 4. 🎙️ AI Voice Tutor & Dual-Mode RAG Chatbot
* **What it does:** Acts as a 24/7 personal professor answering natural language questions via voice or text.
* **Dual Intelligence Layers:**
  * **Cloud LLM (Gemini 2.5 Flash):** Generates step-by-step mathematical explanations, concept analogies, and runnable Python/C++/Java code.
  * **Local Semantic Search (RAG):** When offline or operating without external API access, uses **TF-IDF Vectorization & Cosine Similarity** across local topic encyclopedias to return grounded curriculum notes.
* **Voice Support:** Powered by the browser **Web Speech API** (`SpeechRecognition` for audio capture and `SpeechSynthesis` for natural voice narration).

### 5. 💻 DSA Adaptive Arena & Practice Workspace
* **What it does:** Interactive practice arena for Data Structures & Algorithms with 19 core topic modules (Arrays, Sliding Window, Binary Search, Trees, Graphs, Dynamic Programming, Backtracking, etc.) and over 200 curated problems.
* **Features:** In-browser code editing, complexity analysis (Big-O time and space), and multi-language support (Java, Python, C++).

### 6. 👔 Dynamic AI Mock Interviewer
* **What it does:** Simulates real-world engineering and data science technical interview rounds.
* **Features:**
  * Progressive 3-tier hints (Concept nudge → Algorithmic strategy → Full code solution).
  * Timed live interview sessions.
  * Real-time automated grading against criteria: algorithmic correctness, edge case handling, and communication clarity.

### 7. 🎯 Weak Areas & Mistake Pattern Analyzer
* **What it does:** Continuously scans assessment submissions to catch bad coding habits and conceptual misconceptions.
* **Features:** Identifies specific issues (e.g., *Overfitting on high-variance data*, *Off-by-one errors in binary search*, *Gradient explosion in deep layers*) and generates instant **15-minute high-priority remedial drills**.

### 8. ⏱️ Daily Study Planner & SM-2 Spaced Retention
* **What it does:** Scientifically structures the student's study day based on their available time (30 min, 1 hr, 2 hr, 3 hr).
* **Cognitive Algorithm:** Implements the **SuperMemo SM-2 algorithm**, scheduling flashcard and quiz reviews at mathematically calculated intervals to maximize long-term retention.

### 9. 📄 Syllabus & Notes Extractor
* **What it does:** Ingests raw university syllabus text or PDF curriculum outlines.
* **Features:** Automatically extracts core topics, detects prerequisites, establishes module sequences, and generates customized flashcards and quizzes.

### 10. 📊 Interactive Visual Analytics Dashboard
* **What it does:** Delivers high-definition visual telemetry on the student's cognitive growth.
* **Visuals (Recharts):** Multi-axis radar charts for skill breadth, velocity curves, quiz score distributions, and real-time study streak trackers.

---

## 🛠️ Technology Stack & Usage Matrix

| Technology | Category | Where Used in Code | Exact Role & Purpose |
| :--- | :--- | :--- | :--- |
| **React 18** | Frontend Framework | `frontend/src/App.jsx`, `frontend/src/pages/*` | Single Page Application (SPA) reactive UI and component architecture |
| **React Router v6** | Client Routing | `frontend/src/App.jsx` | Client-side page navigation, URL parameters, and private route guards |
| **Tailwind CSS** | UI Styling | `frontend/tailwind.config.js`, `index.css` | Cyberpunk dark-mode design system, glassmorphism, responsive layouts |
| **Recharts** | Data Visualization | `frontend/src/pages/DashboardPage.jsx` | Renders radar charts, progress lines, and accuracy trend graphs |
| **Framer Motion** | UI Animation | `frontend/src/pages/HomePage.jsx` | Smooth animations, interactive card transitions, and micro-interactions |
| **Lucide React** | Iconography | `frontend/src/components/Layout.jsx` | High-quality, lightweight SVG iconography across all pages |
| **Web Speech API** | Voice AI (STT/TTS) | `frontend/src/services/voiceService.js` | Real-time speech-to-text recognition and text-to-speech audio synthesis |
| **SuperMemo SM-2** | Cognitive Science | `frontend/src/services/adaptiveEngine.js` | Calculates memory decay curves and schedules optimal revision intervals |
| **Python 3 & Flask** | Backend Web API | `app.py` | High-performance RESTful API server, routing, and controller logic |
| **Flask-CORS** | Security / Headers | `app.py` | Configures Cross-Origin Resource Sharing and secure cookie exchanges |
| **Werkzeug Security** | Cryptography | `services/db_service.py` | PBKDF2 with SHA-256 password hashing for safe credential storage |
| **Google Gemini 2.5** | Generative AI / LLM | `services/llm_tutor_service.py` | Large Language Model generating explanations, answers, and evaluations |
| **Scikit-Learn** | Machine Learning | `services/automl_service.py` | 7 ML models (Random Forest, SVM, KNN, GB, etc.) and preprocessing pipelines |
| **TF-IDF & Cosine** | Local Semantic Search | `services/llm_tutor_service.py` | Offline Vector RAG retrieving textbook notes based on query similarity |
| **Pandas & NumPy** | Data Wrangling | `services/real_data_service.py` | Matrix transformations, DataFrame cleaning, and numerical data processing |
| **MongoDB & PyMongo** | Database | `services/db_service.py` | NoSQL document storage (`AIEDUCATION`) for users, quizzes, and history |
| **In-Memory Engine** | Resilience Fallback | `services/db_service.py` | Automatic zero-crash in-memory fallback when MongoDB is not running |
| **Gunicorn** | WSGI Server | `Procfile` | Production multi-worker WSGI server for cloud deployment (Render) |

---

## 🏛️ System Architecture

```
                                  USER BROWSER
                                        │
                 ┌──────────────────────┴──────────────────────┐
                 ▼                                             ▼
        [React 18 Frontend]                           [Web Speech API]
        • Tailwind & Glassmorphic UI                  • Speech-to-Text (STT)
        • Recharts Visual Analytics                   • Text-to-Speech (TTS)
        • SM-2 Cognitive Planner                               │
                 │                                             │
                 └──────────────────────┬──────────────────────┘
                                        │ HTTP REST Requests (JSON / CORS)
                                        ▼
                               [Flask Backend API]
                               (Python 3.10+ / app.py)
                                        │
         ┌──────────────────────────────┼──────────────────────────────┐
         ▼                              ▼                              ▼
  [AI / LLM & RAG Layer]       [AutoML Engine]              [Persistence Layer]
  • Gemini 2.5 Flash API       • 7 Scikit-Learn Models      • MongoDB (PyMongo)
  • TF-IDF Vectorizer          • ColumnTransformer Pipeline • In-Memory Fallback
  • Cosine Similarity          • Performance Leaderboard    • Werkzeug PBKDF2 Hash
```

---

## 📁 Project Directory Structure

```text
AutoLearn-main/
├── app.py                         # Main Flask REST API server & SPA server
├── requirements.txt               # Python package dependencies
├── .env                           # Environment secrets (MongoDB URI, Gemini Key)
├── .env.example                   # Example environment variable template
├── Procfile                       # Gunicorn entrypoint for Render deployment
├── run.sh                         # Unified startup shell script
├── RUN.md                         # Quick run guide
├── README.md                      # Complete project documentation
│
├── services/                      # Python backend business logic
│   ├── automl_service.py          # Scikit-Learn 7-model training & leaderboard
│   ├── catalog_service.py         # YouTube, Kaggle, and course resource ranking
│   ├── db_service.py              # MongoDB driver with automated in-memory fallback
│   ├── interview_service.py       # Technical interview evaluation algorithms
│   ├── llm_tutor_service.py       # Gemini 2.5 Flash + Local TF-IDF RAG engine
│   └── real_data_service.py       # Student dataset ingestion and normalizer
│
├── data/                          # Dataset files and sample learning records
│   └── raw/                       # Raw CSV learning analytics datasets
│
└── frontend/                      # React 18 single-page application
    ├── package.json               # Frontend dependencies & npm scripts
    ├── tailwind.config.js         # Cyberpunk/Neon Tailwind configuration
    ├── vercel.json                # Vercel SPA routing & deployment config
    ├── public/
    │   ├── index.html             # HTML entry point with AIFORGE branding
    │   └── background.jpg         # Parallax space nebula background asset
    └── src/
        ├── App.jsx                # Root router & route guard definitions
        ├── index.css              # Custom neon gradients, animations & scrollbars
        ├── components/
        │   └── Layout.jsx         # Sticky navigation header & user profile status
        ├── context/
        │   └── AuthContext.jsx    # Session state, login/logout, clean-start logic
        ├── hooks/
        │   └── useFlaskData.js    # Data fetching hook connecting frontend to API
        ├── pages/
        │   ├── HomePage.jsx       # Landing page with clean Sign-In / Sign-Up
        │   ├── GoalSelectionPage  # 4-track career goal selector
        │   ├── StartPage.jsx      # Diagnostic assessment launcher
        │   ├── QuizPage.jsx       # Interactive multiple-choice & coding quizzes
        │   ├── DashboardPage.jsx  # Recharts mastery telemetry & AutoML stats
        │   ├── TutorPage.jsx      # AI Voice Tutor chat interface
        │   ├── InterviewPage.jsx  # Dynamic mock technical interview arena
        │   ├── DSAPage.jsx        # 19 DSA module curriculum & practice
        │   ├── StudyPlannerPage   # Time-aware daily sprint with SM-2 revision
        │   ├── WeakAreasPage.jsx  # Mistake pattern detector & remedial drills
        │   ├── SyllabusExtractor  # AI-driven syllabus & lecture note parser
        │   ├── KnowledgeGraphPage # Visual concept dependency graph
        │   └── ResourcesPage.jsx  # Curated videos, datasets, and tutorials
        ├── services/
        │   ├── adaptiveEngine.js  # SM-2 algorithm & cognitive mastery tracking
        │   ├── dsaService.js      # 200+ DSA problem dataset & solutions
        │   ├── interviewService.js# Dynamic interview questions & rubrics
        │   └── voiceService.js    # Web Speech API adapter (STT / TTS)
        └── utils/
            ├── api.js             # Centralized fetch wrapper with CORS credentials
            └── mockData.js        # Fallback dataset for zero-latency development
```

---

## 🚀 Getting Started & Local Setup

### Prerequisites
- **Python:** Version 3.10 or higher
- **Node.js:** Version 18.x or higher (with `npm`)
- **MongoDB (Optional):** Local MongoDB Community Server running on `localhost:27017` or a free MongoDB Atlas connection string. *(If you don't have MongoDB installed, the project automatically uses its built-in in-memory fallback engine).*

---

### Step 1: Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/AIFORGE.git
cd AIFORGE
```

---

### Step 2: Backend Setup (Python & Flask)

1. **Create and activate a virtual environment:**
   * **Windows (PowerShell):**
     ```powershell
     python -m venv .venv
     .\.venv\Scripts\Activate.ps1
     ```
   * **Mac / Linux:**
     ```bash
     python3 -m venv .venv
     source .venv/bin/activate
     ```

2. **Install Python dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Verify Python packages:**
   ```bash
   python -m py_compile app.py
   ```

---

### Step 3: Frontend Setup (React)

1. **Navigate to the frontend folder and install packages:**
   ```bash
   cd frontend
   npm install
   ```

2. **Test build the frontend:**
   ```bash
   npm run build
   ```

3. **Return to project root:**
   ```bash
   cd ..
   ```

---

## ⚙️ Environment Configuration (.env)

Create a `.env` file in the project root directory (a template is available in `.env.example`):

```env
# MongoDB Connection
MONGODB_URI=mongodb://localhost:27017/
MONGODB_DB_NAME=AIEDUCATION

# AI / Large Language Model
GEMINI_API_KEY=your_google_gemini_api_key_here
GEMINIAI_MODEL=gemini-2.5-flash

# Security Session Secret
SECRET_KEY=aiforge-fullstack-secret-key-2026
```

> **Note on Gemini API Key:** You can generate a free Gemini API key from [Google AI Studio](https://aistudio.google.com/). If omitted, the platform automatically switches to its local Scikit-Learn TF-IDF semantic search engine.

---

## 🏃 Running the Application

### Option A: Development Mode (Hot Reloading — Recommended)
Run the backend and frontend in two separate terminals:

* **Terminal 1 (Backend API on Port 5000):**
  ```bash
  python app.py
  ```
  *API runs at:* `http://localhost:5000`

* **Terminal 2 (Frontend React on Port 3000):**
  ```bash
  cd frontend
  npm start
  ```
  *Application opens at:* `http://localhost:3000`

---

### Option B: Unified Production Server
Build the React frontend into static assets and serve everything through Flask:
```bash
cd frontend && npm run build && cd ..
python app.py
```
Open your browser at **`http://localhost:5000`**.

---

## 🌐 API Endpoints Overview

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/auth/register` | Creates a new student account (PBKDF2 salted hash) |
| `POST` | `/api/auth/login` | Authenticates student and creates a secure session |
| `GET` | `/api/auth/me` | Returns currently signed-in student profile |
| `POST` | `/api/auth/logout` | Clears student authentication session |
| `POST` | `/api/tutor/chat` | Interacts with Gemini 2.5 Flash / TF-IDF RAG tutor |
| `GET` | `/api/models/predict` | Runs 7-model AutoML inference on learner metrics |
| `GET` | `/api/quiz/generate` | Generates diagnostic questions for a topic |
| `POST` | `/api/quiz/submit` | Evaluates answers and updates mastery score |
| `GET` | `/api/data/status` | Reports MongoDB connection status & dataset rows |

---

## 🐙 How to Add & Push this Project to GitHub

Follow these exact steps in your terminal to initialize git, commit all files (including this `README.md`), and push to your GitHub account:

### Step 1: Open Terminal in the Project Root
Make sure you are in `AutoLearn-main` (the folder containing `app.py` and `README.md`).

### Step 2: Check Git Status
```bash
git status
```

### Step 3: Initialize Git (If not already initialized)
```bash
git init
```

### Step 4: Ensure `.gitignore` Excludes Unneeded Files
Verify or create a `.gitignore` file in your root folder:
```gitignore
# Virtual Environment
.venv/
venv/
__pycache__/
*.pyc

# Node & Frontend
node_modules/
frontend/node_modules/
frontend/build/
.DS_Store

# Sensitive Secrets
.env
```

### Step 5: Stage All Project Files
```bash
git add .
```

### Step 6: Commit the Changes
```bash
git commit -m "feat: complete AIFORGE platform with full README documentation and modern AI features"
```

### Step 7: Create a New Repository on GitHub
1. Open [GitHub](https://github.com/) in your browser and sign in.
2. Click the **`+`** icon in the top right corner and select **New repository**.
3. Name your repository (e.g., `AIFORGE` or `aiforge-platform`).
4. Set it to **Public** (or **Private**).
5. **Do NOT** check "Add a README file" or ".gitignore" (we already created them locally).
6. Click **Create repository**.

### Step 8: Link and Push to Your GitHub Repository
Run the following commands in your terminal (replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual GitHub username and repository name):

```bash
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

*(If you already have a remote configured, simply run `git push origin main`)*.

---

## ❓ Troubleshooting & FAQ

* **Q: What if MongoDB is not installed on my computer?**
  * **A:** Nothing breaks! `services/db_service.py` detects that MongoDB is offline and automatically activates an in-memory data store. All accounts, logins, quizzes, and learning paths will work seamlessly for demos and presentations.
* **Q: Why does the voice tutor not speak or listen?**
  * **A:** Ensure you are using a modern Chromium-based browser (Google Chrome, Microsoft Edge, Brave) and that you have granted microphone permissions in your browser bar.
* **Q: Can I run this without a paid Gemini API key?**
  * **A:** Yes! Gemini 2.5 Flash has a free tier on Google AI Studio. Even without any API key, the built-in Scikit-Learn TF-IDF vectorizer answers topic questions using local course notes.

---

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).

---

<p align="center">
  <b>AIFORGE</b> — Built with passion for adaptive, intelligent, and accessible AI/ML education.
</p>
