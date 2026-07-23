# Freshness Monitoring

## Business Question

Which datasets are delayed or potentially stale?

## Objective

This analysis measures data freshness and identifies delayed source feeds.

## SQL Query Used

```sql
SELECT *
FROM MONITORING.DATA_FRESHNESS_RESULTS;
```

## Metrics Displayed

- Dataset Name
- Latest Record Date
- Days Delayed
- Freshness Status
- Freshness Category

## Business Value

This analysis helps:

- Detect delayed pipelines
- Monitor ingestion health
- Reduce stale reporting risks
- Improve operational awareness

## Expected Output

The screenshot should display freshness metrics for each dataset.

## Interpretation

Datasets with larger delays may indicate ingestion issues requiring investigation.

## Screenshot Recommendation

The screenshot should focus on freshness monitoring results and dataset status indicators.
