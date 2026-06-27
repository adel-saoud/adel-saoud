<div align="center">

# Adel Saoud

### AI Engineer @ SFEIR · on mission at Decathlon France

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=780&lines=AI+Engineer+%C2%B7+SFEIR+%C2%B7+on+mission+at+Decathlon+France;Multi-agent+HR+assistant+%C2%B7+30%2C000+employees+%C2%B7+97.7%25+accuracy;Quality+%C2%B7+Cost+%C2%B7+Privacy+%E2%80%94+covered)](https://git.io/typing-svg)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-adel--saoud-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/adel-saoud)

</div>

---

## About

I'm an AI Engineer at **SFEIR**, a French IT consulting firm, currently on mission at **Decathlon France** building **DaiLY** — a multi-agent HR assistant for 30,000+ employees in Google Chat, with answer accuracy lifted from ~60% to 97.7% on its lead agent through a systematic eval pipeline. Before joining SFEIR, I spent five years inside Decathlon — first in France on internal HR tooling, then in the UK building the e-commerce marketplace platform that drove £2.6M GMV in 2024.

I work embedded inside client teams, owning delivery end-to-end. My four open-source projects mirror the patterns I ship in production. Currently exploring privacy-safe RAG and cost-attribution patterns for production LLM systems.

- 🛠️ Multi-agent systems · RAG · LLMOps · evaluation pipelines
- 🌍 🇫🇷 French (native) · 🇬🇧 English (C2) · 🇪🇸 Spanish

---

## ✅ Live projects

Four production-grade open-source projects, all type-strict, high-coverage, full CI. Together they cover the three problems every team running LLMs hits:

> **Cost: gateway tracks where the budget went; autopilot prevents it going to the wrong place. Quality: detector catches quality drops when prompts change. Privacy: guardian keeps personal data out of both the index and the response.**

### [llm-gateway](https://github.com/adel-saoud/llm-gateway)
An OpenAI-compatible gateway that attributes spend across the four stages of a RAG pipeline — retrieval, reranking, generation, evaluation — so teams stop guessing which stage is eating their budget.

> **RAG-aware cost attribution · <8ms gateway overhead · multi-provider fallback · circuit breakers · 92% coverage**

### [llm-cost-autopilot](https://github.com/adel-saoud/llm-cost-autopilot)
A two-stage router (embedding similarity, then DeBERTa zero-shot on ambiguous cases) that sends each request to the cheapest capable model, then learns from its own routing mistakes via a feedback loop.

> **94.6% routing accuracy · self-improving · 60–80% cost reduction on typical workloads · 95% coverage**

### [llm-regression-detector](https://github.com/adel-saoud/llm-regression-detector)
A CI quality gate that runs your LLM against a golden dataset on every PR, diffs accuracy with Wilson 95% confidence intervals, and blocks the merge when the drop is statistically real — inspired by the eval pipeline behind DaiLY in production.

> **-30pp regression detected automatically in CI · 86% coverage · GitHub Actions + Slack alerts**

### [guardian-rag](https://github.com/adel-saoud/guardian-rag)
A RAG pipeline with three-stage PII detection at ingestion (Presidio + GLiNER + DeBERTa) and a post-generation audit on every answer — aligned with EU AI Act Article 10 by design.

> **100% PII recall · 0.93 precision · 0 post-generation leaks · 93% coverage**

---

## 🏆 Missions

### DaiLY — GenAI mission @ Decathlon France (via SFEIR) · *2026 · proprietary*
Lead developer on a multi-agent HR assistant in Google Chat serving 30,000+ employees across France and Switzerland.
- Coordinator + **4 specialized sub-agents** over the **A2A protocol** on Cloud Run, built on Google ADK and Gemini (Vertex AI)
- LLM-as-Judge eval pipeline: **600+ golden cases** across 4 agents + a coordinator routing suite — rubric pass lifted from **~60% to 97.7% on HR Knowledge**, 87–96% across the remaining agents
- 2-layer production kill switch (5–10s Cloud Run cutoff + 30s TTL registry toggle, no redeploy) · keyless CI/CD via GitHub Actions + Workload Identity Federation
- BigQuery observability tying answer quality to the exact prompt revision (per-prompt-hash, per-model, per-cost-center)
- Appointed France's technical lead on the **RAG Alignment Task Force** for the 100K-user global rollout

### Marketplace platform — Software Engineer @ Decathlon UK · *2023–2026 · proprietary*
Built the e-commerce marketplace connector platform across three countries.
- 8 Java/Spring Boot microservice connectors across UK, South Korea, and Switzerland
- **£2.6M GMV** in 2024 · **€528K GMV** on the Glovo connector since August 2025
- **40,000+ product updates/day** via Cloud Firestore
- Onboarding time per new marketplace: **8 weeks → 4 weeks**

### Software Engineering — Decathlon France · *2021–2023 · proprietary*
Automation of HR processes and internal tooling.
- Built a Java/Spring Boot aggregator integrating with Greenhouse webhooks — cut manual data entry by 50%
- Streamlined contract generation and internal API workflows

---

## 💻 Tech stack

<div align="center">

### AI & ML
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Vertex AI](https://img.shields.io/badge/Vertex_AI-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Google ADK](https://img.shields.io/badge/Google_ADK-1A73E8?style=for-the-badge&logo=google&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=for-the-badge&logo=google&logoColor=white)
![Claude](https://img.shields.io/badge/Anthropic_Claude-CC785C?style=for-the-badge&logo=anthropic&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![Presidio](https://img.shields.io/badge/Presidio-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![GLiNER](https://img.shields.io/badge/GLiNER-2D3748?style=for-the-badge)

### Backend
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Java](https://img.shields.io/badge/Java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)

### Cloud & Infra
![Google Cloud](https://img.shields.io/badge/Google_Cloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Cloud Run](https://img.shields.io/badge/Cloud_Run-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)

### Databases & Vector
![Postgres](https://img.shields.io/badge/PostgreSQL-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=for-the-badge&logo=googlebigquery&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logo=qdrant&logoColor=white)
![Firestore](https://img.shields.io/badge/Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)

</div>

---

<div align="center">

### Let's connect

Happy to chat about RAG, multi-agent systems, evaluation, and LLMOps.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-adel--saoud-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/adel-saoud)

</div>
