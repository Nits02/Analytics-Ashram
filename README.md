
![alt text](./images/challenge.png)


---

# 🚨 CivAI — DRPI-Powered Resilience Intelligence System
### A Smart Disaster Preparedness and Response Platform powered by GenAI & BI — Team: Analytics Ashram

---

## 🔍 Hackathon Overview

This project was developed for the [Databricks Smart Business Insights Challenge](https://hackathon.stackup.dev/web/events/databricks-smart-business-insights-challenge?scid=701Vp00000JlYwNIAV) — a global innovation competition to reimagine data analytics using Databricks Lakehouse, AI/BI dashboards, and modern application building with Databricks Apps.

Participants were tasked with solving one of the following:
- Revenue Forecasting for Retail
- Disaster Recovery Preparedness Index (DRPI)

We chose the second challenge, recognizing its potential societal impact.

---

## 🧠 Problem Statement — DRPI: Disaster Recovery Preparedness Index

Disasters are unpredictable but their impacts don’t have to be. Traditional preparedness assessments are static, fragmented, and reactive. DRPI was proposed as a metric to **quantify readiness and suggest resilience strategies** using a data-driven, AI-enhanced platform.

---

## 💡 Our Solution — Meet CivAI 🌪️

CivAI is an **AI-powered disaster recovery insights assistant** that assesses DRPI scores and provides recommendations through:
- **GenAI insights** using Databricks' MosaicML
- **BI dashboards via Databricks SQL**
- **Smart interactions** via Databricks Genie Spaces
- **Interactive apps** using the Databricks Apps SDK

By combining multiple data sources (infrastructure, healthcare, economic, climate), our system delivers **real-time, explainable, and actionable preparedness intelligence** to communities and emergency planners.

---

## 👨‍👩‍👧‍👦 Team: Analytics Ashram

We are a group of passionate data professionals working at the intersection of **AI, public safety, and data-driven insights**.

- 🧠 **[Your Name]** – AI/ML Lead
- 📊 **[Your Name]** – BI Engineer
- 🏗 **[Your Name]** – Solutions Architect

> We believe that *data can save lives* — when it's accessible, explainable, and intelligent.

---

## 📈 System Architecture

![DRPI CivAI Architecture](images/DRPI_System_Component_Diagram.jpg)

### Key Components:
- **Data Ingestion**: Structured/unstructured from infra, climate, health.
- **Feature Engineering**: Index scoring across domains.
- **DRPI Index Calculation**: AI model pipelines via Databricks Notebooks.
- **Insights Generation**: MosaicML + GPT-4 via MLFlow for contextual GenAI output.
- **Visualization**: BI dashboards on Databricks SQL & Genie Spaces.
- **Deployment**: Through Databricks Apps for UI integration.

---

## 🧠 Why Databricks?

| Tool/Feature        | Justification |
|---------------------|---------------|
| **MosaicML**        | For scalable fine-tuning of GenAI models with DRPI context. |
| **Databricks SQL**  | For building fast, intuitive DRPI dashboards for stakeholders. |
| **Genie Spaces**    | Enables interactive chatbot-like UX with context persistence. |
| **Databricks Apps** | Seamless deployment of complete UX on top of Lakehouse infra. |

---

## ✨ Key Features

- 🧠 **OrcivAI Chatbot (GenAI Assistant)**: Conversational assistant that explains DRPI, interprets dashboards, and recommends actions.
- 📊 **Smart BI Dashboard**: Tracks DRPI at state/city level with drill-down capabilities.
- 🧰 **Custom DRPI Calculator**: Upload regional datasets, get preparedness scores instantly.
- 🧠 **Action Intelligence Panel**: Policy and investment recommendations using AI.
- 🏛 **Databricks App UI**: Integrated front-end built with the Databricks App SDK.

---

## 🔄 Architecture Decision Records (ADRs)

We made several critical design decisions documented in our ADRs:

1. **ADR-001**: Chose DRPI use case over revenue due to social impact potential.
2. **ADR-002**: Adopted AI/BI over traditional rule-based index calculation for scalability and explainability.
3. **ADR-003**: Selected Genie Spaces for chat-style UX and persistent context retrieval.
4. **ADR-004**: Used Databricks Apps for seamless deployment and secure data interaction.
5. **ADR-005**: Chose MosaicML for rapid experimentation and fine-tuning of GPT-based insights.
6. **ADR-006**: Leveraged Databricks SQL for live dashboards that update with pipeline refresh.

> Read more: [`docs/adrs/`](./docs/adrs/)

---

## 🚀 Impact & Outcomes

| Category | Outcome |
|----------|---------|
| Preparedness Awareness | DRPI democratized for policymakers, NGOs, and citizens. |
| Explainability | GenAI insights help interpret scores & recommend next steps. |
| Interactivity | Users engage through dashboard or chatbot. |
| Deployability | End-to-end app hosted within the Databricks ecosystem. |

---

## 🛠️ Tech Stack

| Layer               | Stack |
|--------------------|-------|
| Data Ingestion     | Delta Lake, Auto Loader |
| AI Models          | GPT-4, MosaicML, MLflow |
| BI Layer           | Databricks SQL, Genie Spaces |
| UX Deployment      | Databricks Apps SDK |
| Collaboration      | Notebooks, Spaces, Lakehouse integration |

---

## 📺 Demo

> 🎥 Coming Soon: Watch our walkthrough video here  
> _(To be uploaded before final submission)_

---

## 🤝 Contribute & Collaborate

We’d love your feedback or collaboration! Feel free to fork the repo, raise issues, or connect on LinkedIn.

---

📫 **Contact**: [team.analytics.ashram@example.com](mailto:team.analytics.ashram@example.com)  
💡 Let's make our cities smarter and safer.

---

<sub>Built with ❤️ and Databricks by Team Analytics Ashram — May 2025</sub>
