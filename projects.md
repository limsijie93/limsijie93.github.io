---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
toc: true
toc_label: "Projects"
---

A few of the larger systems I've built — each with the outcome, my role, and an architecture sketch. Most of this work sits inside private company codebases, so these are write-ups with sanitized diagrams rather than public repos — happy to walk through any of them in more depth.

## PULSE AI Health Scoring Platform (Teladoc)

**Outcome: a single view of member health across 100M+ members, improving health outcomes by 29%.**

Architected end-to-end — data architecture, ML architecture, training process, and Lakeflow training/inference pipelines — a RAG platform that moves governed member data from the Snowflake Gold layer to a HIPAA-compliant LLM and writes back governed health scores (churn risk, engageability from recruitable → enrolled, chronic-condition clinical risk), with an evaluation layer for confidence, groundedness, calibration, drift, and feature attributions.

![PULSE AI Health Scoring Platform architecture](/assets/images/projects/pulse-ai-rag-platform.svg)

**Stack:** Snowflake (Gold/medallion), HIPAA-compliant LLM, RAG (LangChain, LlamaIndex, Pinecone), Databricks Lakeflow (Azure-hosted), MLflow, Python.

## Unified Predictions Platform / Member360 (Teladoc)

**Outcome: one prediction store serving 10,000 clinicians and 50+ downstream APIs and applications.**

Built a unified prediction store (model registry, SCD2 history, deterministic UUID-v5 IDs, Lakeflow streaming tables + materialized views) with SHAP batch scoring, replacing siloed per-system member data and enabling self-serve member insights via Power BI dashboards. Underpinned by two-level SCD2 identity resolution with a Verato-based Global ID — accelerating go-to-market for new clinical offerings.

![Member360 prediction store data flow](/assets/images/projects/member360-predictions.svg)

**Stack:** Snowflake, Databricks (Lakeflow, Unity Catalog, MLflow), SHAP, dbt.

## Marketing Intelligence Score Portfolio (Teladoc)

**Outcome: +12% upsell conversion and ≥2x campaign lift in top deciles.**

Built and shipped eight production scores across four decision layers — Economic Value, Member State, Action Selection, and Outreach Activation — synthesized into an Expected Value score that ranks members for outreach. Used propensity-score matching to de-bias observational outreach comparisons and uplift modeling to rank members by incremental (causal) effect, validated against a randomized A/B holdout.

![Marketing Intelligence Score Portfolio](/assets/images/projects/marketing-intelligence-portfolio.svg)

**Stack:** Snowflake, Databricks (Lakeflow, MLflow), dbt, Python; gradient-boosted models with SHAP.

## Agentic Systematic Crypto Trading Engine (Pass App)

**Outcome: 1.6 Sharpe over 6 months on ~$500k traded notional, at sub-200ms prediction latency.**

Owned end-to-end an agentic AI-assisted trading engine ingesting X.com signals and multi-provider price feeds (including Hyperliquid perpetuals) for real-time price prediction on a high-throughput streaming pipeline, with Redis Pub/Sub queue management for concurrent asynchronous predictions.

![Agentic crypto trading engine streaming pipeline](/assets/images/projects/crypto-trading-engine.svg)

*The equity curve in the diagram is illustrative with synthetic data — not actual trading results.*

**Stack:** Python, agentic LLM framework, Redis Pub/Sub, real-time streaming pipeline, Hyperliquid.

## AI Alternative-Data Credit-Scoring Engine (Finantier)

**Outcome: 100k+ individuals scored; licensed by Indonesia's regulator (OJK, IKD Batch 15).**

Owned end-to-end — data collection, ETL, predictive modeling — a credit-scoring engine drawing on alternative data (telco, e-commerce, digital-wallet) and open-finance data from 20+ financial institutions. Monitored ~100k API calls per month via Elasticsearch request/response logging and Metabase dashboards.

![AI alternative-data credit-scoring engine](/assets/images/projects/credit-scoring-engine.svg)

**Stack:** Python, FastAPI, PostgreSQL, Elasticsearch, Docker, Kubernetes, Kong Gateway; PubSub + Spark ingestion; AWS SageMaker, AWS Athena.

## Satellite-Imagery Alternative-Data Signal Engine (Vulcan AI)

**Outcome: +16% alpha in palm-oil futures, up to $0.5M P&L impact (26% informational gain).**

Worked embedded with a commodities trading desk end-to-end — from use-case discovery through sourcing and API-ingesting Planet Labs satellite imagery and building Mask-RCNN computer-vision models, to running inference and converting outputs into a productized, Azure-hosted trading-signal offering.

![Satellite-imagery signal engine](/assets/images/projects/satellite-signal-engine.svg)

**Stack:** Python, Mask-RCNN, satellite imagery (Planet Labs), CV inference pipeline, Azure.

---

More detail on any of these — and the rest of my background — is on the [resume](/resume/) page.
