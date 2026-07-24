# Quality Rule Engine

## Business Question

What data quality validations are implemented across the marketing analytics platform?

## Objective

This screenshot demonstrates the SQL-based Quality Rule Engine implemented within the `QUALITY` schema.

The framework validates dataset completeness, accuracy, consistency, freshness, and integrity before data is consumed by downstream analytical reports.

The Quality Rule Engine serves as the foundation of the monitoring framework and helps ensure that business stakeholders can trust the underlying marketing data.

## SQL Query Used

```sql
SHOW VIEWS IN SCHEMA QUALITY;
```

## Quality Rules Implemented

### Row Count Validation

Detects incomplete or missing data loads.

### Null Value Checks

Identifies missing business-critical values.

### Duplicate Detection

Validates uniqueness of key identifiers.

### Accepted Values Validation

Ensures categorical fields contain approved business values.

### Freshness Monitoring

Detects delayed or stale source feeds.

### Volume Anomaly Detection

Identifies unusual increases or decreases in data volume.

### Revenue Reconciliation

Validates revenue consistency across reporting layers.

## Validation Objects Displayed

The screenshot should display quality validation objects such as:

```text
INT_ACCEPTED_VALUES
INT_DUPLICATE_CHECKS
INT_FRESHNESS
INT_NULL_CHECKS
INT_ROW_COUNTS
INT_REVENUE_RECON
```

along with additional quality validation views implemented within the QUALITY schema.

## Business Value

These validations help:

- Detect data quality issues early
- Prevent inaccurate reporting
- Improve trust in analytical outputs
- Reduce manual validation effort
- Increase data reliability
- Support proactive monitoring
