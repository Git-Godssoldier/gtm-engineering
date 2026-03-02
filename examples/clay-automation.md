# Clay Deck Automation Case Study

## Company Background

Clay is a data enrichment and automation platform. Their CS team manages 15+ accounts and previously spent **90+ hours per quarter** on deck creation.

## The Problem

Before automation, QBR creation took **6 hours per account**:
- 45 min: Pull product usage from Snowflake
- 30 min: Review CRM records in Salesforce
- 60 min: Analyze Gong transcripts
- 90 min: Build narrative from data
- 2 hrs: Create slides from scratch
- 30 min: Review and finalize

## The Solution

Automated deck generation that aggregates data from multiple sources and generates presentations in minutes.

### Architecture

```
Data Sources:
├── Snowflake (product usage)
├── Salesforce (CRM)
├── Gong (conversations)
└── Custom APIs
        ↓
Aggregation Layer:
├── Unified query interface
├── Data normalization
└── Insight extraction (AI)
        ↓
Generation Layer:
├── Narrative generation (AI)
├── Chart creation
└── Template population
        ↓
Delivery:
├── Slack notification
├── PPTX file
└── Editable link
```

## Results

| Metric | Before | After | Improvement |
|--------|--------|-------|-------------|
| Time per QBR | 6 hours | 10 min | 36x faster |
| Quality | Variable | Consistent | Higher |
| Coverage | Enterprise only | All accounts | 100% |
| CS time on decks | 90+ hrs/qtr | 15 hrs/qtr | 6x reduction |

## Key Learnings

1. **Data aggregation is the foundation** - Connect siloed data first
2. **90% complete is the goal** - Let humans handle final 10%
3. **Quality at scale** - Smaller accounts now get enterprise-quality QBRs
4. **Pull vs. Push** - CS team now requests more automation

## Source

- [How Clay Automates Deck Creation](https://thegtme.com/p/how-clay-automates-deck-creation)
