## Project Screenshots

### 1. Snowflake Database Structure

screenshots/01_snowflake_database_structure.png

This screenshot shows the Snowflake database structure used in the project, including RAW, STAGING, QUALITY, MONITORING, and ANALYTICS schemas.

---

### 2. Quality Rule Engine

screenshots/02_quality_rule_engine.png

This screenshot shows the quality rule engine objects created in the QUALITY schema, including row count checks, null checks, duplicate checks, accepted values checks, freshness checks, volume anomaly checks, and revenue reconciliation checks.

---

### 3. Monitoring Data Quality Results

screenshots/03_monitoring_data_quality_results.png

This screenshot shows the centralized monitoring output from `MONITORING.DATA_QUALITY_RESULTS`, where all quality test results are combined into a single monitoring layer.

---

### 4. Pipeline Health Summary

screenshots/04_pipeline_health.png

This screenshot shows the overall pipeline health summary, including total tests, passed tests, failed tests, quality score, and pipeline status.

---

### 5. Data Quality Scorecard

screenshots/05_data_quality_scorecard.png

This screenshot shows the business-facing data quality scorecard with quality dimensions such as completeness, uniqueness, validity, consistency, freshness, volume stability, and revenue accuracy.

---

### 6. Freshness Monitoring

screenshots/06_freshness_monitoring.png

This screenshot shows freshness monitoring results, including latest record date, days delayed, freshness status, and freshness category for each dataset.

---

### 7. Alert Log

screenshots/07_alert_log.png

This screenshot shows the alert log generated from failed checks. If no rows are returned, it indicates that no active alerts were generated because all quality checks passed.
