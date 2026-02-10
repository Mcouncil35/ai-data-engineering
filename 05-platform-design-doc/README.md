# 05 — Industrial Data Platform Design Doc

**Project 4** | Month 6 | Semester 2

## Objective

Produce a professional architecture design document for an industrial data platform built on MySQL.

## Deliverables

- [ ] Design document (8–12 pages)
- [ ] MySQL Workbench ER diagrams
- [ ] Decision log (ADR format)
- [ ] Architecture diagram: source → ingestion → processing → OLTP → warehouse/serving
- [ ] OLTP vs. warehouse decision analysis
- [ ] Performance & scaling notes: indexing strategy, partitioning plan
- [ ] Security & access: MySQL user roles, privileges, encryption

## Document Sections

1. **Architecture Diagram** — Data flow from source through all layers
2. **Component Descriptions** — What each component does, why chosen, alternatives considered
3. **Data Contracts** — Schemas, SLAs, ownership for key data interfaces
4. **OLTP vs. Warehouse Decision** — When to query OLTP vs. warehouse tables
5. **Performance & Scaling** — Indexing strategy, partitioning plan, query optimization
6. **Security & Access** — MySQL user roles, privileges, encryption at rest/in transit

## Tech Stack

- MySQL Workbench (ER diagrams)
- draw.io / Excalidraw (architecture diagrams)
- Markdown (documentation)

## Structure

```
diagrams/      # ER diagrams, architecture diagrams
docs/          # Design document, ADR decision log
```

## Course Reference

*Advanced Data Modeling* — Meta (Coursera)
