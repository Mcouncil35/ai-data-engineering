# AI Data Engineering Syllabus
### Coursera Plus | No DeepLearning.AI Track

---

## TERM 1 — FOUNDATIONS

### 1. AI & Analytics Foundations
**Introduction to Data Analytics**
- **Provider:** IBM
- **Topics:**
  - Data lifecycle
  - Analytics workflows
  - Business framing
  - Data-driven decisions
- *Replaces: AI for Everyone*

---

### 2. Data Management & SQL
**Databases and SQL for Data Science with Python**
- **Provider:** IBM
- **Topics:**
  - SQL (DDL, DML, joins)
  - Python + SQL integration
  - Data modeling basics

> **Alternative (Design-Focused):**
> *Database Design and Basic SQL in PostgreSQL* — University of Michigan
> Deeper focus on ER modeling + normalization.

---

### 3. Programming Foundations
**Python for Everybody Specialization**
- **Provider:** University of Michigan

OR

**Python for Data Science, AI & Development**
- **Provider:** IBM

Both are strong and Coursera Plus included.

---

### TERM 1 PORTFOLIO PROJECT
**Project: Business Analytics Dashboard Database**
- Design and build a normalized relational database (PostgreSQL or SQLite) for a real-world dataset (e.g., e-commerce sales, public health data)
- Write Python scripts to ingest, clean, and query the data using SQL
- Produce a short analytics report with business recommendations based on query results
- **Deliverables:** GitHub repo with SQL schema, Python scripts, ERD diagram, and a written summary report
- **Skills demonstrated:** SQL DDL/DML, Python-SQL integration, data lifecycle, business framing

---
---

## TERM 2 — ANALYSIS & MODELING

### 4. Data Preparation & Exploration
**Applied Data Science with Python Specialization**
- **Provider:** University of Michigan
- **Topics:**
  - pandas
  - Data wrangling
  - Statistics
  - Visualization
  - scikit-learn intro
- *More academic than the IBM single-course option.*

---

### 5. Statistical Modeling / Machine Learning
**Applied Machine Learning in Python**
- **Provider:** University of Michigan
- **Topics:**
  - Regression
  - Classification
  - Clustering
  - Model evaluation
- *Replaces: DeepLearning.AI ML Specialization. More classical ML, very solid.*

---

### 6. Data Visualization & Storytelling

| Option | Course | Provider |
|--------|--------|----------|
| A (Python-Based) | Data Visualization with Python | IBM |
| B (Dashboard Tool) | Data Visualization with Tableau Specialization | UC Davis |

---

### TERM 2 PORTFOLIO PROJECT
**Project: End-to-End ML Analysis with Visual Storytelling**
- Select a public dataset (e.g., Kaggle housing prices, UCI ML repo, or government open data)
- Perform full EDA: cleaning, wrangling, statistical summaries using pandas
- Build and evaluate at least 2 ML models (e.g., regression + classification or clustering)
- Create a polished visualization dashboard (matplotlib/seaborn or Tableau) telling the data story
- **Deliverables:** Jupyter notebook with full analysis, model comparison report, interactive or static dashboard, GitHub repo with README walkthrough
- **Skills demonstrated:** pandas, scikit-learn, model evaluation, data visualization, storytelling

---
---

## TERM 3 — ENGINEERING & DEPLOYMENT

### 7. ETL & Pipelines
**ETL and Data Pipelines with Shell, Airflow & Kafka**
- **Provider:** IBM
- *High ROI for automation roles.*

---

### 8. Cloud Data Engineering
**Data Engineering, Big Data, and Machine Learning on Google Cloud**
- **Provider:** Google Cloud
- **Topics:**
  - BigQuery
  - Dataflow
  - Scalable pipelines
  - Cloud storage

---

### 9. Deployment & MLOps
**Machine Learning in Production on Google Cloud**
- **Provider:** Google Cloud

OR

**Preparing for Google Cloud Professional Data Engineer Exam**
- **Provider:** Google Cloud

- **Focus Areas:**
  - Deployment architecture
  - Monitoring
  - Production systems
  - Model lifecycle

---

