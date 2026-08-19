# Awesome-ETL

## Top ETL Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Data Integration, ELT/ETL Pipelines, Connectors, CDC, Orchestration & Warehouse Loading*
**Last updated: August 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **ETL / ELT**. These tools extract data from sources (SaaS apps, databases, files, streams), transform it, and load it into data warehouses, lakes, or destinations — with reliable connectors, schema handling, scheduling, and monitoring.

**Examples** include Talend, Matillion, Fivetran, Airbyte, Hevo Data, Informatica, IBM DataStage, Azure Data Factory, AWS Glue, and Stitch (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom connectors, DataOps workflows, and full control over data movement — ideal for data engineers, analytics teams, and organizations that want transparent, cost-effective, vendor-lock-in-free pipelines.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms
- **[Talend](https://www.talend.com/)** (Qlik Talend)  
  Enterprise data integration platform with strong ETL, data quality, MDM, and hybrid capabilities. Offers both cloud and self-managed options rooted in open-source heritage.
- **[Matillion](https://www.matillion.com/)**  
  Cloud-native ELT platform optimized for modern data warehouses (Snowflake, BigQuery, Redshift, Databricks). Visual pipeline design with pushdown transformations and strong warehouse-native performance.
- **[Fivetran](https://www.fivetran.com/)**  
  Fully managed ELT leader known for reliability, automatic schema handling, and a large catalog of high-quality connectors. Minimal maintenance for business-critical SaaS-to-warehouse pipelines.
- **[Airbyte](https://airbyte.com/)**  
  Popular open-core data integration platform (also available as managed cloud). Large connector library, Connector Development Kit, and flexible self-hosted or cloud deployment.
- **[Hevo Data](https://hevodata.com/)**  
  No-code / low-code ELT platform focused on real-time or near-real-time pipelines, ease of use, and predictable pricing for growing data teams.
- **[Informatica](https://www.informatica.com/)** (now part of Salesforce)  
  Enterprise-grade data management suite with extensive connectors, data quality, governance, MDM, and AI-assisted integration (CLAIRE).
- **[IBM DataStage](https://www.ibm.com/products/datastage)**  
  High-performance parallel ETL engine for complex, large-scale batch and hybrid workloads, often used in regulated and on-premises environments.
- **[Azure Data Factory](https://azure.microsoft.com/en-us/products/data-factory/)**  
  Microsoft’s cloud data integration service with code-free data flows, hybrid connectivity, SSIS lift-and-shift, and deep Azure ecosystem integration.
- **[AWS Glue](https://aws.amazon.com/glue/)**  
  Serverless ETL/ELT service on AWS with Spark-based jobs, Data Catalog, crawlers, and tight integration with the AWS analytics stack.
- **[Stitch](https://www.stitchdata.com/)**  
  Simple, managed ELT service (originally built on Singer) focused on straightforward SaaS and database replication into warehouses with predictable pricing.

## Open-Source GitHub Projects
- **[Airbyte](https://github.com/airbytehq/airbyte)**  
  Leading open-source ELT platform with 300–600+ connectors (certified + community), Connector Development Kit (CDK), UI, API, and full self-hosting support (Docker/Kubernetes). Strong alternative to managed ELT tools.
- **[Meltano](https://github.com/meltano/meltano)**  
  Declarative, code-first data integration engine built on the Singer specification. CLI-driven, GitOps-friendly, with orchestration support and access to hundreds of Singer taps/targets via Meltano Hub.
- **[Apache NiFi](https://github.com/apache/nifi)**  
  Powerful open-source dataflow system with visual drag-and-drop design for routing, transformation, protocol mediation, and real-time or batch movement. Excellent for complex, event-driven, or IoT-style pipelines.
- **[Apache Airflow](https://github.com/apache/airflow)**  
  The de-facto open-source workflow orchestrator for data pipelines. Define DAGs in Python, schedule complex multi-step ETL/ELT jobs, and monitor execution at scale.
- **[dbt Core](https://github.com/dbt-labs/dbt-core)**  
  Open-source transformation layer (the “T” in ELT). Write modular SQL models, tests, and documentation that run inside the warehouse; pairs perfectly with any extract-load tool.
- **[Singer](https://www.singer.io/)** / Singer taps & targets  
  Open-source specification and ecosystem of composable “taps” (extractors) and “targets” (loaders). Underpins many tools including Meltano and historical Stitch connectors.
- **[dlt (data load tool)](https://github.com/dlt-hub/dlt)**  
  Lightweight Python library for building data pipelines as code. Simple, flexible ingestion with schema inference and support for many sources/destinations.
- **[Sling](https://github.com/slingdata-io/sling)** / **[ingestr](https://github.com/bruin-data/ingestr)** / similar CLIs  
  Modern open-source CLI tools for fast, code-light data movement between databases, files, and warehouses.
- **[Apache Spark](https://github.com/apache/spark)** + related engines  
  Foundational open-source engine for large-scale data processing and custom ETL jobs (often used under Glue, Databricks, or self-managed clusters).

### Additional Strong Open-Source Options
- **Orchestration & workflow engines**: Prefect, Dagster, Kestra, Mage, Temporal, Argo Workflows.
- **Streaming & CDC**: Apache Kafka + Kafka Connect, Debezium, Flink, and related connectors.
- **Legacy / visual tools**: Pentaho Data Integration (PDI/Kettle), older Talend Open Studio lineage (note: Open Studio was discontinued; migrate carefully).
- **Python-centric libraries**: pandas, Polars, joblib, and custom pipeline frameworks.
- Community **connector catalogs**, **schema evolution helpers**, and **data quality tools** (Great Expectations, Soda, etc.).
- Many smaller **CLI extractors**, **DuckDB-based local ETL**, and **GitOps pipeline runners**.

**Frameworks for building custom systems**: Pair **Airbyte** or **Meltano** (extract & load) with **dbt Core** (transform) and **Apache Airflow / Dagster / Prefect** (orchestration). Run everything on Kubernetes or simple Docker for full ownership. Add Apache NiFi for complex routing or Spark for heavy transformation workloads.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- ETL/ELT pipelines often move sensitive or regulated data; ensure compliance with privacy, security, and data-residency requirements.
- Self-hosted open-source solutions require operational expertise (monitoring, scaling, connector maintenance, security hardening) and do not eliminate infrastructure or engineering costs.

---
**Made for data engineers, analytics teams, and platform builders.**  
Let's make data integration more open, reliable, and controllable.