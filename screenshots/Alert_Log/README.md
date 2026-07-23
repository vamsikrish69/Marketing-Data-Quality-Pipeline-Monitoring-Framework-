# Alert Log

## Business Question

Which data quality issues have generated alerts requiring investigation?

## Objective

This analysis monitors alert records generated from failed quality checks across the marketing data platform.

The alert log provides a centralized view of quality incidents that require attention from data engineers, analysts, or business stakeholders.

Alerts may be generated from:

- Row Count Validation Failures
- Null Value Failures
- Duplicate Record Detection
- Accepted Values Violations
- Freshness Monitoring Failures
- Volume Anomaly Detection
- Revenue Reconciliation Issues

## SQL Query Used

```sql
SELECT *
FROM MONITORING.ALERT_LOG
ORDER BY ALERT_DATE DESC;
```

## Metrics Displayed

- Alert ID
- Dataset Name
- Alert Type
- Alert Severity
- Alert Date
- Alert Description

## Business Value

This analysis helps teams:

- Identify quality issues immediately
- Prioritize investigation efforts
- Improve operational monitoring
- Reduce reporting risks
- Improve trust in business analytics
- Support proactive incident management

## Expected Output

The screenshot should display records from:

```text
MONITORING.ALERT_LOG
```

Example output:

```text
ALERT_ID
DATASET_NAME
ALERT_TYPE
SEVERITY
ALERT_DATE
ALERT_DESCRIPTION
```

## Interpretation

Rows returned indicate quality issues that require investigation and remediation.

Each alert represents a failed data quality rule or monitoring condition.

Examples include:

- Missing source data
- Delayed dataset refreshes
- Duplicate records
- Invalid values
- Revenue discrepancies

## No Alerts Scenario

If no rows are returned:

```text
No active alerts exist.
All quality checks passed successfully.
```

This is considered the expected healthy state of the framework and indicates that no critical data quality issues were detected during monitoring.

## Screenshot Recommendation

The screenshot should focus on the query output results.

If alerts exist, display the most recent alerts.

If no alerts are returned, a screenshot showing an empty result set is acceptable because it demonstrates that all implemented quality checks passed successfully.