### TERM 3 PORTFOLIO PROJECT
**Project: Automated Cloud Data Pipeline with Deployed ML Model**
- Build an ETL pipeline using Apache Airflow that ingests data from an API or file source on a schedule
- Transform and load data into BigQuery (or a cloud data warehouse)
- Train an ML model and deploy it as a prediction endpoint on Google Cloud (Vertex AI or Cloud Functions)
- Add basic monitoring/logging for the pipeline and model predictions
- **Deliverables:** GitHub repo with Airflow DAGs, transformation scripts, deployment config, architecture diagram, and a demo video or write-up showing the pipeline running end-to-end
- **Skills demonstrated:** ETL orchestration, Airflow, BigQuery, cloud deployment, MLOps, production monitoring

---
---

## GENAI LAYER

### 10. Generative AI Foundations
**Introduction to Generative AI**
- **Provider:** Google Cloud
- *Short but foundational.*

> **Stronger Alternative:**
> *Generative AI for Data Analysts* — IBM
> More applied and practical for pipelines.

---

### 11. Prompt Engineering
**ChatGPT Advanced Data Analysis**
- **Provider:** Vanderbilt University
- *More applied, production-oriented.*

---

### GENAI LAYER PORTFOLIO PROJECT
**Project: GenAI-Augmented Data Analysis Tool**
- Build a Python application that uses an LLM API (OpenAI, Google Gemini, or similar) to assist with data analysis tasks
- Implement prompt-engineered workflows: natural language to SQL, automated EDA summaries, report generation
- Integrate into an existing dataset or pipeline from a previous project
- **Deliverables:** GitHub repo with working application, example prompts and outputs, a write-up comparing GenAI-assisted vs. manual analysis workflows
- **Skills demonstrated:** LLM API integration, prompt engineering, practical GenAI application, pipeline augmentation

---
---

## CAPSTONE PORTFOLIO PROJECT
**Project: Full-Stack AI Data Engineering Solution**
- Combine all skills into a single end-to-end project:
  - Ingest real-world data from multiple sources (API + database + files)
  - Build a scheduled ETL pipeline (Airflow) loading into a cloud warehouse
  - Apply ML models for prediction or classification
  - Deploy the model with monitoring
  - Add a GenAI layer (natural language querying or automated reporting)
  - Present results in a dashboard or web interface
- **Deliverables:** GitHub repo, architecture diagram, live demo or recorded walkthrough, portfolio-ready write-up
- **Skills demonstrated:** Everything — SQL, Python, ML, ETL, cloud engineering, MLOps, GenAI, data storytelling

---
---

## FINAL COURSE LIST

| # | Course | Provider |
|---|--------|----------|
| 1 | Introduction to Data Analytics | IBM |
| 2 | Databases and SQL for Data Science with Python | IBM |
| 3 | Python for Everybody | University of Michigan |
| 4 | Applied Data Science with Python | University of Michigan |
| 5 | Applied Machine Learning in Python | University of Michigan |
| 6 | Data Visualization with Python | IBM |
| 7 | ETL and Data Pipelines with Shell, Airflow & Kafka | IBM |
| 8 | Data Engineering, Big Data, and ML on Google Cloud | Google Cloud |
| 9 | Machine Learning in Production on Google Cloud | Google Cloud |
| 10 | Introduction to Generative AI | Google Cloud |
| 11 | Generative AI for Data Analysts | IBM |

---

## PORTFOLIO SUMMARY

| Project | Term | Key Skills |
|---------|------|------------|
| Business Analytics Dashboard Database | Term 1 | SQL, Python, ERD, business analysis |
| End-to-End ML Analysis with Visual Storytelling | Term 2 | pandas, scikit-learn, visualization, EDA |
| Automated Cloud Data Pipeline with Deployed ML Model | Term 3 | Airflow, BigQuery, cloud deploy, MLOps |
| GenAI-Augmented Data Analysis Tool | GenAI Layer | LLM APIs, prompt engineering, automation |
| Full-Stack AI Data Engineering Solution | Capstone | All skills combined |

---

## GRADUATE COMPETENCIES

| Skill | Source |
|-------|--------|
| SQL + schema design | Courses 2, 4 |
| Python automation | Courses 3, 4 |
| Classical ML | Course 5 |
| Cloud data engineering | Course 8 |
| ETL orchestration (Airflow) | Course 7 |
| Production ML architecture | Course 9 |
| GenAI workflow integration | Courses 10, 11 |

---

> **Program Notes:**
> - Mirrors WGU structure
> - Avoids DeepLearning.AI dependency
> - Fully Coursera Plus compatible
> - Industry-aligned for AI Data Engineer roles
> - 5 portfolio projects demonstrating progressive skill building
