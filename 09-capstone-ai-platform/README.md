# 09 — Capstone: AI Automation Data Platform

**Capstone Project** | Month 12 | Semester 3

## Objective

Integrate all program components into a single, end-to-end AI automation platform that demonstrates production-grade engineering practices. The entire platform runs via `docker compose up`.

## Deliverables

- [ ] Complete GitHub repository with all components
- [ ] Single `docker-compose.yml` spinning up the entire platform
- [ ] Architecture diagram (draw.io or MySQL Workbench)
- [ ] Runbook document
- [ ] 5-minute presentation: problem statement, architecture walkthrough, demo, key decisions, retrospective

## Components

| # | Component | Description |
|---|-----------|-------------|
| 1 | **Airflow Pipeline** | Ingests, validates, transforms, loads data into MySQL on daily schedule |
| 2 | **MySQL Historian** | Full schema: machines, devices, ports, events, time-series, severities. Star schema warehouse tables |
| 3 | **AI Summarizer Service** | Dockerized FastAPI + LangChain — queries events, generates JSON summaries via LLM |
| 4 | **Data Quality Tests** | Schema validation, referential integrity checks, volume anomaly detection |
| 5 | **Prompt & Version Tracking** | Prompt versions stored in MySQL, each summary linked to prompt version |
| 6 | **Drift Monitoring** | Track fault volume over time, alert on distribution shifts |
| 7 | **Runbook** | Documentation for pipeline failures, AI failures, data quality failures |

## Tech Stack

- Apache Airflow (orchestration)
- MySQL 8.0+ (data store)
- FastAPI + LangChain (AI summarizer)
- Docker Compose (infrastructure)
- Python 3.10+

## Architecture

```
Raw Data (CSV/JSON/API)
      |
      v
[Airflow Pipeline] ---> Validate ---> Transform ---> Load
      |                                                |
      v                                                v
[Pipeline Logs]                              [MySQL Historian]
                                                       |
                                          +------------+------------+
                                          |                         |
                                          v                         v
                               [FastAPI Summarizer]        [MySQL Warehouse]
                                          |                         |
                                          v                         v
                               [daily_summaries]          [Analytics Queries]
                                          |
                                          v
                               [Monitoring & Alerts]
```

## Structure

```
airflow/
└── dags/              # Airflow DAG definitions
summarizer-api/
└── src/               # FastAPI + LangChain application
monitoring/            # Drift detection scripts
sql/
└── init/              # Full MySQL schema initialization
docs/
├── architecture/      # Architecture diagrams
└── runbook/           # Operational runbook
docker-compose.yml     # Full platform: MySQL + Airflow + FastAPI + monitoring
```

## Running

```bash
docker compose up -d
# Airflow UI:      http://localhost:8080
# Summarizer API:  http://localhost:8000
```

## Course Reference

*Machine Learning Engineering for Production (MLOps)* — DeepLearning.AI (Coursera)
