# Wania Maqsood

Software Engineering graduate focused on **backend engineering and AI-powered applications**. I build practical APIs and data pipelines in Python: databases, containers, validation, and workflows where an LLM is one component rather than the whole product.

> My portfolio proves that I can build AI-powered backend applications that solve practical problems.

**Looking for:** Junior Backend Engineer · Junior Python Developer · Entry-Level AI Engineer · AI Backend Engineer
**Contact:** `waniamaqsoood@gmail.com`

## Featured projects (FlyRank Backend Engineering Internship)

### [Social Media Studio](https://github.com/waniamaqsood/socialMediaStudio): capstone
Turns one blog post into LinkedIn and Instagram drafts using a local LLM (Ollama), requires human approval, and publishes through swappable adapters (a real Discord webhook plus mock LinkedIn and X).
- FastAPI + SQLite, with a draft → approved/rejected → published workflow and 409 state checks
- Generation validated against platform length and hashtag limits, with retry and error feedback
- A separate worker publishes due schedules and returns interrupted jobs to the queue after a restart
- Idempotency keys stop repeated publish calls from re-sending a schedule slot; the README documents exactly where duplicates are still possible (concurrency, ambiguous timeouts)

### [Task API (FastAPI + PostgreSQL + Docker)](https://github.com/waniamaqsood/flyRankAssignments)
One REST API built three ways (in-memory → SQLite → PostgreSQL), ending in a Docker Compose stack.
- Parameterized SQL, seed-once initialization, named volume for persistence
- The commit history shows each stage: in-memory, then SQLite, then PostgreSQL in Docker

### [Polite Scraper (data-ingestion pipeline)](https://github.com/waniamaqsood/politeScraper)
A polite scraper structured as a data-ingestion job: identifying User-Agent, delay and timeout, HTML cache, pagination, Pydantic validation, retry-once rules, JSON output and a run report.

### [FastAPI + Supabase Auth](https://github.com/waniamaqsood/authenticationPractice): supporting project
Bearer-token protected routes with sign-up and login delegated to Supabase Auth, documented with Swagger/OpenAPI.

## Skills shown in these projects

**Languages & frameworks:** Python, FastAPI, Pydantic, SQL
**Data:** PostgreSQL, SQLite, psycopg, parameterized queries
**Infrastructure:** Docker, Docker Compose, environment-based configuration
**AI:** Local LLM integration (Ollama), output validation with retry
**Practices:** REST design, idempotency checks, approval workflows, adapter pattern, pytest

## How I document my work

Each project README states what it does, how to run it, how it was tested, and what it does **not** do. Limitations are listed on purpose; I would rather show an accurate picture than a flattering one.
