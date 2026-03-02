# Product Analytics Data Sources

## Overview

Integration documentation for product analytics platforms.

## Amplitude

### Connection
- API Key: [Project Settings]
- Secret Key: [Project Settings]

### Key Queries

**User Activity:**
```javascript
// Query for active users by account
Amplitude.getInstance().getUserActivity({
  user_id: accountId,
  start: '2024-01-01',
  end: '2024-03-31'
});
```

**Event Breakdown:**
```javascript
// Event types by frequency
Amplitude.EventSnapshot({
  events: ['feature_used', 'workflow_run', 'action_taken'],
  groupby: 'event_type',
  segments: ['account_id']
});
```

## Snowflake

### Connection
- Account: [your-account.snowflakecomputing.com]
- Warehouse: [ANALYTICS_WH]
- Database: [PRODUCT_DB]

### Key Queries

**Usage Summary:**
```sql
SELECT 
  DATE_TRUNC('day', event_time) as date,
  COUNT(DISTINCT user_id) as unique_users,
  COUNT(*) as total_events
FROM PRODUCT_DB.USAGE_EVENTS
WHERE account_id = ?
AND event_time >= DATEADD(day, -90, CURRENT_DATE())
GROUP BY 1
ORDER BY 1;
```

**Feature Adoption:**
```sql
SELECT 
  feature_name,
  COUNT(DISTINCT user_id) as users,
  COUNT(*) as events
FROM PRODUCT_DB.FEATURE_USAGE
WHERE account_id = ?
GROUP BY 1
ORDER BY 2 DESC;
```

## BigQuery

### Connection
- Project: [your-project-id]
- Dataset: [product_analytics]

### Key Queries
Same structure as Snowflake with BigQuery syntax.

## Mixpanel

### Connection
- Project ID: [from settings]
- Service Account: [from settings]

### Key Queries
Use Mixpanel API for user and event data.

## Data Model

### Standard Schema
```
events:
  - event_id
  - event_type
  - user_id
  - account_id
  - timestamp
  - properties (JSON)

users:
  - user_id
  - account_id
  - email
  - role
  - created_at
  - last_active_at
```
