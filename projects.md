---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
toc: true
toc_label: "Projects"
---

A few of the larger systems I've built. Most of this work sits inside private company codebases, so these are write-ups rather than public repos — happy to walk through any of them in more depth.

## PULSE AI Health Scoring Platform (Teladoc)

Architected a RAG (retrieval-augmented generation) platform end-to-end — data architecture, ML architecture, training process, and Lakeflow training/inference pipelines — that moves member data from the Snowflake Gold layer to a HIPAA-compliant LLM and writes back governed health scores (churn risk, engageability, chronic-condition clinical risk), with an evaluation layer for confidence, groundedness, calibration, drift, and feature attributions.

Delivers a single, holistic view of member health that flags health and comorbidity risks early across a 100M+ member ecosystem, improving health outcomes by 29%.

**Stack:** Snowflake (Gold/medallion), HIPAA-compliant LLM, RAG (LangChain, LlamaIndex, Pinecone), Databricks Lakeflow (Azure-hosted), MLflow, Python.

## Unified Predictions Platform / Member360 (Teladoc)

Built a unified prediction store (model registry, SCD2 history, deterministic UUID-v5 IDs, Lakeflow streaming tables + materialized views) with SHAP batch scoring, serving 10,000 clinicians and 50+ downstream APIs and applications and replacing siloed per-system member data.

Underpinned by two-level SCD2 identity resolution with a Verato-based Global ID that consolidates fragmented source-system records into one member identity.

**Stack:** Snowflake, Databricks (Lakeflow, Unity Catalog, MLflow), SHAP, dbt.

## Agentic Systematic Crypto Trading Engine (Pass App)

Owned end-to-end (architecture through implementation) an agentic AI-assisted trading engine that ingests X.com signals and multi-provider price feeds — including Hyperliquid perpetuals — to drive real-time price predictions on a high-throughput streaming pipeline.

Delivered a 1.6 Sharpe ratio over a 6-month window on ~$500k traded notional (~$120k trading revenue), with sub-200ms prediction latency via Redis Pub/Sub queue management.

**Stack:** Python, agentic LLM framework, Redis Pub/Sub, real-time streaming pipeline, Hyperliquid.

## AI Alternative-Data Credit-Scoring Engine (Finantier)

Owned end-to-end — data collection, ETL, and predictive modeling — a credit-scoring engine for individuals across Southeast Asia, drawing on alternative data (telco, e-commerce, digital-wallet) and open-finance data aggregated from 20+ financial institutions.

Scored 100k+ individuals and secured an innovative credit-scoring (ICS) license with Indonesia's regulator (OJK, IKD Batch 15).

**Stack:** Python, FastAPI, PostgreSQL, Elasticsearch, Docker, Kubernetes, Kong Gateway; PubSub + Spark ingestion; AWS SageMaker, AWS Athena.

## Satellite-Imagery Alternative-Data Signal Engine (Vulcan AI)

Worked embedded with a commodities trading desk to own the entire pipeline end-to-end — from use-case discovery, through sourcing and ingesting satellite imagery (Planet Labs) and building computer-vision models (Mask-RCNN), to running inference and converting outputs into a productized, Azure-hosted trading-signal offering.

Drove +16% alpha in palm-oil futures and up to $0.5M P&L impact (26% informational gain).

**Stack:** Python, Mask-RCNN, satellite imagery (Planet Labs), CV inference pipeline, Azure.

---

More detail on any of these — and the rest of my background — is on the [resume](/resume/) page.
