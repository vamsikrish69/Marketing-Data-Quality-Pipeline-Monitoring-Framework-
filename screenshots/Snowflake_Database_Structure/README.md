# Snowflake Database Structure

## Business Question

How is the data quality monitoring framework organized within Snowflake?

## Objective

This screenshot demonstrates the overall Snowflake architecture implemented for the Marketing Data Quality & Pipeline Monitoring Framework.

The framework uses a layered architecture to separate ingestion, transformation, validation, monitoring, and reporting responsibilities.

## Architecture

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

## Schemas Included

### RAW

Stores source datasets.

### STAGING

Stores standardized and cleaned datasets.

### QUALITY

Stores validation rules and quality test outputs.

### MONITORING

Stores centralized monitoring tables and alerts.

### ANALYTICS

Stores business-facing scorecards and monitoring reports.

## Business Value

This architecture helps:

- Separate responsibilities
- Improve maintainability
- Simplify troubleshooting
- Support scalable quality monitoring
- Improve trust in analytical reporting

## Expected Output

The screenshot should display:

```text
RAW
STAGING
QUALITY
MONITORING
ANALYTICS
```

within the Snowflake database structure.

## Screenshot Recommendation

The screenshot should focus on the Snowflake object tree showing all schemas created for the framework.
