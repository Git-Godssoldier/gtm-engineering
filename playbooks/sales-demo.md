# Sales Demo Automation Playbook

## Overview

Create personalized demo environments for strategic prospects.

## Prerequisites

- Browserbase account
- Stagehand SDK
- AI coding tool (Claude Code, Cursor)
- Demo template framework

## Step-by-Step Process

### Step 1: Receive Request

Sales engineer submits via Slack:
```
/demo [prospect_name] [industry] [key_use_cases]
```

### Step 2: Run Enrichment

Automatically pull:
- Firmographic data (company size, industry)
- Technographic signals (tools they use)
- Recent news (announcements, funding)
- Hiring patterns (job postings)

### Step 3: Identify Use Cases

Match enrichment to product capabilities:
- Industry-specific features
- Integration opportunities
- ROI-relevant use cases

### Step 4: Generate Demo Environment

Build custom website matching prospect's product:

```javascript
// Prompt for AI coding tool
Build a ${industry} website for ${prospect_name}
that demonstrates ${use_cases}.
Style: ${prospect_brand_colors}
User journeys: ${journeys}
```

### Step 5: Simulate User Behavior

Run browser automation:

```javascript
// Stagehand script
import { Stagehand } from "@browserbasehq/stagehand";

async function simulateJourneys(demoUrl) {
  const stagehand = new Stagehand();
  await stagehand.init();
  
  // Journey 1: Browse products
  await stagehand.page.goto(demoUrl);
  await stagehand.act("browse product catalog");
  await stagehand.act("add item to cart");
  
  // Journey 2: Complete purchase
  await stagehand.act("go to checkout");
  await stagehand.act("fill shipping form");
  await stagehand.act("complete purchase");
  
  return stagehand.getEvents();
}
```

### Step 6: Inject Data

Add custom logic between actions:
- Track events
- Generate sessions
- Create user segments
- Enable AI insights

### Step 7: Deliver to Sales

Provide:
- Demo URL
- Key journeys to highlight
- Talking points
- ROI estimates
- Similar customer proof points

## Metrics to Track

- Demos created per month
- Time to generate demo
- Pipeline influenced
- Sales engineer satisfaction

## Example: E-commerce Demo

**Prospect:** Fashion retailer

**Demo Environment:**
- Mock clothing store
- Product browsing journey
- Cart abandonment flow
- Loyalty program signup

**Simulated Data:**
- 500+ users
- 2000+ events
- 50+ sessions
- Conversion funnel

## Common Patterns by Industry

| Industry | Demo Type | Key Journeys |
|----------|-----------|--------------|
| E-commerce | Online store | Browse, cart, checkout |
| B2B SaaS | Dashboard | Login, feature use, settings |
| Healthcare | Patient portal | Booking, records, messaging |
| Finance | Banking app | Transfers, statements, alerts |
