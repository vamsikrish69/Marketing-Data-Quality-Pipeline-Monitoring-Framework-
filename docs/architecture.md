# Architecture

## Overview

The project follows a layered architecture designed to separate ingestion, validation, monitoring, and reporting responsibilities.

```text
RAW
 ↓
STAGING
 ↓
QUALITY
 ↓
MONITORING
 ↓
ANALYTICS
```

---

## Database Structure

```text
MARKETING_DATA_QUALITY_DB

├── RAW
├── STAGING
├── QUALITY
├── MONITORING
└── ANALYTICS
```

---

## RAW Layer

Stores source datasets as loaded from files.

Objects:

```text
CAMPAIGNS
CUSTOMERS
MARKETING_TOUCHPOINTS
CONVERSIONS
AD_SPEND
```

---

## STAGING Layer

Standardizes source data.

Objects:

```text
STG_CAMPAIGNS
STG_CUSTOMERS
STG_MARKETING_TOUCHPOINTS
STG_CONVERSIONS
STG_AD_SPEND
```

Responsibilities:

- Text standardization
- Data cleaning
- Validation preparation

---

## QUALITY Layer

Contains validation rules.

Objects:

```text
INT_ROW_COUNT_CHECKS
INT_NULL_CHECKS
INT_DUPLICATE_CHECKS
INT_ACCEPTED_VALUES_CHECKS
INT_REFERENTIAL_INTEGRITY_CHECKS
INT_FRESHNESS_CHECKS
INT_VOLUME_ANOMALY_CHECKS
INT_REVENUE_RECONCILIATION
```

---

## MONITORING Layer

Centralizes quality results.

Objects:

```text
DATA_QUALITY_RESULTS
ALERT_LOG
PIPELINE_HEALTH
DATA_FRESHNESS_RESULTS
```

---

## ANALYTICS Layer

Business-facing monitoring marts.

Objects:

```text
FCT_DATA_QUALITY_RESULTS
FCT_PIPELINE_HEALTH
FCT_DATA_FRESHNESS
FCT_ALERT_SUMMARY
DATA_QUALITY_SCORECARD
```

---

## End-to-End Flow

```text
Source Data
 ↓
RAW
 ↓
STAGING
 ↓
QUALITY RULES
 ↓
MONITORING RESULTS
 ↓
ANALYTICS DASHBOARDS
```
