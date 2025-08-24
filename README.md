# 🚀 AstraFlow – AI-Powered Task & Workflow Automation Platform

[![Tech Stack](https://img.shields.io/badge/stack-React%20%7C%20FastAPI%20%7C%20SpringBoot%20%7C%20Postgres%20%7C%20Docker-blue)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
[![CI](https://github.com/<your-username>/AstraFlow/actions/workflows/ci.yml/badge.svg)](#)

---

## 📌 Short Description
**AstraFlow** is a modern, **AI-powered task & workflow automation platform** designed to help teams manage projects, automate workflows, predict delays, and collaborate in real-time.  
Built as a **learning + practical monorepo project**, it demonstrates production-ready engineering across **frontend, backend, AI/ML, real-time systems, and DevOps**.

---

## ✨ Features / Highlights
- 🔐 **Authentication & RBAC** – Secure JWT auth, role-based access (Admin, Manager, Employee).
- ✅ **Tasks & Workflows** – CRUD tasks, dependencies, workflow builder with versioning.
- 🤖 **AI Assistance** – Text summarization, smart prioritization, and delay risk prediction (ML).
- ⚡ **Real-Time Collaboration** – Live updates, typing indicators, presence with Socket.IO.
- 📊 **Analytics Dashboard** – Burndown charts, workload heatmaps, SLA tracking.
- 📝 **Reports** – Export analytics to **CSV** or generate professional **PDF reports** via Java service.
- 🗄️ **Database** – PostgreSQL with Alembic migrations & seeders.
- 🐳 **DevOps Ready** – Docker Compose (dev/prod), GitHub Actions CI, optional Kubernetes.

---

## 🛠 Tech Stack

| Layer        | Tech Used |
|--------------|-----------|
| **Frontend** | React 18, Vite, TypeScript, TailwindCSS, React Router, React Query, React Hook Form, React Flow, Recharts, Socket.IO client |
| **Backend**  | Python FastAPI, SQLAlchemy + Alembic, PostgreSQL, Pydantic v2, PyJWT, passlib (bcrypt), python-socketio |
| **AI/ML**    | scikit-learn, transformers (DistilBART), fallback extractive summarizer |
| **Reports**  | Java Spring Boot 3, OpenHTMLtoPDF |
| **Real-Time**| Socket.IO (namespaces, rooms) |
| **Deploy**   | Docker Compose, GitHub Actions CI, optional Kubernetes manifests |
| **Testing**  | PyTest, Jest + RTL, JUnit |

---

## 📂 Project Structure
```plaintext
/astraflow
  ├── frontend/           # React + Vite app (UI & workflow builder)
  ├── backend/            # FastAPI backend (API, DB, AI, Socket.IO)
  ├── java-report-service/ # Spring Boot microservice for PDF generation
  ├── infra/              # Docker, Kubernetes, CI/CD configs
  ├── docs/               # Documentation & playbook
  ├── docker-compose.dev.yml
  ├── docker-compose.prod.yml
  ├── README.md
  └── LICENSE
