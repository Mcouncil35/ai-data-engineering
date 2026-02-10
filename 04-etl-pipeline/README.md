# 04 — Automated ETL Pipeline

**Project 3** | Month 5 | Semester 2

## Objective

Build a fully orchestrated ETL pipeline using Apache Airflow that runs daily and produces auditable outputs.

## Deliverables

- [ ] Airflow DAG file(s) for the ETL pipeline
- [ ] Supporting Python modules (extract, validate, transform, load)
- [ ] Docker Compose setup (Airflow + MySQL)
- [ ] Sample pipeline run output
- [ ] README with architecture diagram

## Method

1. **Extract:** Ingest raw data from file source (CSV/JSON, simulating upstream system)
2. **Validate:** Schema + range checks (reuse/extend Project 1 logic)
3. **Transform:** Clean, deduplicate, derive new fields (e.g., event severity classification)
4. **Load:** Insert into MySQL target tables via `mysql-connector-python`
5. **Report:** Generate daily summary table + data quality report
6. **Operational:** Retry logic (3 attempts, exponential backoff), failure notifications, pipeline run log

## Tech Stack

- Apache Airflow (via Docker)
- MySQL 8.0+ (via Docker)
- Python 3.10+
- Docker Compose

## Structure

```
dags/          # Airflow DAG definitions
src/           # Python ETL modules
tests/         # pytest test suite
sql/
└── init/      # MySQL schema initialization
docker-compose.yml    # Airflow + MySQL
```

## Running

```bash
# Start Airflow + MySQL
docker compose up -d

# Access Airflow UI
open http://localhost:8080
```

## Course Reference

*ETL and Data Pipelines with Shell, Airflow and Kafka* — IBM (Coursera)
