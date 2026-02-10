# 07 — AI Diagnostics Summarizer

**Project 6** | Month 10 | Semester 3

## Objective

Build an AI-powered summarization system that converts raw diagnostic events into actionable intelligence.

## Deliverables

- [ ] Python module for LLM-based summarization
- [ ] Versioned prompt template
- [ ] Test cases (5+) with evaluation results (expected vs. actual)
- [ ] Docker Compose (MySQL + summarizer)
- [ ] Sample outputs showing structured JSON summaries
- [ ] README with architecture and prompt design decisions

## Method

1. **Input:** Query last 24 hours of events from the MySQL Diagnostics Historian
2. **Processing:** Send event data to an LLM with a structured prompt
3. **Output:** Structured JSON summary — severity assessment, top issues, likely root causes, recommended checks, confidence levels
4. **Storage:** Write summaries back to a `daily_summaries` table in MySQL
5. **Evaluation:** At least 5 test cases with expected vs. actual output comparison

## Tech Stack

- Python 3.10+
- OpenAI API or Anthropic API
- MySQL 8.0+ (via Docker)
- Docker Compose

## Structure

```
src/           # Python summarization module
prompts/       # Versioned prompt templates
tests/         # Test cases + evaluation
sql/
└── init/      # MySQL schema (daily_summaries table)
docker-compose.yml
```

## Running

```bash
docker compose up -d
python src/summarizer.py
```

## Course Reference

*Generative AI with Large Language Models* — DeepLearning.AI & AWS (Coursera)
