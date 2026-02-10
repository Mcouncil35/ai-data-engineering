# 06 — Industrial Event Processor

**Project 5** | Month 7 | Semester 2

## Objective

Build an industrial data processing system that derives operational intelligence from raw device events.

## Deliverables

- [ ] Extended MySQL schema with process value tables + migration scripts
- [ ] Event severity classification model with configurable rules
- [ ] Device metadata enrichment pipeline
- [ ] Anomaly flagging: spike-in-fault-frequency detection via rolling window analysis
- [ ] Operational metrics: MTBF proxy per device, rolling fault rate, "worst performers" ranking
- [ ] Docker Compose (MySQL + Python processor)
- [ ] README with data model diagram

## Method

1. **Time-Series Support:** Extend Historian schema with process value tables
2. **Event Severity Model:** Classify events into severity tiers with configurable rules
3. **Device Metadata Enrichment:** Join event data with device metadata
4. **Anomaly Flagging:** Detect spikes in fault frequency using rolling window analysis
5. **Operational Metrics:** MTBF proxy, rolling fault rate, worst performers ranking

## Tech Stack

- MySQL 8.0+ (via Docker)
- Python 3.10+ (mysql-connector-python, Pandas)
- Docker Compose

## Structure

```
sql/
├── migrations/   # Schema migration scripts
└── queries/      # Analytical + metric queries
src/              # Python processing modules
tests/            # pytest test suite
docker-compose.yml
```

## Running

```bash
docker compose up -d
python src/processor.py
```

## Course Reference

Applied integration month — no new course
