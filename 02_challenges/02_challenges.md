# 💡 Challenges Addressed by RAISE (Resilience AI for Singapore Emergencies)

**RAISE** is an AI-powered Disaster Resilience and Preparedness Intelligence (DRPI) system built for the Databricks Smart Business Insights Challenge. It tackles critical challenges across climate resilience, public safety, and emergency response through the lens of open data, AI/BI capabilities, and social impact.

---

## 🌍 Business & Societal Challenges

1. **Climate Vulnerability in Urban Regions**
   - Singapore faces increasing exposure to extreme weather events like heatwaves, thunderstorms, and flash floods due to climate change.
   - Vulnerable populations (e.g., elderly, low-income households) are disproportionately impacted by such events, especially in underserved neighborhoods.

2. **Lack of Real-Time Risk Awareness**
   - Urban populations lack access to localized, real-time insights on climate risks and preparedness measures.
   - Public agencies need better tools to target emergency interventions and optimize resource deployment.

3. **Fragmented View of Resilience**
   - Existing data on weather, health infrastructure, social determinants of health (SDOH), and emergency resources is scattered and difficult to act upon collectively.
   - There is a need for a unified framework that combines environmental, infrastructural, and demographic factors.

---

## 🧠 Technical Challenges

1. **Data Integration Across Disparate Sources**
   - Aggregating and harmonizing data from AccuWeather, PredictHQ, and Singapore’s Open Data APIs involves handling multiple formats (CSV, API, JSON), varying schemas, and update frequencies.

2. **Real-Time & Predictive Indexing**
   - Computing a **Disaster Resilience and Preparedness Index (DRPI)** requires scalable, low-latency pipelines that transform raw geospatial + SDOH + event risk data into actionable insights.

3. **AI Modeling in a Context-Aware Way**
   - The DRPI model must account for domain-specific attributes like heat index severity, forecast uncertainty, neighborhood infrastructure, healthcare proximity, and socio-economic vulnerability.

4. **Visualization & Human-Centric Interaction**
   - Building AI/BI dashboards that are intuitive, real-time, and interactive for a variety of stakeholders (residents, city planners, emergency services).
   - Enabling **Genie Spaces** to allow conversational data exploration in natural language.

5. **Governance, Security & Reusability**
   - Ensuring data governance, traceability, and reusability through **Databricks Unity Catalog** and secure Delta Lake architecture.
   - Enabling seamless integration across **Databricks Apps**, alerting, and workflows.

---
---

## ✅ Summary

**RAISE** rises to meet both societal and technical challenges by leveraging a unified lakehouse platform and open data to drive proactive, AI-enabled disaster resilience insights for Singapore. It empowers city agencies, residents, and responders with real-time visibility, risk scoring, and conversational analytics — building a safer, smarter future.

