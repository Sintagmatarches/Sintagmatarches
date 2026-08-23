# Sintagmatarches

Data · BI · Analytics Engineering · Machine Learning · Applied AI

I build reproducible analytical projects and working data products—from acquisition and transformation to explicit metrics, evaluated models and public interfaces.

## Selected projects

### EU Tender Intelligence Agent

Official TED Search API ingestion, structured procurement and lot processing, deterministic supplier qualification, version/change intelligence, and evidence-linked decisions. The local runtime adds hybrid retrieval, embeddings, bounded tool calling and a claim/evidence gate, with adversarial tests for prompt injection and forged evidence.

[Live application](https://applied-ai-lab.smjlw.chatgpt.site/eu-tender-intelligence-agent) · [Source and technical evidence](https://github.com/Sintagmatarches/applied-ai-lab#eu-tender-intelligence-agent) · [Evaluation](https://github.com/Sintagmatarches/applied-ai-lab/blob/main/docs/tender-ai-evaluation.md)

The public Cloudflare app provides live TED discovery and deterministic assessment. Docker and Azure Terraform are supplied for the private runtime; the repository does not claim that Azure deployment has been completed.

### Finland Rail Monitoring System

Live and historical monitoring built from official Digitraffic data, with regional geospatial analytics and an executable PySpark / Delta Lake Bronze–Silver–Gold pipeline. Incremental watermarks, idempotent reruns, recovery paths, quality gates and contracts are covered by automated tests.

The committed 1 Aug 2025–31 Jul 2026 snapshot contains **403,054** modelled passenger journeys; **95.81%** of completed final arrivals were within five minutes.

[Live monitor](https://applied-ai-lab.smjlw.chatgpt.site/finland-rail-reliability-monitor) · [Source and methodology](https://github.com/Sintagmatarches/applied-ai-lab#finland-rail-monitoring-system) · [Data-platform evidence](https://github.com/Sintagmatarches/applied-ai-lab/blob/main/docs/rail/data-platform.md)

Power BI / DAX assets and Fabric delivery instructions are prepared; publishing to a user-owned Fabric workspace remains a credentialed manual step.

### Olist Delivery Delay Predictor

A server-side relative risk scorer trained with leakage-safe point-in-time features, chronological validation and comparison of logistic regression, XGBoost, CatBoost and blends. Portable TypeScript inference is tested against the Python reference.

On the 14,471-order final benchmark, the deployed logistic baseline achieved **6.32% PR-AUC**, **63.44% ROC-AUC**, and found **107 of 620** late orders in the highest-risk 10% (7.4% precision). The result is intentionally reported as modest ranking performance, not a calibrated probability claim.

[Live predictor](https://applied-ai-lab.smjlw.chatgpt.site/olist-delivery-delay-predictor) · [Source and evaluation](https://github.com/Sintagmatarches/applied-ai-lab#olist-delivery-delay-predictor) · [Model card](https://github.com/Sintagmatarches/applied-ai-lab/blob/main/artifacts/model-card.md)

## Working stack

Python · SQL · Power BI / Power Query / DAX · PySpark · Delta Lake · data quality and contracts · classical ML · RAG / retrieval · agent tool calling · Docker · GitHub Actions · Terraform

## More work

- [Portfolio](https://sintagmatarches.github.io/portfolio/?v=20260823-current-projects-v1) — live projects, analytical reports and visualizations.
- [Olist Delivery Reliability report](https://sintagmatarches.github.io/portfolio/assets/olist-delivery-reliability-v2.pdf?v=20260823-current-projects-v1) — SQL / Power BI delivery analysis.
- [Estonia County Economic Livability report](https://sintagmatarches.github.io/portfolio/assets/estonia-county-economic-livability-v1.pdf?v=20260823-current-projects-v1) — county-level affordability and labour-market analysis.
