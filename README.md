# Hi, I'm Vaishali

Analytics Engineer and AI builder. 12+ years of experience.
Currently at Apple, first analytics hire on the ESCI team,
building production AI systems with Python, dbt, Airflow and Snowflake.

---

## 🤖 AI Projects

### 📊 Analytics AI Toolkit
An AI reasoning suite for experimentation that grades its own output.
Deterministic statistics are computed first, then Claude interprets the
verified numbers, so it never invents a statistic. Four tools, connected by
a shared JSON schema so one investigation flows into the next.

- **A/B Test Interpreter:** z-test with Fisher's exact fallback, Welch's t for
  continuous metrics, SRM detection, Bayesian and Benjamini-Hochberg, and a
  ship or hold verdict
- **Sample Size Calculator:** power analysis, MDE curves, test-duration estimate
- **Root Cause Analysis:** hypothesis matrix, diagnostic SQL, ranked next steps
- **Metric Trade-offs:** second-order effects, guardrails, composite metric

**What sets it apart:** a graded eval and error-analysis loop scores every tool's
output (deterministic checks plus an LLM judge) and gates CI. Model-agnostic across
Claude, OpenAI, DeepSeek, and Gemini with one env var. 73 unit tests, green on every push.

**Stack:** Python · SciPy · Claude API · Streamlit · Plotly · GitHub Actions
👉 [GitHub](https://github.com/vaishalizilpe/analytics-ai-toolkit) · [Live App](https://analytics-ai-toolkit-vz.streamlit.app)

---

### 🔍 Airflow DAG Auditor
An Airflow DAG that audits other Airflow deployments. Reads DAG, run, and task
history through the Airflow 3 REST API and ranks the pipelines most likely to be
causing problems.

**What sets it apart:** it finds the failures nothing else reports. A task that
fails regularly but passes on retry leaves the DAG green, so no dashboard shows
it and no alert fires. The auditor reads archived attempt history and surfaces
those runs specifically. It ships with a seeder that provisions a throwaway
Airflow and generates three weeks of real run history from fixtures with
documented ground truth, so every figure in the report can be checked by hand.

**Stack:** Python · Airflow 3 · REST API · pytest
👉 [GitHub](https://github.com/vaishalizilpe/airflow-dag-auditor)

*v0: flakiness detection working end to end. Runtime drift and orphan detection next.*

---

### 🟠 deLOD: Tableau Calculation Coach
Claude-powered app that generates, explains, and debugs Tableau
calculated fields from plain English. 3 modes. 5 domain schemas.
Includes Tableau Public schema import and CSV field inference.

**Stack:** Python · Claude API · Streamlit · Prompt Engineering
👉 [GitHub](https://github.com/vaishalizilpe/deLOD) · [Live App](https://delodbyvz.streamlit.app)

---

### 🎓 Zero to PhD
Give it a topic and a number of days. Get a structured, day-by-day
learning plan built entirely on free resources at Harvard/MIT quality,
ending with something you actually built. No link dumps, no paywalls.

**Stack:** Claude Code · Markdown
👉 [GitHub](https://github.com/vaishalizilpe/zero-to-phd)

---

### 🎯 AI Career Advisor
Fetches real job postings, extracts in-demand skills via NLP,
calls AI model for personalized career gap analysis across 500+ postings per session.

**Stack:** Python · Claude API · Adzuna API · Streamlit · DuckDB
👉 [GitHub](https://github.com/vaishalizilpe/ai-skills-salary-advisor) · [Live App](https://ai-skills-career-advisor.streamlit.app)

---

### 💬 Text-to-SQL Job Market Chatbot
Ask any question in plain English. AI model converts it to SQL,
runs it against a real database, and explains the answer.

**Stack:** Python · Claude API · DuckDB · Streamlit
👉 [GitHub](https://github.com/vaishalizilpe/text-to-sql-chatbot)

---

### ✅ Finance Metrics Validator
Automates KPI reconciliation with in-memory SQL validation.
CI-gated on every push, so no manual QA is required.

**Stack:** Python · SQL · DuckDB · GitHub Actions
👉 [GitHub](https://github.com/vaishalizilpe/finance-metrics-validator)

---

## Core Strengths
- Data modeling and warehouse design
- dbt transformation architecture
- Metric definition and validation systems
- SQL and Python data quality frameworks
- Claude API skill development and production deployment
- Stakeholder-ready analytics outputs

## Engineering Principles
- Metrics must be reproducible
- Data must be testable
- Pipelines must be observable
- Assumptions must be documented
- Tools must work from the terminal

---

## 🛠️ Stack
**AI:** Claude API · Anthropic SDK · Prompt Engineering · LLM Integration
**Data Engineering:** dbt · Snowflake · GCP · BigQuery · Postgres · DuckDB
**Languages:** Python · SQL
**BI:** Tableau · Streamlit · Alteryx

---

## 📫 Connect
[LinkedIn](https://www.linkedin.com/in/vaishalizilpe)
