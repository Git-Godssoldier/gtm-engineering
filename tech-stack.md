# GTM Tech Stack

> Core tools powering Opulentia's Go-to-Market engineering workflows.

---

## 📊 CRM & Data Management

### Attio ⭐ Key User: `hello@opulentia.ai`
**Category:** Modern CRM / Relationship Intelligence

| Capability | Use Case |
|------------|----------|
| Object Store | Flexible data models for accounts, deals, people |
| Views | Custom pipelines and lists for GTM workflows |
| Automations | Trigger-based actions and integrations |
| API | RESTful + webhook support for agent automation |

**Agent Integration:**
- Read/write records via Attio API
- Automate deal stage updates
- Sync with enrichment tools (Apollo, Clay)

**Status:** ✅ Active — Primary CRM for Opulentia GTM operations

---

## 📧 Communication & Outreach

### Slack
**Category:** Team Communication / Alerts

| Capability | Use Case |
|------------|----------|
| Channels | GTM team coordination, deal alerts |
| Webhooks | Automated notifications from agents |
| Threads | Contextual discussions on accounts/deals |
| Apps | Integration with CRM, calendar, and tools |

**Agent Integration:**
- Send alerts on key events (deal closed, meeting booked)
- Post daily standups or pipeline summaries
- Create threads for account research discussions

**Status:** ✅ Active — Team coordination hub

---

### Outlook ⭐ Key User: `hello@opulentia.ai`
**Category:** Email / Calendar / Scheduling

| Capability | Use Case |
|------------|----------|
| Email | Customer communication and follow-ups |
| Calendar | Meeting scheduling and availability |
| Contacts | Prospect and customer relationship data |
| Rules | Automated email routing and responses |

**Agent Integration:**
- Parse inbound emails for intent signals
- Draft and send follow-up sequences
- Schedule meetings via calendar API
- Track email engagement metrics

**Status:** ✅ Active — Primary email and calendar platform

---

## 🔍 Enrichment & Prospecting

### LinkedIn Sales Navigator
**Category:** Prospecting / Relationship Intelligence

| Capability | Use Case |
|------------|----------|
| Advanced Search | Target accounts by criteria (ICP matching) |
| Lead Recommendations | AI-suggested prospects |
| InMail | Direct outreach to decision-makers |
| Account Mapping | Organizational hierarchies and relationships |

**Agent Integration:**
- Identify decision-makers at target accounts
- Research account activity and signals
- Map organizational structures for outreach strategy

**Status:** ✅ Active — Premium prospecting tool

---

### Apollo
**Category:** B2B Contact Database / Enrichment

| Capability | Use Case |
|------------|----------|
| Contact Database | 200M+ B2B contacts with verified emails |
| Company Data | Firmographics, technographics, intent data |
| Sequences | Automated outbound email campaigns |
| Enrichment | Real-time data enrichment via API |

**Agent Integration:**
- Enrich Attio records with contact data
- Build targeted prospect lists by ICP
- Verify email addresses before outreach
- Sync engagement data back to CRM

**Status:** ✅ Active — Primary enrichment source

---

### AmpleMarkets
**Category:** Sales Engagement / Multi-Channel Outreach

| Capability | Use Case |
|------------|----------|
| Email Sequences | Automated multi-touch campaigns |
| LinkedIn Automation | Connection requests and messaging |
| Task Management | Follow-up reminders and prioritization |
| Analytics | Campaign performance tracking |

**Agent Integration:**
- Orchestrate multi-channel outreach sequences
- Personalize messages at scale using AI
- Track response rates and optimize timing
- Sync activity to CRM for reporting

**Status:** ✅ Active — Sales engagement orchestration

---

## 🤖 AI & Automation

### Happystance
**Category:** AI Meeting Assistant / Conversation Intelligence

| Capability | Use Case |
|------------|----------|
| Transcription | Automatic meeting notes and summaries |
| Action Items | Extracted follow-ups and tasks |
| CRM Sync | Auto-log calls to CRM records |
| Search | Query across all conversations |

**Agent Integration:**
- Parse meeting transcripts for insights
- Extract action items and assign owners
- Update CRM records with conversation context
- Generate follow-up emails based on discussions

**Status:** ✅ Active — Meeting intelligence layer

---

## 📋 Stack Summary

| Tool | Category | Key User | Status |
|------|----------|----------|--------|
| Attio | CRM | `hello@opulentia.ai` ⭐ | Active |
| Slack | Communication | Team | Active |
| Outlook | Email/Calendar | `hello@opulentia.ai` ⭐ | Active |
| LinkedIn Sales Navigator | Prospecting | GTM Team | Active |
| Apollo | Enrichment | GTM Team | Active |
| AmpleMarkets | Sales Engagement | GTM Team | Active |
| Happystance | AI Assistant | GTM Team | Active |

---

## 🔗 Integration Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                     AGENT ORCHESTRATION                      │
└─────────────────────────────────────────────────────────────┘
                              │
        ┌─────────────────────┼─────────────────────┐
        ▼                     ▼                     ▼
   ┌─────────┐         ┌──────────┐         ┌─────────────┐
   │  Attio  │◄───────►│ Happystance │◄──────►│   Outlook   │
   │   CRM   │         │   (AI)      │        │ Email/Cal   │
   └─────────┘         └──────────┘         └─────────────┘
        ▲                     │                     │
        │                     │                     │
        ▼                     ▼                     ▼
   ┌─────────┐         ┌──────────┐         ┌─────────────┐
   │ Apollo  │         │  Slack   │         │ AmpleMarkets│
   │Enrich   │         │  Alerts  │         │ Engagement  │
   └─────────┘         └──────────┘         └─────────────┘
        ▲                                          │
        │                                          │
        └──────────────────┬───────────────────────┘
                           ▼
                  ┌────────────────────┐
                  │ LinkedIn Sales Nav │
                  │   Prospecting      │
                  └────────────────────┘
```

---

## 📝 Usage Notes

1. **Attio is the single source of truth** for all GTM data
2. **Happystance bridges meetings → CRM** with automatic logging
3. **Apollo + LinkedIn** provide enrichment for all prospecting
4. **AmpleMarkets** orchestrates outbound across channels
5. **Slack** is the notification layer for all agent actions

For integration details, see the [Citations](./citations.md) document.
