# 🏥 AI Health Report System

![Project Status](https://img.shields.io/badge/status-active-brightgreen.svg)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)

Welcome to the **AI Health Report System** repository! This platform is a robust, microservices-driven application designed to capture user symptoms, analyze medical data using AI/RAG pipelines, predict severity, and generate comprehensive PDF reports.

## 🌟 Project Overview

This system is built using a modern tech stack encompassing a **React** frontend, a **Node.js API Gateway**, various **Express.js** microservices for standard operations, and **FastAPI (Python)** microservices for heavy AI and Machine Learning computations.

Our architecture ensures high scalability, separation of concerns, and the ability to integrate cutting-edge AI models (LLMs, Scikit-learn) with standard health profiling operations.

---

## 🤝 Contribution Guidelines: Create & Contribute!

**To all project members:** This repository is designed to be highly modular so that everyone can leverage their specific strengths. **You are encouraged to create, build, and contribute according to your knowledge and assigned roles.** 

Whether you are a frontend wizard, a backend architect, or an AI/ML enthusiast, there is a space for you here:

*   🎨 **Frontend Team (React, Tailwind):** Focus on the `frontend/` directory. Enhance the UI/UX for symptom capture, report dashboards, and profile management.
*   ⚙️ **Backend Team (Node.js, Express, MongoDB):** Own the `services-node/` and `backend-gateway/` directories. Build out the Authentication, Profile, Intake, and Notification services.
*   🧠 **AI & ML Team (Python, FastAPI, LangChain):** Drive the intelligence in the `services-python/` directory. Optimize the RAG pipeline, refine the ChromaDB vector stores, and improve the Scikit-learn severity classifiers.

**Workflow:**
1. Pick up an issue or feature that aligns with your assigned role.
2. Create a new feature branch (e.g., `feature/frontend-intake-form` or `ai/rag-pipeline-optimization`).
3. Develop, test, and push your changes.
4. Open a Pull Request for review. Feel free to experiment and bring your best ideas to the table!

---

## 🏗️ System Architecture & Technologies

### 1. Frontend Client
* **Tech:** React, Vite, Tailwind CSS
* **Responsibilities:** User Login, Symptom Submission, Viewing Reports.

### 2. API Gateway
* **Tech:** Node.js, Express.js
* **Responsibilities:** Auth Middleware, Rate Limiting, Request Validation, Central Logging.

### 3. Core Microservices (Node.js)
| Service | Responsibilities | Technologies |
| :--- | :--- | :--- |
| **Authentication** | JWT Generation, Password Hashing | Express, bcrypt, JWT |
| **Profile** | User Vitals, Medical History | Express, MongoDB |
| **Intake** | Symptom Capture, Data Validation | Express, MongoDB |
| **Report** | Compile insights, Generate PDFs | Express, ReportLab, PDFKit |
| **Notification** | Emergency Alerts, Email | Nodemailer, SMTP |
| **History** | Store & Manage Reports, Analytics | Express, MongoDB |

### 4. AI & ML Microservices (Python)
| Service | Responsibilities | Technologies |
| :--- | :--- | :--- |
| **AI / RAG Service** | Context Retrieval, LLM Prompting | FastAPI, LangChain, ChromaDB |
| **Severity Classifier** | Risk Prediction, ML Inference | FastAPI, Scikit-learn, Joblib |

---

## 📂 Repository Structure

```text
ai-health-report-system/
├── frontend/                 # React client
├── backend-gateway/          # Central API Gateway
├── services-node/            # Express.js Microservices
├── services-python/          # FastAPI Microservices
└── infrastructure/           # Docker Compose, DB Configs
```

---

## 🚀 Local Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd ai-health-report-system
   ```

2. **Environment Variables:**
   Create a `.env` file in the root and respective service directories based on the `.env.example` templates.

3. **Running the System:**
   *(Instructions on Docker setup or individual service startup scripts will be added here as the infrastructure is finalized.)*

---

*Let's build something amazing together!*