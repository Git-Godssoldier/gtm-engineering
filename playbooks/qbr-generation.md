# QBR Generation Playbook

## Overview

Generate Quarterly Business Review (QBR) decks in 10 minutes instead of 6 hours.

## Prerequisites

- Snowflake/BigQuery access (product usage)
- Salesforce/HubSpot access (CRM)
- Gong/Chorus access (conversations)
- Zendesk/Linear access (support)
- Brand template

## Step-by-Step Process

### Step 1: Trigger Generation

**Manual:** `/generate_qbr [account_name]`

**Scheduled:** Auto-generate 2 weeks before scheduled QBR

### Step 2: Aggregate Data (Parallel)

Query all sources simultaneously:

```sql
-- Product Usage (Snowflake)
SELECT date, total_events, unique_users, feature_breakdown
FROM usage_events
WHERE account_id = ?
AND date >= date_sub(current_date, interval 90 day)

-- CRM (Salesforce)
SELECT * FROM Account WHERE Id = ?
SELECT * FROM Opportunity WHERE AccountId = ?

-- Conversations (Gong)
GET /calls?account_id=?&from_date=90d_ago

-- Support (Zendesk)
GET /tickets?organization_id=?&created_within=90d
```

### Step 3: Extract Insights

**From Conversations:**
- Implemented use cases
- Pain points mentioned
- Expansion signals
- Feature requests
- Key quotes

**From Support:**
- Ticket volume trend
- Common issues
- CSAT scores
- Resolution time

### Step 4: Generate Narrative

Use AI prompt:

```
Create QBR for {account_name} with:
- Usage: {usage_data}
- CRM: {crm_data}
- Conversations: {insights}
- Support: {tickets}

Generate:
1. Executive Summary (3-4 bullets)
2. Usage Highlights (metrics + trend)
3. Use Cases Implemented (with outcomes)
4. Support Summary
5. Forward-Looking Recommendations
6. Expansion Opportunities

Include:
- Exact numbers (not approximations)
- Source citations
- Customer quotes from Gong
```

### Step 5: Generate Charts

Create visualizations:
- Usage trend line
- Feature adoption bar chart
- User activity distribution

### Step 6: Populate Template

Fill slides with content + charts.

### Step 7: Deliver

- Post to Slack channel
- Email to account team
- Link in CRM note

## Quality Checklist

- [ ] Every metric has a source citation
- [ ] Numbers are exact (not "approximately")
- [ ] At least one customer quote included
- [ ] Charts are properly formatted
- [ ] Forward-looking recommendations are actionable
- [ ] Expansion opportunities are specific

## Time Savings

| Task | Before | After |
|------|--------|-------|
| Data Pull | 75 min | 2 min |
| Analysis | 60 min | 3 min |
| Narrative | 90 min | 2 min |
| Slides | 120 min | 2 min |
| Review | 30 min | 10 min |
| **Total** | **6 hrs** | **10 min** |
