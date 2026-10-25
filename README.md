# SevaHealth AI 🏥

**AI-Native Preventive Healthcare & NCD Early-Warning Platform**

SevaHealth AI is an AI-assisted preventive healthcare platform designed to support early identification of Non-Communicable Disease (NCD) risks, explain contributing risk factors, and encourage preventive lifestyle changes.

The platform supports citizens, healthcare workers, clinicians, and public health administrators through integrated screening, risk assessment, care planning, and health monitoring workflows.

## ✨ Key Features

- **Health Screening:** CBAC and IDRS-based screening workflows.
- **Risk Assessment:** Multi-factor NCD risk stratification with explainable risk factors.
- **Preventive Care Plans:** Personalized 30-day lifestyle and habit recommendations.
- **Health Monitoring:** Daily check-ins and wearable biometric integration.
- **Clinical Triage:** High-risk alerts, referrals, and AI-assisted SOAP notes.
- **Population Health Analytics:** District-level dashboards and outcome monitoring.
- **Clinical Safety:** Human-in-the-loop review for escalated cases.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Backend development |
| FastAPI | REST API development |
| PostgreSQL 16 | Database |
| JSONB | Flexible data storage |
| AI/LLM Providers | AI-assisted workflows |
| Docker | Containerization |
| Swagger/OpenAPI | API documentation |

## 🏗️ Architecture

The project follows a modular architecture with separate application interfaces and backend services for screening, risk assessment, preventive interventions, clinical workflows, wearable data, and population health analytics.

**Core Workflow:**

`Screen → Understand → Assess Risk → Predict → Intervene → Monitor → Escalate → Measure`

## 🚀 Getting Started

### Prerequisites
- Python
- pip
- Git

### Installation

```bash
# Clone the repository
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd sevahealth-ai

# Install dependencies
pip install -e ".[dev]"

# Seed synthetic demo data
python scripts/seed_data.py

# Start the development server
python -m uvicorn services.api.main:app --reload --port 8000
```

### Access the Application

- **Web Portal:** http://localhost:8000/
- **API Documentation:** http://localhost:8000/docs
- **Health Check:** http://localhost:8000/health

*Note: These commands assume the project dependencies and local configuration are set up correctly.*

## 🧪 Testing

```bash
# Run automated tests
pytest tests -v

# Run end-to-end verification
python scripts/test_e2e.py
```

## 🔐 Clinical Safety

SevaHealth AI is designed as a **clinical decision-support platform, not a diagnostic system**.

- Risk estimates do not represent confirmed diagnoses.
- AI supports preventive guidance and clinical documentation.
- Medication prescribing and autonomous medical decisions are outside the intended scope.
- Escalated cases require review by qualified healthcare professionals.

## 📂 Project Structure

```text
sevahealth-ai/
├── apps/             # Citizen, clinician and public health interfaces
├── services/         # API, screening, risk and clinical services
├── packages/         # Shared schemas, validation and utilities
├── infrastructure/   # Docker, database and monitoring
├── ml/               # Data processing and ML pipelines
├── agents/            # Specialized AI agents
├── docs/              # Documentation and reuse analysis
├── scripts/           # Seeding and verification scripts
└── tests/             # Automated tests
```

## 📜 Open-Source Attribution

Third-party repositories, licenses, and reuse details are documented in [`docs/REUSE_MATRIX.md`](docs/REUSE_MATRIX.md) and [`docs/repository-reuse-analysis.md`](docs/repository-reuse-analysis.md).

## ⚠️ Disclaimer

This project is intended for preventive health support, education, and demonstration. It is not a substitute for professional medical advice, diagnosis, or treatment. Use synthetic data for demonstrations and protect all sensitive health information.

---

**Project:** SevaHealth AI  
**Focus:** Preventive Healthcare • AI-Assisted Risk Assessment • NCD Early Warning • Clinical Decision Support
