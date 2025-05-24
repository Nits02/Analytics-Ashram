# 🧠 Architecture Decision Records (ADR) – DRPI System

This document captures key architectural decisions made during the design and implementation of the **Disaster Risk & Preparedness Index (DRPI)** solution.

---

## ADR-0001: Choose Databricks as Core Platform

**Status**: Accepted  
**Date**: 2024-04-01

### Context
The DRPI system requires scalable ingestion, real-time computation, Delta Lake storage, and an analytics interface for data scientists and public health experts.

### Options Considered
1. AWS Glue + S3 + Athena + CloudWatch
2. Azure Synapse + Blob Storage + Power BI
3. GCP BigQuery + Dataflow + Looker
4. **Databricks (Delta Lake + DBR + Unity Catalog)** ✅

### Decision
We selected **Databricks** as the core platform to host ingestion jobs, Spark pipelines, storage layers (Bronze/Silver/Gold), and advanced analytics.

### Rationale
- Native **Delta Lake** support for versioning and ACID transactions
- **Unified workspace** for notebooks, jobs, SQL, ML & dashboards
- Strong governance via **Unity Catalog**
- Seamless integration with **BI tools**, alerting, and APIs

---

## ADR-0002: Use Genie Spaces for Collaboration and Reusability

**Status**: Accepted  
**Date**: 2024-04-05

### Context
Our system includes multiple roles: engineers, data scientists, and public health analysts. We need a shared space for models, dashboards, pipelines, and notebooks.

### Options Considered
1. GitHub Wiki + CI/CD
2. Custom MLFlow environment
3. **Databricks Genie Spaces** ✅

### Decision
We chose **Genie Spaces** to organize, share, and govern collaborative DRPI assets in a governed workspace.

### Rationale
- Shared **team-based view** of all notebooks, dashboards, pipelines
- Easy discovery, publishing, and versioning of analytics
- Tight integration with Unity Catalog and data lineage

---

## ADR-0003: Adopt Unified AI/BI Dashboard Approach

**Status**: Accepted  
**Date**: 2024-04-07

### Context
The DRPI platform must communicate real-time disaster risk to both technical and non-technical users via intuitive dashboards.

### Options Considered
1. Power BI or Tableau via external connections
2. Custom frontend using React + D3.js
3. **Databricks Unified Dashboard (SQL, BI, Python, ML)** ✅

### Decision
We selected **Databricks Unified Dashboard** for visualizing DRPI scores, public health indicators, and alerts.

### Rationale
- Built-in support for **SQL, Python, and ML outputs**
- One-click publishing of **Dashboards inside Databricks**
- Real-time **integration with Delta tables**
- Reduces maintenance overhead of managing a separate frontend

---

## ADR-0004: Implement Alerts via Databricks Apps & Workflows

**Status**: Accepted  
**Date**: 2024-04-10

### Context
We need to automatically alert government responders or analysts when DRPI scores exceed thresholds.

### Options Considered
1. Cron + Lambda + SES (AWS)
2. External Airflow DAGs with SMTP
3. **Databricks Workflows + Apps for Alerting** ✅

### Decision
We chose **Databricks Jobs + Alerting Apps** to automate and deliver alerts to end-users via email/SMS.

### Rationale
- Fully managed inside the Databricks ecosystem
- Use of `email`, `webhook`, or `Slack` alerts in workflow steps
- Scales seamlessly with the DRPI computation engine

---

## ADR-0005: Organize ETL Using Multi-Layer Delta Architecture

**Status**: Accepted  
**Date**: 2024-04-15

### Context
Ingested data varies in structure and quality, including weather APIs, event feeds, and demographics data. A layered storage architecture is critical for reliability and traceability.

### Options Considered
1. Use S3 buckets with manual versioning
2. Single Lakehouse with no separation
3. **Delta Lake with Bronze, Silver, and Gold layers** ✅

### Decision
We adopted the **Bronze → Silver → Gold** Delta Lake approach.

### Rationale
- Enables **audit logs and time travel** at each stage
- Simplifies debugging and reruns of failed jobs
- Gold layer optimized for **consumption (BI/API)**

---

## ADR-0006: Design DRPI Score as Weighted Composite (Hazard + SDOH)

**Status**: Accepted  
**Date**: 2024-04-18

### Context
We needed a flexible, explainable risk scoring mechanism that blends external hazard signals with internal vulnerability data.

### Options Considered
1. Pure ML-based black-box risk model
2. Rule-based threshold scoring
3. **Hybrid weighted scoring: DRPI = w1 * Hazard + w2 * SDOH** ✅

### Decision
We implemented a **hybrid scoring model** with tunable weights and optional ML enhancements.

### Rationale
- Human-readable and explainable
- Easy to debug and tune
- Allows ML overlay for smarter adaptive scoring

---

