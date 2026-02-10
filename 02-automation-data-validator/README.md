# 02 — Automation Data Validator

**Project 1** | Month 2 | Semester 1

## Objective

Build a production-style data validation tool for industrial device events.

## Deliverables

- [ ] Working Python script/module for data validation
- [ ] Sample input data (100+ records, some malformed)
- [ ] Sample output: clean dataset + error log + summary report
- [ ] Dockerfile for containerized execution
- [ ] Automated test suite (pytest) with min 70% coverage
- [ ] README in lab report format

## Method

1. **Read** CSV and JSON input files containing device event records
2. **Validate** against a defined schema (required fields, data types)
3. **Check** value ranges (e.g., temperature within bounds, timestamp not in future)
4. **Log** all validation errors with row number, field, and reason
5. **Output** clean dataset (passing records) + summary report (total records, pass/fail counts, error breakdown)

## Tech Stack

- Python 3.10+ (Pandas, csv, json)
- pytest
- Docker
- VS Code

## Structure

```
src/           # Validation modules
tests/         # pytest test suite
data/
├── input/     # Raw CSV/JSON input files
└── output/    # Clean datasets + error logs + summaries
Dockerfile     # Containerized execution
```

## Running

```bash
# Local
python src/validator.py --input data/input/ --output data/output/

# Docker
docker build -t data-validator .
docker run -v $(pwd)/data:/app/data data-validator
```

## Course Reference

*Python and Pandas for Data Engineering* — Duke University (Coursera)
