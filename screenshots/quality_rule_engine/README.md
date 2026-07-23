# Quality Rule Engine

## Business Question

What quality validations are executed across the marketing datasets?

## Objective

This screenshot demonstrates the SQL-based quality rule engine implemented within the QUALITY schema.

The framework validates dataset completeness, accuracy, consistency, freshness, and integrity.

## Quality Rules Implemented

### Row Count Validation

Detects incomplete or missing loads.

### Null Value Checks

Identifies missing business-critical values.

### Duplicate Detection

Validates uniqueness of identifiers.

### Accepted Values Validation

Ensures categorical values remain valid.

### Freshness Monitoring

Detects stale source data.

### Volume Anomaly Detection

Identifies abnormal volume changes.

### Revenue Reconciliation

Validates reporting accuracy.

## Business Value

These validations help:

- Detect data issues early
- Prevent reporting failures
- Improve trust in downstream analytics
- Reduce manual validation effort

## Expected Output

The screenshot should display quality rule tables such as:

```text
TEST_ROW_COUNTS
TEST_NULL_CHECKS
TEST_DUPLICATE_KEYS
TEST_ACCEPTED_VALUES
TEST_FRESHNESS
TEST_VOLUME_ANOMALIES
TEST_REVENUE_RECON
```

## Screenshot Recommendation

The screenshot should focus on quality validation objects within the QUALITY schema.
