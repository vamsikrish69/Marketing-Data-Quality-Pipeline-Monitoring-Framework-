# Monitoring Data Quality Results

## Business Question

How are quality test results monitored centrally?

## Objective

This screenshot shows the centralized monitoring table containing quality validation results from all implemented checks.

The monitoring layer consolidates quality outcomes into a single operational view.

## SQL Query Used

```sql
SELECT *
FROM MONITORING.DATA_QUALITY_RESULTS
ORDER BY TEST_DATE DESC;
```

## Metrics Displayed

- Dataset Name
- Test Name
- Test Status
- Test Result
- Test Date
- Failure Details

## Business Value

This monitoring layer helps:

- Centralize quality reporting
- Track quality trends
- Identify failing datasets
- Improve operational visibility

## Expected Output

The screenshot should show:

```text
DATASET_NAME
TEST_NAME
TEST_STATUS
TEST_DATE
```

for multiple quality checks.

## Interpretation

Successful records indicate healthy data quality.

Failed records indicate issues requiring investigation.

## Screenshot Recommendation

The screenshot should focus on the monitoring results table.
