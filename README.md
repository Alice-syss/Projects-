# Projects- 1

# Cloud Logistics Data Pipeline & SLA Analytics Framework

## Executive Program Overview
This program establishes a decoupled data framework designed to ingest raw, multi-modal logistical tracking data, enforce strict data quality constraints, and prepare records for cloud data warehousing to drive real-time Service Level Agreement (SLA) telemetry.

## system Architecture & Workflow
1. **Transformation Layer (Python/Pandas):** Ingests raw operational payloads, implements robust error handling to bypass system blocks, standardizes text casing, and programmatically manages missing numeric fields using median metrics.
2. **Analytics Warehousing Layer (Snowflake):** Establishes optimized cloud relational data tables and utilizes advanced SQL conditional aggregation (`COUNT(CASE WHEN...)`) to build reusable business views.

##  Core Operational Metrics Captured
* **Delivery SLA Accuracy (%):** Evaluates successful delivery completions against total volume metrics.
* **Network Physical Dimensions:** Synthesizes rolling averages for package weights and transit vectors grouped by transportation modes (`KARA`, `HAVA`, `DENİZ`).

Data Extracted from: https://www.kaggle.com/datasets/sezginkaraglle/logistics-dataset?resource=download
