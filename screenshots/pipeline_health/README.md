# Pipeline Health Summary

## Business Question

What is the overall health status of the marketing data pipeline?

## Objective

This analysis provides a consolidated health score for the platform by aggregating quality validation results.

## SQL Query Used

```sql
SELECT *
FROM MONITORING.PIPELINE_HEALTH;
```

## Metrics Displayed

- Total Tests
- Passed Tests
- Failed Tests
- Quality Score
- Pipeline Status

## Business Value

This summary helps:

- Measure platform health
- Identify operational issues
- Track quality performance
- Support data governance

## Expected Output

The screenshot should display:

```text
TOTAL_TESTS
PASSED_TESTS
FAILED_TESTS
QUALITY_SCORE
PIPELINE_STATUS
```

## Interpretation

A higher quality score indicates stronger data reliability.

A healthy pipeline should show:

```text
High Quality Score
Few or No Failed Tests
Healthy Pipeline Status
```

## Screenshot Recommendation

The screenshot should focus on overall pipeline metrics and health indicators.
