# Michel Cano

**Senior Backend Developer at XalDigital**

5 years building production backend systems. Currently working on healthcare sector solutions. Two libraries published on PyPI. 600+ automated tests across projects.

Based in Mexico City.

---

### Currently

Senior Backend Developer at **XalDigital** (AWS Premier Partner) — building backend solutions to unify and integrate clinical and administrative systems for healthcare clients. Python, Django, PostgreSQL, Docker.

---

### Open Source (PyPI)

**[legismex](https://github.com/lehcimhdz/legismex)** — Python library for Mexico's legislative data. 67 modules covering Congress, Senate, DOF, and 25+ state legislatures. httpx, Pydantic, Playwright. CI/CD with daily automated health monitor. `pip install legismex`

**[open-data-mexico](https://github.com/lehcimhdz/open-data-mexico-api)** — Async Python client for datos.gob.mx (CKAN). 28 categories, 5,000+ datasets. httpx async, Pydantic v2, TTL cache. Includes optional FastAPI server. `pip install open-data-mexico`

---

### Backend Projects

**[mex-open-data-backend-fastapi](https://github.com/lehcimhdz/mex-open-data-backend-fastapi)** — REST API with FastAPI, SQLAlchemy, Alembic, API key auth (SHA-256), Celery, Redis, Prometheus metrics, health/liveness/readiness probes. Docker multi-stage. 26 tests.

**[data-cdmx-backend-django](https://github.com/lehcimhdz/data-cdmx-backend-django)** — Django REST backend with 7 apps, 11 models, Celery + Beat, health check, Swagger docs. 105 tests.

**[DiplomaticU](https://github.com/lehcimhdz/diplomaticU)** — Full-stack EdTech: React 19, TypeScript, Supabase. 14 pages, 19 components, 10-table schema, auth, gamification.

---

### Production Systems

**Victim Registry System** *(private)* — Django REST API, PostgreSQL with field-level encryption, Celery + Redis (3 priority queues), automated document generation (ODT → PDF), Google APIs with OAuth2. Docker Compose (5 services), Cloudflare Tunnel. 500+ cases/year, 95% time reduction.

**Pipeline Registro** *(private)* — 9 Airflow DAGs for operational observability: data cleaning, integrity checks, Celery error audit, DB maintenance. Running on Ubuntu Server 24/7.

**OpenClaw AI Agent** — AI agent on Ubuntu Server + Telegram for natural language database querying.

---

### Data Engineering

**[global-trade-aws](https://github.com/lehcimhdz/global-trade-aws)** — 8 Airflow DAGs, UN Comtrade API, medallion architecture, dbt, data quality validation, Slack + SLA alerting. Terraform IaC. 433 tests.

**[mex-open-data ecosystem](https://github.com/lehcimhdz/mex-open-data-pipeline)** — 5 repos: Airflow pipeline → S3 data lake → FastAPI backend + PySpark analytics → Athena. Terraform modularized (5 modules). 170+ tests.

**[cdmx-api-pipeline](https://github.com/lehcimhdz/cdmx-api-pipeline)** — 7 Airflow DAGs for CDMX open data (2.4M transit records, 808K investigation files). Terraform (VPC, EC2, RDS, ElastiCache). Sentry + Slack. 95 tests.

**[pipeline-legismex-aws](https://github.com/lehcimhdz/pipeline-legismex-aws)** — 8 Airflow DAGs, 20+ states, medallion architecture. Terraform (RDS, security groups, automated backups).

---

### Other

**[Homo Politicus](https://github.com/lehcimhdz/homo-politicus)** — Political & economic simulator in C++. Cobb-Douglas GDP, dynamic labor markets, sovereign debt. 2,150 LOC.

---

### Tech

**Backend:** Python, Django REST Framework, FastAPI, SQLAlchemy, Alembic, Celery, Redis, Pydantic, PostgreSQL

**Data:** Apache Airflow, PySpark, dbt, pandas, Parquet, boto3

**Cloud:** AWS (S3, RDS, EC2, ElastiCache, Secrets Manager, Glue, Athena, CloudWatch), Terraform (modularized)

**Frontend:** React 19, TypeScript, Tailwind CSS, Supabase

**Ops:** Docker, Nginx, Cloudflare Tunnel, GitHub Actions CI/CD, Sentry, Prometheus

**Testing:** pytest (600+ tests), moto, unittest.mock

---

### Background

B.A. International Relations — UNAM (2019) · B.S. Mathematics — UnADM (in progress) · Data Engineer Associate — DataCamp (2026)
