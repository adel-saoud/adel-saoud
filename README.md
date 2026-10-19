<div align="center">

# Adel Saoud

### AI & Software Engineer @ SFEIR · on mission at Decathlon France

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=780&lines=AI+Engineer+%C2%B7+SFEIR+%C2%B7+on+mission+at+Decathlon+France;Multi-agent+HR+assistant+%C2%B7+30%2C000%2B+employees+%C2%B7+97.7%25+rubric+pass;Quality+%C2%B7+Cost+%C2%B7+Privacy%2C+covered)](https://git.io/typing-svg)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-adel--saoud-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/adel-saoud)

</div>

---

## About

I'm an AI Engineer at **SFEIR**, a French IT consulting firm, currently on mission at **Decathlon France** building **DaiLY**, a multi-agent HR assistant for 30,000+ employees in Google Chat. A systematic eval pipeline lifted its lead agent's rubric pass rate from ~60% to 97.7%. Before joining SFEIR, I spent five years inside Decathlon: first in France on internal HR tooling, then in the UK building the e-commerce marketplace platform that drove £2.6M GMV in 2024.

I work embedded inside client teams, owning delivery end-to-end. My open-source projects tackle problems I've met running LLMs in production: privacy-safe RAG, cost attribution and quality evaluation.

- 🛠️ Multi-agent systems · RAG · LLMOps · evaluation pipelines
- 🌍 🇫🇷 French (native) · 🇬🇧 English (C2) · 🇪🇸 Spanish

---

## ✅ Live projects

Four open-source projects engineered to production standards: Pyright strict, 86–95% test coverage, CI and eval workflows on every push. Together they cover the three problems every team running LLMs hits:

> - **Cost:** gateway tracks where the budget went; autopilot prevents it going to the wrong place
> - **Quality:** detector catches quality drops when prompts change
> - **Privacy:** guardian keeps personal data out of both the index and the response

### [llm-gateway](https://github.com/adel-saoud/llm-gateway)
An OpenAI-compatible gateway that attributes spend across the four stages of a RAG pipeline (retrieval, reranking, generation, evaluation), so teams stop guessing which stage is eating their budget.

> **RAG-aware cost attribution · multi-provider fallback · circuit breakers · Redis rate limiting · 92% coverage**

### [llm-cost-autopilot](https://github.com/adel-saoud/llm-cost-autopilot)
A two-stage router (embedding similarity, then DeBERTa zero-shot on ambiguous cases) that sends each request to the cheapest capable model, then an async verifier re-runs a sample on a stronger model and logs every routing disagreement to a correction dataset.

> **94.6% agreement with a stronger-model verifier · 14.6% cost reduction on a 1,000-request load test · 95% coverage**

### [llm-regression-detector](https://github.com/adel-saoud/llm-regression-detector)
A CI quality gate that runs your LLM against a golden dataset on every PR, diffs accuracy with Wilson 95% confidence intervals, and blocks the merge when the drop is statistically real.

> **-30pp regression detected automatically in CI · 86% coverage · GitHub Actions + Slack alerts**

### [guardian-rag](https://github.com/adel-saoud/guardian-rag)
A RAG pipeline with three-stage PII detection at ingestion (Presidio, GLiNER, then DeBERTa validation on low-confidence spans only) and a post-generation audit on every answer, designed around EU AI Act data-governance principles (Art. 10).

> **100% PII recall · 0.93 precision on a 91-entity synthetic benchmark · 0 post-generation leaks · 93% coverage**

---

## 🏆 Missions

### DaiLY · GenAI mission @ Decathlon France (via SFEIR) · *2026 · proprietary*
Lead developer on a multi-agent HR assistant in Google Chat serving 30,000+ employees in France, answering in 5 languages.
- Coordinator + **4 specialized sub-agents** over the **A2A protocol** on Cloud Run, built on Google ADK and Gemini (Vertex AI)
- Vertex AI Search RAG pipeline over **100+ HR policy documents**, unifying HR knowledge scattered across **280+ internal tools**; every answer passes a grounding-evidence gate before reply
- LLM-as-Judge eval pipeline: **600+ golden cases** across 4 agents + a coordinator routing suite; rubric pass lifted from **~60% to 97.7% on HR Knowledge**, 87–96% across the remaining agents
- Production security: prompt-injection screening (Google Model Armor), signed agent-to-agent calls, fail-closed PII redaction on LLM traces, EU data residency
- 2-layer production kill switch (5–10s Cloud Run cutoff + 30s TTL registry toggle, no redeploy) · keyless CI/CD via GitHub Actions + Workload Identity Federation
- BigQuery observability tying answer quality to the exact prompt revision (per-prompt-hash, per-model, per-cost-center)
- Technical alignment with Decathlon NL and ES on cross-country RAG architecture

### Marketplace platform · Software Engineer @ Decathlon UK · *2023–2026 · proprietary*
Built the e-commerce marketplace connector platform across three countries.
- 8 Java/Spring Boot microservice connectors across UK, South Korea, and Switzerland
- **£2.6M GMV** in 2024 · **€528K GMV** on the Glovo connector since August 2025
- **40,000+ product updates/day** via Cloud Firestore
- Onboarding time per new marketplace: **8 weeks → 4 weeks**
- Built a cost-free user-management interface in Google Apps Script: **90% reduction in fraudulent transactions across all 90 UK retail stores**

### Software Engineering · Decathlon France · *2021–2023 · proprietary*
Automation of HR processes and internal tooling.
- Built a Java/Spring Boot aggregator integrating with Greenhouse webhooks, cutting manual data entry by 50%
- Streamlined contract generation and internal API workflows

---

## 💻 Tech stack

<p align="center">
  <sub><b>AI &amp; LLM</b></sub><br />
  <img src="https://unpkg.com/@lobehub/icons-static-png@1.97.1/light/gemini-color.png" width="36" height="36" alt="Gemini" title="Gemini" />&nbsp;&nbsp;
  <img src="https://unpkg.com/@lobehub/icons-static-png@1.97.1/light/vertexai-color.png" width="36" height="36" alt="Vertex AI" title="Vertex AI" />&nbsp;&nbsp;
  <picture><source media="(prefers-color-scheme: dark)" srcset="https://unpkg.com/@lobehub/icons-static-png@1.97.1/dark/openai.png" /><img src="https://unpkg.com/@lobehub/icons-static-png@1.97.1/light/openai.png" width="36" height="36" alt="OpenAI" title="OpenAI" /></picture>&nbsp;&nbsp;
  <img src="https://unpkg.com/@lobehub/icons-static-png@1.97.1/light/claude-color.png" width="36" height="36" alt="Claude" title="Claude" />&nbsp;&nbsp;
  <picture><source media="(prefers-color-scheme: dark)" srcset="https://unpkg.com/@lobehub/icons-static-png@1.97.1/dark/ollama.png" /><img src="https://unpkg.com/@lobehub/icons-static-png@1.97.1/light/ollama.png" width="36" height="36" alt="Ollama" title="Ollama" /></picture>&nbsp;&nbsp;
  <img src="https://unpkg.com/@lobehub/icons-static-png@1.97.1/light/huggingface-color.png" width="36" height="36" alt="Hugging Face" title="Hugging Face" />
</p>

<p align="center">
  <sub><b>Backend · Cloud · Data</b></sub><br />
  <img src="https://skillicons.dev/icons?i=py,fastapi,java,spring,kafka,gcp,docker,githubactions,terraform,postgres,redis,firebase,prometheus,grafana&perline=14" alt="Python, FastAPI, Java, Spring Boot, Kafka, Google Cloud, Docker, GitHub Actions, Terraform, PostgreSQL, Redis, Firestore, Prometheus, Grafana" />
</p>

```jsonc
// GET /.well-known/agent-card.json
{
  "name": "Adel Saoud",
  "description": "AI Engineer · lead dev of a multi-agent HR assistant for 30,000+ employees",
  "documentationUrl": "https://linkedin.com/in/adel-saoud",
  "skills": [
    { "id": "agents", "name": "Multi-agent systems",
      "tags": ["Google ADK", "A2A protocol", "Gemini", "Vertex AI"] },
    { "id": "rag", "name": "RAG & grounding",
      "tags": ["Vertex AI Search", "Qdrant", "hybrid search", "Presidio", "GLiNER"] },
    { "id": "evals", "name": "Evaluation & LLMOps",
      "tags": ["LLM-as-Judge", "golden datasets", "MLflow", "Databricks", "OpenTelemetry"] },
    { "id": "safety", "name": "AI safety & privacy",
      "tags": ["Model Armor", "Cloud DLP", "PII redaction"] },
    { "id": "models", "name": "Models",
      "tags": ["Gemini", "OpenAI", "Claude", "Ollama", "Hugging Face"] },
    { "id": "backend", "name": "Backend",
      "tags": ["Python", "FastAPI", "Java", "Spring Boot", "Kafka"] },
    { "id": "cloud", "name": "Cloud & DevOps",
      "tags": ["Google Cloud", "Cloud Run", "Terraform", "Docker", "GitHub Actions"] },
    { "id": "data", "name": "Data & observability",
      "tags": ["BigQuery", "Firestore", "PostgreSQL", "Redis", "Prometheus", "Grafana"] }
  ]
}
```

---

<div align="center">

### Let's connect

Happy to chat about RAG, multi-agent systems, evaluation, and LLMOps.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-adel--saoud-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/adel-saoud)

</div>
