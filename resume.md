---
layout: single
title: "Resume"
permalink: /resume/
toc: true
toc_sticky: true
toc_label: "Contents"
last_synced: "2026-10-09 22:25 UTC"
---

# Si Jie Lim
limsijie93@gmail.com | [GitHub](https://github.com/limsijie93) | [LinkedIn](https://linkedin.com/in/si-jie-lim/)
Work authorization: United States · Canada · Taiwan · Singapore | Open to international relocation
Languages: English (fluent), Mandarin Chinese (fluent) | Open to regional and international travel

## Summary
Senior data scientist and AI/ML tech lead with ~8 years across regulated financial services, insurtech, alternative-data trading, open finance, and healthcare AI. Currently leads the PULSE AI team at Teladoc Health, building end-to-end ML and LLM prediction platforms on Snowflake and Databricks that power an outcome-based health model across a 100M+ member base. Strengths span production ML systems and MLOps, agentic AI, and quantitative trading, complemented by adjunct teaching and curriculum development with 90%+ mid-career conversion outcomes.

## Professional Experience

### Teladoc Health – US-listed leader in integrated virtual care (100M+ members); a consumer-facing marketplace matching patients to clinical service providers
*United States*
**Senior Data Scientist — AI/ML Tech Lead (PULSE AI)** | Oct 2022 – Present
- Lead a 5-person PULSE AI team and partner with a 10-person cross-discipline agile pod to own the end-to-end process for production ML and AI software components across marketing-enablement, clinical-risk, member-engagement, and platform workflows for a 100M+ member ecosystem.
- Architected and built the PULSE AI scoring platform end-to-end (data and ML architecture, training process, Lakeflow training/inference pipelines), delivering a holistic single view of member health that flags health and comorbidity risks early and improved health outcomes by 29%.
- Built the Unified Predictions Platform / Member360 store serving 10,000 clinicians and 50+ downstream APIs and applications, enabling self-serve access to member insights and PULSE AI scores across Product, Marketing, and Clinical teams via Power BI dashboards, replacing siloed per-system member data and accelerating go-to-market for new clinical offerings.
- Built a revenue forecasting model against service enrollment to support revenue planning and resourcing decisions.
- Analyzed the end-to-end consumer acquisition-to-enrollment funnel in Amplitude and Mixpanel, complementing Snowflake/dbt pipeline analytics with product-usage instrumentation to inform onboarding and enrollment optimization.
- Own production software quality beyond ML/data pipelines, including API/service integration points, tests, code reviews, CI/CD gates, monitoring, incident response, and root-cause fixes for downstream platform reliability.
- Shipped an eight-score marketing-intelligence portfolio (economic value, member state, action selection, outreach activation) with an Expected Value synthesis; used propensity-score matching to de-bias observational outreach comparisons and uplift modeling to rank members by incremental (causal) effect for Action Selection, then validated top-decile uplift rankings against a randomized A/B holdout, lifting upsell conversion 12% and driving ≥2x campaign lift in top deciles.
- Improved retention (+21% MAU) and reduced churn (-17%) across the 100M+ member base via inactivity prediction (gradient-boosted survival models, XGBoost) and personalized nudges.
- Architected personalized recommendations across the enrollment journey to improve cost efficiency (+24% revenue; -18% cost), and pioneered a next-best-action engine to gamify engagement (+11%) and improve clinical outcomes (+14%).
- Owned the build-vs-buy decision to select Databricks as the ML/data platform and Snowflake as the underlying data infrastructure, then established the ML platform foundation on Databricks (Lakeflow Declarative Pipelines, Unity Catalog, MLflow, Azure-hosted) with dbt transformations and CI/CD + A/B-testing orchestration (Terraform, GitHub Actions), cutting deployment lead time 46% and lifting team productivity 44%; fine-tuned and productionized LLMs (QLoRA, RLHF via PyTorch and Hugging Face Transformers), reducing time to deployment 53%.
- Built a RAG (retrieval-augmented generation) pipeline for the HIPAA-compliant LLM using LangChain and LlamaIndex over a Pinecone vector store, grounding LLM outputs in governed member data retrieved from the Snowflake Gold layer.
- Realized 19% in client value by applying AI to drive better clinical outcomes for users under Value-Based Care (VBC) services.

### Pass App – AI-powered Web3 wallet
*Switzerland*
**Senior AI/Machine Learning Engineer (Advisory, concurrent)** | Mar 2025 – Nov 2025
- Owned end-to-end an agentic AI-assisted crypto-trading engine ingesting X.com signals and multi-provider price feeds (including Hyperliquid perpetuals) for real-time price prediction on a high-throughput streaming pipeline, achieving a 1.6 Sharpe ratio over a 6-month window on ~$500k traded notional (~$120k trading revenue).
- Implemented Redis Pub/Sub queue management for asynchronous API calls to the crypto-trading prediction engine, reducing latency to sub-200 ms and enabling concurrent predictions.
- Drove AI-assisted development across a 20+ engineer team — introducing Cursor, Claude Code, and context-engineering practices — increasing shipping velocity 33% and doubling test-driven code quality.
- Built a collaborative-filtering recommender surfacing tokens and next-best actions, lifting user engagement 35% and trading activity 41%.
- Built agentic DeFi research and Web3-onboarding frameworks on the Microsoft Agent Framework and LangGraph to automate protocol research and onboard new users with jargon-free guidance.

### Finantier – Open-finance startup, Y Combinator (W21)
*Singapore*
**Engineering Manager (Head of Data)** | Feb 2021 – Oct 2022
- Led a team of 8 as Head of Data / Engineering Manager, owning hiring, roadmap, and cross-functional delivery.
- Owned end-to-end an AI alternative-data credit-scoring engine (data collection → ETL → predictive modeling) that scored 100k+ individuals across Southeast Asia, and secured an innovative credit-scoring (ICS) license with Indonesia’s regulator (OJK, IKD Batch 15).
- Designed and optimized PostgreSQL source-system schemas for customer profiles, bank transactions, and credit transactions; wrote SQL for ETL/data ingestion and analytics workflows, including index optimization for faster querying.
- Implemented Elasticsearch request/response logging for credit-scoring API calls and created Metabase dashboards and queries to monitor ~100k API calls per month across production usage.
- Trained and deployed credit-scoring models on AWS SageMaker and used AWS Athena for large-scale SQL analytics over data-lake exports, complementing the GitLab CI/CD, Kubeflow, and MLflow-based MLOps platform.
- Built an MLOps platform (GitLab CI/CD, Kubeflow, MLflow, Evidently.ai, AWS SageMaker) that accelerated model releases to a biweekly cadence, increased monitoring frequency 13× (quarterly → weekly), and cut deployment lead time 42%.
- Architected a separate streaming platform (PubSub, Spark) across microservices, increasing API throughput 45% and reducing latency 32%.

### Vulcan AI – AI startup funded by EDB Singapore
*Singapore*
**AI Data Scientist** | Aug 2019 – Feb 2021
- Used alternative data to drive commodities-trading decisions for the client's trading desk — working embedded end-to-end, from use-case discovery through delivery, building a satellite-imagery alternative-data signal engine (sourcing imagery via Planet Labs, computer-vision models via Mask-RCNN, converting inference into trading signals) and turning it into a productized, Azure-hosted offering, driving +16% alpha in palm-oil futures and up to $0.5M P&L impact (26% informational gain).
- Deployed a computer-vision system (multi-object tracking + fruit grading) at palm-oil mills processing ~1,000 tons of fruit, lifting mill throughput and oil-extraction rate 21%.
- Built hyper-local satellite-imagery insights for palm-oil estate planning and crop/land-use decisions, cutting land-use-planning cost 11%.

### NTUC Income – Largest composite insurer in Singapore
*Singapore*
**Senior Executive, Business Intelligence (Analytics CoE)** | Aug 2018 – Aug 2019
- Built a propensity model predicting whether existing customers would purchase additional products, driving a 3.4% increase in new premiums through targeted cross-sell.
- Developed a claims-legitimacy model to flag non-legitimate claims on existing policies, improving claim efficacy and cost efficiency 4.8% and informing an underwriting-process redesign.

### DBS Bank Ltd – Largest bank in SEA; Best Bank in the World (2018–2020)
*Singapore*
**Business Analytics Graduate Immersion Programme** | Aug 2017 – Aug 2018
- Built A/B tests and design experiments on real-time clickstream data that improved app sign-up rate 14.5% for user onboarding.
- Worked with Amazon DynamoDB NoSQL storage for consumer app-session state in the DBS app, supporting session continuity and analytics for real-time onboarding experiments.
- Developed an ML-based DLP alert-prioritization model and NLP risk-surveillance models that reduced data loss 16.7% per alert.

### Pioneers & Leaders – Financial media publisher
*Singapore*
**Financial Journalist** | Apr 2014 – Jul 2017
- Grew readership 24.9% with synthesized, accessible financial content on macro trends and public-listed stocks.

## Advisory & Teaching (Concurrent)

### TripleTen – Online tech bootcamp for career switchers
*United States*
**Subject Matter Expert — Data Science, ML & AI (Advisory)** | Nov 2024 – Present
- Serve as the Data Science, ML & AI subject-matter expert in a part-time advisory capacity, driving AI-focused content development and train-the-trainer enablement across the curriculum.
- Deliver live, multi-day workshops and bootcamps to approximately 12 enterprise learner cohorts per year (~25 learners per cohort, ~300 learners/year) via Zoom, Google Meet, and Microsoft Teams as part of TripleTen's enterprise-facing delivery model, spanning a broad mix of industries among the 100+ B2B clients served.
- Partner closely with TripleTen's sales team to design and deliver an "AI for Sales" curriculum for enterprise learners, facilitating sales-specific AI training alongside the core engineering/data-science curriculum.
- Built AI grading workflows and a learner-facing learning assistant, adding AI safety guardrails to prevent misuse and support responsible learner interactions.
- Partner with product managers and business stakeholders on AI product delivery timelines and outcomes for 100+ B2B clients running workforce upskilling programs, with biweekly releases and average learning-assistant usage of about 100 AI/API calls per user per week.
- Run regular evaluations of stochastic model behavior and user feedback loops, using learner-reported issues to adjust responses, prompt behavior, rollout rules, and product UX.
- Built core course content — AI-Assisted Programming (with an emphasis on agentic development), Basics of Machine Learning, Data Wrangling, Data Visualization in Tableau, and Data Visualization for Better Business Insights.
- Authored hands-on workshop content including the Prompting Playbook, Agentic Development, and “How To Make Your Agents Smarter With Skills.”
- Trained 5+ instructors who went on to deliver workshops to 500+ learners, scaling AI-literacy content across the program.

### Adjunct Lecturer – BCG, Ngee Ann Polytechnic, Udacity, Le Wagon, MAGES Institute
*United States*
**Lecturer & Curriculum Developer** | Jan 2021 – Present
- Achieved 90% career conversion for mid-career switchers into data science and data engineering roles.
- Delivered live, cohort-based training at BCG to approximately 6 cohorts per year (~70 learners per cohort, ~420 learners/year).
- Lecturer and curriculum/module developer across Agile DataOps, Data Analytics/Science, Artificial Intelligence, AI Programming with Python, the Business Analytics Nanodegree, and Quantitative Finance for Real Estate Investing.

## Selected Projects

### PULSE AI Health Scoring Platform (Teladoc)
- Architected end-to-end — data architecture, ML architecture, training process, and Lakeflow training/inference pipelines — a RAG (retrieval-augmented generation) platform, built with LangChain and LlamaIndex over a Pinecone vector store, that moves member data from the Snowflake Gold layer to a HIPAA-compliant LLM and writes back governed health scores (churn risk, engageability from recruitable → enrolled, chronic-condition clinical risk) with an evaluation layer for confidence, groundedness, calibration, drift, and feature attributions.
- Delivers a single, holistic view of member health that flags health and comorbidity risks early across the 100M+ member ecosystem, improving health outcomes by 29%.
- **Stack:** Snowflake (Gold/medallion), HIPAA-compliant LLM, RAG (LangChain, LlamaIndex, Pinecone vector store), Databricks Lakeflow (Azure-hosted), MLflow, Python.

### Unified Predictions Platform / Member360 (Teladoc)
- Built a unified prediction store (model registry, SCD2 history, deterministic UUID-v5 IDs, Lakeflow streaming tables + materialized views) with SHAP batch scoring, serving 10,000 clinicians and 50+ downstream APIs and applications and replacing siloed per-system member data.
- Underpinned by two-level SCD2 identity resolution with a Verato-based Global ID that consolidates fragmented source-system records into one member identity — accelerating go-to-market for new clinical offerings and reducing downstream integration friction.
- **Stack:** Snowflake, Databricks (Lakeflow, Unity Catalog, MLflow), SHAP, dbt.

### Marketing Intelligence Score Portfolio (Teladoc)
- Built and shipped eight production scores across four decision layers — Economic Value, Member State, Action Selection, and Outreach Activation — synthesized into an Expected Value score that ranks members for outreach.
- Lifted upsell conversion 12% and drove ≥2x campaign lift in top deciles.
- **Stack:** Snowflake, Databricks (Lakeflow, MLflow), dbt, Python; gradient-boosted models with SHAP.

### Agentic Systematic Crypto Trading Engine (Pass App)
- Owned end-to-end (architecture through implementation) an agentic AI-assisted trading engine that ingests X.com signals and multi-provider price feeds — including Hyperliquid perpetuals — to drive real-time price predictions on a high-throughput streaming pipeline.
- Delivered a 1.6 Sharpe ratio over a 6-month window on ~$500k traded notional (~$120k trading revenue).
- Used Redis Pub/Sub for queue management of asynchronous prediction API calls, supporting concurrent crypto-trading predictions with sub-200 ms latency.
- **Stack:** Python, agentic LLM framework, Redis Pub/Sub, real-time streaming pipeline, Hyperliquid.

### AI Alternative-Data Credit-Scoring Engine (Finantier)
- Owned end-to-end — data collection, ETL, and predictive modeling — a credit-scoring engine for individuals across Southeast Asia, drawing on alternative data (telco, e-commerce, digital-wallet) and open-finance data aggregated from 20+ financial institutions.
- Scored 100k+ individuals and secured an innovative credit-scoring (ICS) license with Indonesia’s regulator (OJK, IKD Batch 15).
- Implemented Elasticsearch request/response logging for credit-scoring API calls and created Metabase dashboards and queries to monitor ~100k API calls per month across production usage.
- **Stack:** Python, FastAPI, PostgreSQL, Elasticsearch, Docker, Kubernetes, Kong Gateway; PubSub + Spark ingestion; AWS SageMaker (training/deployment), AWS Athena (large-scale SQL analytics).

### Satellite-Imagery Alternative-Data Signal Engine (Vulcan AI)
- Worked embedded with the client's commodities trading desk to own the entire pipeline end-to-end — from use-case discovery, through sourcing and API-ingesting satellite imagery (Planet Labs) and building computer-vision models (Mask-RCNN), to running the inference pipeline and converting outputs into a productized, Azure-hosted trading-signal offering.
- Drove +16% alpha in palm-oil futures and up to $0.5M P&L impact (26% informational gain).
- **Stack:** Python, Mask-RCNN, satellite imagery (Planet Labs), CV inference pipeline, Azure.

## Technical Skills
- **Languages & Querying:** Python, SQL, JavaScript, Solidity
- **AI-Assisted Development & Rapid Prototyping:** Claude (Claude Chat, Claude Code, Claude Cowork), Cursor, Lovable, Supabase, Vercel, GitHub, context engineering
- **ML & AI:** LLMs (QLoRA, RLHF, prompt engineering), RAG (LangChain, LlamaIndex, Pinecone vector store), Hugging Face Transformers, PyTorch, TensorFlow, scikit-learn, XGBoost, agentic frameworks (LangGraph, Microsoft Agent Framework), computer vision (Mask-RCNN), SHAP, recommendation systems, survival & propensity modeling, causal inference (uplift modeling, propensity-score matching), A/B testing
- **Data & ML Platforms:** Databricks (Lakeflow Declarative Pipelines, Unity Catalog, MLflow), Snowflake (medallion architecture), Spark / PySpark, dbt, Feast (feature store), Kubeflow, Evidently.ai
- **Databases, Search & Queues:** PostgreSQL, Amazon DynamoDB, Elasticsearch, Redis Pub/Sub
- **Cloud & DevOps:** GCP, AWS (SageMaker, Athena), Azure, Docker, Kubernetes, Terraform, GitHub Actions, GitLab CI/CD, Linux, Git
- **Visualization & Product Analytics:** Tableau, Power BI, Metabase, Amplitude, Mixpanel

## Education
- WorldQuant University — M.Sc. Financial Engineering, High Distinction USA (2018 – 2021) — light coursework exposure to financial market-data terminals (Bloomberg, Wind, FactSet, CapitalIQ)
- Nanyang Technological University — B.Bus. (Actuarial Science) Singapore (2014 – 2017) — light coursework exposure to financial market-data terminals (Bloomberg, Wind, FactSet, CapitalIQ)

## Certifications
- Google Cloud Certified — Professional Cloud Architect Sep 2024
- WSQ Advanced Certificate in Learning & Performance (ACLP) 2.0 Mar 2024
- Certified Scrum Master (CSM)
- Encode Solidity Foundation Bootcamp; Solidity Bootcamp; Solana Developer Bootcamp Apr – May 2023
- Alchemy University Ethereum Bootcamp; Encode Zero-Knowledge (ZK) Bootcamp Dec 2022 – Mar 2023

## Hackathons & Awards
- **Hackathons:** BNBChain Zero2Hero; Chainlink Spring 2023; Encode x Polkadot Spring 2023 2023
- **Awards:** CADS Sunrise Rising Data Scientist in ASEAN; Grab AI for SEA Challenge (Top 50); POEMS 2.0 Challenge (Best ETF Investor); CIMB ASEAN Stock Challenge
