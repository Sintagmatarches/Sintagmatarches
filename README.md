# Sintagmatarches

**Junior Data / AI / ML Engineer**

I build reproducible data and ML systems—from acquisition and transformation to explicit contracts, evaluated models, tested APIs and observable deployment designs.

## Selected projects

### Helsinki Water — Forecasting + Optimization

Reproducible decision-science study of 864 monthly Nuuka water-meter observations across eight Helsinki public properties. Expanding backtests selected ETS before the sealed 2018 evaluation: **0.793 property MASE**, with **97.92% empirical coverage** for nominal 90% conformal intervals.

The negative findings are explicit: SARIMA had lower holdout property MASE, the intervals were over-conservative, and base inspection optimization added **0%** because all three candidates fit. OR-Tools CP-SAT produced a **14.59% expected-value gain** only under the binding eight-hour scenario. Statistical signals are not confirmed leaks; scenario value is not realized savings.

[Source and visual evidence](https://github.com/Sintagmatarches/helsinki-water-forecasting-optimization) · [Scientific report](https://github.com/Sintagmatarches/helsinki-water-forecasting-optimization/blob/main/reports/scientific-report.md) · [Versioned metrics](https://github.com/Sintagmatarches/helsinki-water-forecasting-optimization/blob/main/artifacts/v1.0.0/metrics.json)

### Finland Geospatial AI

Native-resolution PyTorch segmentation of official National Land Survey of Finland RGB orthophotos
with Topographic Database vector supervision. The v2 dataset contains 576 256×256 patches at
0.5 m in EPSG:3067, split across five map sheets with 512 m buffers, exact raster/vector alignment,
content hashes and automated spatial-leakage checks.

MLflow records two U-Net runs and a pretrained SegFormer-B0 run. Validation-only selection chose
SegFormer at 0.7344 mIoU; its single hash-locked 96-patch test produced **0.6652 mIoU** and **0.7742
macro Dice**. Water reached 0.9636 IoU, while open-natural land reached 0.3300. The repository includes
boundary and visual error analysis, calibration and risk-coverage plots, strict CPU GeoTIFF inference,
Docker and CI. The older Sentinel-2 / WorldCover v1 is unchanged at **0.3982 mIoU** and **0.4743 macro
Dice**. The two tracks use different data and class definitions, so their scores cannot be compared directly.

[Source and visual evidence](https://github.com/Sintagmatarches/finland-geospatial-ai) · [NLS v2 experiment report](https://github.com/Sintagmatarches/finland-geospatial-ai/blob/main/reports/v2/generated/experiment-report.md) · [Inference operations](https://github.com/Sintagmatarches/finland-geospatial-ai/blob/main/reports/inference-operations.md)

### EU Tender Intelligence Agent

Official TED Search API ingestion, structured procurement and lot processing, deterministic supplier qualification, version/change intelligence, and evidence-linked decisions. The local runtime adds hybrid retrieval, embeddings, bounded tool calling and a claim/evidence gate, with adversarial tests for prompt injection and forged evidence.

[Live application](https://applied-ai-lab.smjlw.chatgpt.site/eu-tender-intelligence-agent) · [Source and technical evidence](https://github.com/Sintagmatarches/applied-ai-lab#eu-tender-intelligence-agent) · [Operations and SLO proposal](https://github.com/Sintagmatarches/applied-ai-lab/blob/main/docs/tender-ai-operations.md)

The public Cloudflare app provides live TED discovery and deterministic assessment. Docker and Azure Terraform are supplied for the private runtime; the repository does not claim that Azure deployment has been completed.

### Finland Rail Monitoring System

Live and historical monitoring built from official Digitraffic data, with regional geospatial analytics and an executable PySpark / Delta Lake Bronze–Silver–Gold pipeline. Incremental watermarks, idempotent reruns, recovery paths, quality gates and contracts are covered by automated tests.

The committed 1 Aug 2025–31 Jul 2026 snapshot contains **403,054** modelled passenger journeys; **95.81%** of completed final arrivals were within five minutes.

[Live monitor](https://applied-ai-lab.smjlw.chatgpt.site/finland-rail-reliability-monitor) · [Source and methodology](https://github.com/Sintagmatarches/applied-ai-lab#finland-rail-monitoring-system) · [Data-platform evidence](https://github.com/Sintagmatarches/applied-ai-lab/blob/main/docs/rail/data-platform.md)

Power BI / DAX assets and Fabric delivery instructions are prepared; publishing to a user-owned Fabric workspace remains a credentialed manual step.

### Olist Delivery Delay Predictor

A server-side relative risk scorer trained with leakage-safe point-in-time features, chronological validation and comparison of logistic regression, XGBoost, CatBoost and blends. Portable TypeScript inference is tested against the Python reference.

On the 14,471-order final benchmark, the deployed logistic baseline achieved **6.32% PR-AUC**, **63.44% ROC-AUC**, and found **107 of 620** late orders in the highest-risk 10% (7.4% precision). The result is intentionally reported as modest ranking performance, not a calibrated probability claim.

[Live predictor](https://applied-ai-lab.smjlw.chatgpt.site/olist-delivery-delay-predictor) · [Source and evaluation](https://github.com/Sintagmatarches/applied-ai-lab#olist-delivery-delay-predictor) · [Versioned serving contract](https://github.com/Sintagmatarches/applied-ai-lab/blob/main/docs/olist-serving-contract.md)

## Working stack

Python · SQL · PySpark · Delta Lake · Power BI / Power Query / DAX · PyTorch · MLflow · FastAPI · Docker · GitHub Actions · Terraform · Azure-oriented infrastructure · data contracts · RAG / agent systems · time-series ML · computer vision · geospatial ML · OR-Tools / CP-SAT

## More work

- [Portfolio](https://sintagmatarches.github.io/portfolio/?v=20260921-engineering-audit) — live projects, analytical reports, visualizations and certificates.
- [Olist Delivery Reliability report](https://sintagmatarches.github.io/portfolio/assets/olist-delivery-reliability-v2.pdf?v=20260921-engineering-audit) — SQL / Power BI delivery analysis.
- [Estonia County Economic Livability report](https://sintagmatarches.github.io/portfolio/assets/estonia-county-economic-livability-v1.pdf?v=20260921-engineering-audit) — county-level affordability and labour-market analysis.
