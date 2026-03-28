# Michel Cano

** Python Developer & Data Engineer**

4+ years building production systems, data pipelines, and open-source tools. Two libraries published on PyPI. 600+ automated tests across projects. Terraform on AWS. PySpark. FastAPI. Django. Airflow.

Based in Mexico City.

---

### Open Source (PyPI)

**[legismex](https://github.com/lehcimhdz/legismex)** — Python library for Mexico's legislative data. 67 modules covering Congress, Senate, DOF, and 25+ state legislatures. httpx, Pydantic, Playwright, async. CI/CD with daily automated health monitor. `pip install legismex`

**[open-data-mexico](https://github.com/lehcimhdz/open-data-mexico-api)** — Async Python client for datos.gob.mx (CKAN). 28 categories, 5,000+ datasets. httpx async, Pydantic v2, in-memory TTL cache. Includes optional FastAPI server. `pip install open-data-mexico`

---

### Data Platform — Mexican Open Data Ecosystem

Five interconnected repos that extract, store, transform, and serve Mexico's federal open data:

| Repo | Stack | What it does |
|------|-------|-------------|
| [mex-open-data-pipeline](https://github.com/lehcimhdz/mex-open-data-pipeline) | Airflow 2.9, CeleryExecutor | 3 DAGs: catalog sync, dataset ingestion (smart skip), PostgreSQL upsert. Slack alerts, SLA monitoring |
| [mex-open-data-backend-fastapi](https://github.com/lehcimhdz/mex-open-data-backend-fastapi) | FastAPI, SQLAlchemy, Alembic, Celery, Redis | REST API with auth, Prometheus metrics, health/liveness/readiness probes |
| [mex-open-data-aws-s3](https://github.com/lehcimhdz/mex-open-data-aws-s3) | Terraform (modularized) | S3 data lake, IAM, Glue, Athena, CloudWatch, SNS, CloudTrail. 5 modules |
| [mex-open-data-spark](https://github.com/lehcimhdz/mex-open-data-spark) | PySpark | Transform, normalize, aggregate, data quality reports, Glue catalog registration |

```
datos.gob.mx → open-data-mexico (PyPI) → Airflow pipeline → S3 data lake
                                                 ↓                ↓
                                            PostgreSQL        PySpark
                                                 ↓                ↓
                                          FastAPI REST API    Athena (SQL)
```

---

### Data Pipelines

**[global-trade-aws](https://github.com/lehcimhdz/global-trade-aws)** — Production-grade pipeline extracting international trade data from all 8 UN Comtrade API endpoints. Airflow with CeleryExecutor, medallion architecture (Bronze/Silver/Gold), dbt, 7-check data quality validation, Slack alerting, SLA monitoring. Terraform IaC (S3, IAM, Secrets Manager, VPC, Glue, Athena, ECR, CloudWatch, MWAA). **433 tests.** Docker Compose. Pre-commit hooks. Makefile.

**[pipeline-legismex-aws](https://github.com/lehcimhdz/pipeline-legismex-aws)** — ETL pipeline using legismex as data source. 8 Airflow DAGs covering 20+ Mexican states with TaskGroups. Medallion architecture: Bronze NDJSON → Silver Parquet → Gold canonical schema. Terraform (RDS, security groups, automated backups).

**[cdmx-api-pipeline](https://github.com/lehcimhdz/cdmx-api-pipeline)** — Airflow pipeline extracting CDMX open data (CKAN): transit ridership (2.4M records), FGJ investigation files (808K), flood risk, Ecobici. Terraform (VPC, EC2, RDS, ElastiCache, Secrets Manager). Sentry + Slack. 95 tests.

---

### Production Systems

**Victim Registry System** *(private repo)* — Full system serving 500+ cases/year for the Mexico City Victims' Commission. Django REST API, PostgreSQL with field-level encryption, Celery + Redis (3 priority queues, exponential backoff), automated document generation (ODT → PDF via Jinja2 + LibreOffice), Google APIs (Drive, Sheets, Gmail) with OAuth2. Docker Compose (5 services), Cloudflare Tunnel, automated backups. Reduced processing time by 95%.

**Pipeline Registro** *(private repo)* — 9 Airflow DAGs for operational observability of the victim registry database: data cleaning (CURP/RFC/email/phone normalization), integrity checks, Celery error audit, performance monitoring, DB maintenance (ANALYZE + index optimization). Running on Ubuntu Server 24/7.

**OpenClaw AI Agent** — AI agent deployed on Ubuntu Server connected to Telegram, enabling natural language querying of the victim registry database by non-technical managers.

---

### Other Projects

**[DiplomaticU](https://github.com/lehcimhdz/diplomaticU)** — Full-stack EdTech: React 19, TypeScript, Supabase. 14 pages, 19 components, 10-table schema, auth, gamification.

**[Homo Politicus](https://github.com/lehcimhdz/homo-politicus)** — Political & economic strategy simulator in C++. Cobb-Douglas GDP, dynamic labor markets, sovereign debt, 5 interconnected systems. 2,150 LOC.

---

### Tech

**Languages:** Python, SQL, TypeScript, JavaScript, C++

**Backend:** Django REST Framework, FastAPI, SQLAlchemy, Alembic, Celery, Redis, Pydantic

**Data:** Apache Airflow, PySpark, dbt, pandas, Parquet, boto3, data quality validation

**Cloud:** AWS (S3, RDS, EC2, ElastiCache, Secrets Manager, IAM, Glue, Athena, CloudWatch, MWAA), Terraform (modularized)

**Frontend:** React 19, TypeScript, Tailwind CSS, Supabase

**Ops:** Docker, Nginx, Cloudflare Tunnel, GitHub Actions CI/CD, Sentry, Prometheus, pre-commit

**Testing:** pytest (600+ tests across projects), moto, unittest.mock, DAG integrity tests

---

### Background

B.A. International Relations — UNAM (2019) · B.S. Mathematics — UnADM (in progress) · Data Engineer Associate — DataCamp (2026)

---

📫 bmichelcano@gmail.com

<br>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=lehcimhdz&theme=dark&hide_border=true" alt="GitHub Streak" height="195" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=lehcimhdz&layout=compact&theme=dark&hide_border=true" alt="Top Lenguajes" height="195" />
</div>
