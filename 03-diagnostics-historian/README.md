# 03 — Diagnostics Historian

**Project 2** | Month 3 | Semester 1

## Objective

Design and populate a MySQL database for industrial equipment diagnostics.

## Deliverables

- [ ] MySQL schema with tables: `machines`, `devices`, `ports`, `events`
- [ ] Proper foreign key relationships and indexing
- [ ] Sample data: minimum 500 event records across 10+ devices
- [ ] Python data loading script via `mysql-connector-python`
- [ ] Analytical queries: top 10 faults, downtime by device, worst ports, daily event trend, reporting gaps
- [ ] Docker Compose file for MySQL
- [ ] README with schema diagram and sample results

## Tech Stack

- MySQL 8.0+ (via Docker)
- Python 3.10+ (mysql-connector-python)
- Docker Compose
- VS Code + MySQL extension

## Structure

```
sql/
├── init/       # DDL schema files — auto-runs on docker compose up
└── queries/    # Analytical query files with comments
src/            # Python data loading scripts
tests/          # pytest test suite
docker-compose.yml
```

## Running

```bash
# Start MySQL
docker compose up -d

# Load sample data
python src/load_data.py

# Run queries
mysql -h 127.0.0.1 -P 3306 -u root -p < sql/queries/analytics.sql
```

## Course Reference

*Database Structures and Management with MySQL* — Meta (Coursera)
