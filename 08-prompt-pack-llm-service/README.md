# 08 — Prompt Pack + Dockerized LLM Service

**Portfolio Upgrade** | Month 11 | Semester 3

## Objective

Create a professional prompt engineering artifact and containerized LLM service.

## Deliverables

- [ ] Versioned prompts (3+ versions with changelogs) managed via LangChain templates
- [ ] Evaluation rubric: accuracy, completeness, format compliance, actionability
- [ ] Test cases (10+): 5 golden inputs, 3 edge cases, 2 adversarial inputs
- [ ] Prompt contract: input/output JSON schemas, constraints, failure behavior
- [ ] Dockerized FastAPI + LangChain service (reads from MySQL, returns structured JSON)
- [ ] Evaluation results table: each prompt version scored across test cases

## Tech Stack

- Python 3.10+
- FastAPI + uvicorn
- LangChain
- MySQL 8.0+ (via Docker)
- Docker + Docker Compose

## Structure

```
src/               # FastAPI application + LangChain chains
prompts/
└── versions/      # Versioned prompt templates + changelogs
tests/             # Test cases (golden, edge, adversarial)
evaluation/        # Evaluation scripts + results
Dockerfile         # FastAPI + LangChain container
docker-compose.yml # MySQL + FastAPI service
```

## Running

```bash
# Start full stack
docker compose up -d

# Test the API
curl http://localhost:8000/summarize -X POST -H "Content-Type: application/json" -d '{"hours": 24}'
```

## Course Reference

*Building LLMs with Hugging Face and LangChain* — Edureka (Coursera)
