# 🧭 Problem Statement

## 🌍 Business Context

In an era marked by increasing climate volatility and urban density, cities like **Singapore** are highly vulnerable to the compounded effects of **natural disasters** such as extreme heatwaves, flash floods, thunderstorms, and haze episodes. These events pose direct threats to **human safety, public health, and community resilience**, especially for **vulnerable populations** including the elderly, low-income residents, and those living in poorly ventilated or exposed housing.

Despite Singapore's advanced infrastructure and open data availability, **decision-makers lack a dynamic, AI-driven tool that provides predictive, real-time insights** into disaster risks and emergency preparedness. This gap limits proactive planning, equitable resource allocation, and hyperlocal emergency responses.

---

## 🔧 Technical Problem

Current datasets—although rich and varied—remain siloed across weather services, government health sources, and urban planning repositories. There is **no unified framework** that fuses this heterogeneous data to compute **actionable, localized disaster risk indices**. Moreover, while Singapore provides APIs and open datasets through [data.gov.sg](https://data.gov.sg), these are underutilized in combination with external sources like **AccuWeather** or **PredictHQ** for AI modeling and visual analytics.

### Key Challenges:
- Lack of **real-time, geospatial AI-driven analytics** for natural disaster vulnerability.
- Absence of **integrated SDOH (Social Determinants of Health) indicators** to assess population sensitivity.
- Need for **dynamic, conversational insights** and visualizations using Databricks-native AI/BI capabilities.
- Requirement for **low-latency dashboards** that can support both operational and policy-level decision-making.

---

## 🧠 Our Social Impact Use Case

We address this challenge by building a **Disaster Risk & Preparedness Index (DRPI)** for Singapore—a composite score derived from:
- Real-time weather anomaly signals (AccuWeather, PredictHQ),
- Public housing and socio-economic vulnerability data (HDB/OneMap/SHI models),
- Environmental, mobility, and infrastructure readiness indicators.

The DRPI is visualized through:
- **AI-powered BI dashboards** in Databricks using Delta Lake,
- **Genie Spaces** for conversational exploration,
- **Databricks Apps** to embed insights directly into emergency management workflows.

---

## 🎯 Why It Matters

By creating a **multi-source, AI-enhanced DRPI platform**, we empower:
- **Government agencies** to pre-emptively allocate emergency resources,
- **NGOs and responders** to prioritize outreach in high-risk zones,
- **Citizens** to access localized risk alerts and preparedness suggestions.

Ultimately, this solution advances **climate resilience**, **public health equity**, and **data-driven governance**—delivering on the social impact mission of this hackathon.

---
