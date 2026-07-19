# Marketing Data Quality & Pipeline Monitoring Framework

## Overview

The Marketing Data Quality & Pipeline Monitoring Framework is a Snowflake-based data quality and observability solution designed to ensure the reliability, consistency, and trustworthiness of marketing analytics datasets.

The framework validates data quality across campaign, customer, touchpoint, conversion, and ad spend datasets while providing centralized monitoring, pipeline health reporting, freshness tracking, anomaly detection, alert management, and business-facing quality scorecards.

The project follows a layered architecture consisting of RAW, STAGING, QUALITY, MONITORING, and ANALYTICS schemas to separate ingestion, validation, monitoring, and reporting responsibilities.

---

## Business Problem

Marketing analytics platforms depend on accurate and timely data from multiple sources.

Examples of common data quality issues include:

- Missing campaign identifiers
- Duplicate conversion records
- Delayed source feeds
- Invalid channel values
- Broken table relationships
- Incomplete data loads
- Revenue inconsistencies

These issues directly impact critical business KPIs such as:

- ROAS
- ROI
- CAC
- Conversion Rate
- Attributed Revenue
- Campaign Performance

Without an effective monitoring framework, stakeholders may make decisions based on inaccurate or incomplete information.

This project solves that challenge by proactively identifying and monitoring data quality issues before they impact downstream reporting.

---

## Project Objectives

The framework was designed to:

- Monitor data quality across marketing datasets.
- Detect missing, duplicate, invalid, and stale data.
- Validate source-to-reporting consistency.
- Track pipeline health and quality trends.
- Centralize quality monitoring results.
- Generate business-facing quality scorecards.
- Improve trust in analytical reporting.

---

## Tech Stack

- Snowflake
- SQL
- Data Modeling
- Data Quality Engineering
- Pipeline Monitoring
- Analytics Engineering
- GitHub

---

## Architecture

```text
RAW
 ↓
STAGING
 ↓
QUALITY RULE ENGINE
 ↓
MONITORING LAYER
 ↓
ANALYTICS SCORECARDS
```

---

## Source Datasets

The framework validates the following marketing datasets:

### Campaigns

Campaign master data including channel, objective, and budget.

### Customers

Customer profile and acquisition information.

### Marketing Touchpoints

Campaign interactions including impressions, clicks, and engagement events.

### Conversions

Customer conversion events and associated revenue.

### Ad Spend

Campaign spend, clicks, and impression metrics.

---

## Quality Rules Implemented

### Row Count Validation

Detects missing or incomplete data loads.

### Null Value Checks

Identifies missing business-critical values.

### Duplicate Detection

Validates uniqueness of key identifiers.

### Accepted Values Validation

Ensures categorical fields contain approved values.

### Referential Integrity Checks

Validates relationships across datasets.

### Freshness Monitoring

Detects stale or delayed source feeds.

### Volume Anomaly Detection

Identifies unusual spikes or drops in row counts.

### Revenue Reconciliation

Ensures revenue consistency across reporting layers.

---

## Monitoring Layer

The monitoring layer centralizes data quality results and operational health metrics.

Objects include:

```text
MONITORING.DATA_QUALITY_RESULTS
MONITORING.ALERT_LOG
MONITORING.PIPELINE_HEALTH
MONITORING.DATA_FRESHNESS_RESULTS
```

---

## Analytics Layer

Business-facing reporting objects include:

```text
ANALYTICS.FCT_DATA_QUALITY_RESULTS

ANALYTICS.FCT_PIPELINE_HEALTH

ANALYTICS.FCT_DATA_FRESHNESS

ANALYTICS.FCT_ALERT_SUMMARY

ANALYTICS.DATA_QUALITY_SCORECARD
```

---

## Key Monitoring Capabilities

- Data Completeness Monitoring
- Data Freshness Monitoring
- Pipeline Health Monitoring
- Data Volume Monitoring
- Revenue Validation
- Alert Management
- Quality Scorecards
- Data Reliability Reporting

---

## Business Questions Answered

- Which datasets contain quality issues?
- Which source feeds are delayed?
- Which tests are failing most frequently?
- Which datasets contain invalid values?
- Which pipeline components require attention?
- What is the overall platform quality score?
- Are reporting datasets trustworthy for business use?

---

## Project Outcome

This project demonstrates how modern data engineering teams implement data quality validation, pipeline monitoring, data observability, and business-facing quality reporting using Snowflake SQL.

The framework enables proactive issue detection, improved reporting reliability, and increased confidence in downstream analytical datasets.
