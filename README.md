# GTM Engineering for Opulentia

> The definitive guide for AI agents to execute world-class go-to-market engineering.

## What is GTM Engineering?

GTM Engineering is the systematic application of automation, data integration, and AI to scale go-to-market motions that traditionally required manual human effort. It encompasses:

- **Sales Demo Automation**: Creating personalized, data-rich demos at scale
- **Deck/Content Generation**: Automated QBRs, pitch decks, and customer materials
- **Prospect Enrichment**: Multi-source data aggregation and signal detection
- **Customer Success Automation**: Usage analytics, health scoring, and renewal playbooks
- **Revenue Intelligence**: Conversation analysis, deal coaching, and forecasting

## Why This Repository Exists

Just as cursor-slidev guides agents on programmatic slide creation, this repository guides agents on **the best way to execute GTM engineering for Opulentia**. An agent reading these rules can immediately:

1. Understand the GTM philosophy and principles
2. Identify the right tasks to execute based on business context
3. Follow proven playbooks with step-by-step instructions
4. Leverage templates for common outputs
5. Integrate with the right data sources and tools

## Core Philosophy

### 1. **Data Aggregation is the Foundation**
> "The system works because it solves the two hardest problems in deck creation: aggregating scattered data and transforming that data into compelling narrative content." — Clay

GTM engineering succeeds when it connects data that normally stays siloed:
- Product usage data (Snowflake, BigQuery, Amplitude, Mixpanel)
- CRM context (Salesforce, HubSpot)
- Conversation intelligence (Gong, Chorus)
- Marketing automation (Customer.io, Iterable)
- Support tickets (Zendesk, Linear)
- Public signals (LinkedIn, news, hiring)

### 2. **Personalization at Scale, Not Templates**
Templates provide structure but not storytelling. The goal is:
- Each prospect/customer gets materials tailored to their context
- Automation handles the 90% — humans review the last 10%
- Quality doesn't degrade under deadline pressure

### 3. **Product-Led GTM**
> "For strategic customers, you really need to resonate with their unique use cases. By showing them what their business will look like when they start using [your product]." — Amplitude

The most powerful GTM motion shows prospects exactly what success looks like:
- Custom demo environments with their branding and use cases
- Simulated user journeys that produce real analytics
- Product usage patterns from similar customers

### 4. **From Push to Pull**
> "It was a push initially and now it's just a pull. Everyone's just asking for more." — Amplitude

Build GTM capabilities so valuable that sales/CS teams pull for more:
- Start with a high-impact use case (e.g., automated QBRs)
- Prove ROI with a small group
- Scale based on demand

## Repository Structure

```
gtm-engineering/
├── .cursor/rules/           # Agent instruction files
│   ├── gtm-overview.mdc     # Core GTM philosophy and principles
│   ├── demo-automation.mdc  # Sales demo automation playbook
│   ├── deck-generation.mdc  # Automated deck/content creation
│   ├── prospect-enrichment.mdc # Signal detection and enrichment
│   ├── customer-success.mdc # CS automation and health scoring
│   └── revenue-intelligence.mdc # Conversation/deal intelligence
├── playbooks/               # Step-by-step execution guides
│   ├── qbr-generation.md    # Automated QBR creation
│   ├── sales-demo.md        # Personalized demo creation
│   ├── executive-briefing.md # Strategic account briefings
│   └── expansion-play.md    # Expansion opportunity detection
├── templates/               # Output templates
│   ├── qbr-slide-deck.md    # QBR structure template
│   ├── sales-one-pager.md   # Sales one-pager template
│   └── health-score-card.md # Customer health dashboard
├── examples/                # Real-world examples
│   └── clay-automation.md   # Clay's deck automation case study
├── data-sources/            # Integration documentation
│   ├── product-analytics.md # Amplitude, Mixpanel, etc.
│   ├── crm.md               # Salesforce, HubSpot
│   └── conversation-intel.md # Gong, Chorus
├── tech-stack.md            # GTM tool inventory (Attio, Slack, Apollo, etc.)
├── citations.md             # Documentation sources and citation guides
└── README.md                # This file
```

## How to Use This Repository

### For AI Agents
1. Read `.cursor/rules/gtm-overview.mdc` for core philosophy
2. Identify the task type (demo, deck, enrichment, etc.)
3. Load the corresponding rule file for detailed instructions
4. Follow the playbook for step-by-step execution
5. Use templates for output formatting

### For Humans
1. Review the playbooks to understand what's possible
2. Customize rules for your specific context
3. Add your own templates and examples
4. Use as a reference when building GTM automation

## Key Metrics to Track

| GTM Task | Before Automation | After Automation | Improvement |
|----------|-------------------|------------------|-------------|
| QBR Creation | 6 hours/account | 10 minutes review | 36x faster |
| Demo Prep | 2+ hours | On-demand | Instant |
| Enrichment | Manual research | Automated pipeline | Continuous |
| Briefing Generation | 4+ hours | Scheduled/automated | Always current |

## Resources & Inspiration

### Opulentia Sources
- **docs.opulentia.ai** — Internal documentation, API reference, integration guides
- **use.opulentia.ai** — User-facing docs, getting started, feature guides

### Must-Read Sources
- **Founding Sales** (foundingsales.com) — Founder-led sales playbook
- **High Growth Handbook** (growth.eladgil.com) — Product marketing and scaling
- **The GTM Engineering Blog** (thegtme.com) — Clay's automation insights
- **Browserbase Blog** — Amplitude's demo transformation

### Case Studies
- Clay: 6 hours → 10 minutes for QBRs
- Amplitude: 40+ custom demos, $10M+ influenced pipeline
- See `examples/` for detailed breakdowns

## Contributing

This repository is designed to be extended. Add:
- New playbooks for emerging GTM tasks
- Templates for your specific use cases
- Integration documentation for new data sources
- Examples from your own automation work

---

*GTM Engineering: Automate the manual, personalize at scale, prove with data.*
