# Citations & Sources

> Key documentation and resources for GTM Engineering at Opulentia.

---

## 📚 Primary Sources

### docs.opulentia.ai
**Category:** Internal Documentation Hub

| Resource | Description | Last Updated |
|----------|-------------|--------------|
| API Reference | REST API endpoints for agent integration | Current |
| Integration Guides | Step-by-step setup for each tool | Current |
| Best Practices | GTM workflow standards and patterns | Current |
| Troubleshooting | Common issues and resolutions | Current |

**Access:** Internal team and authorized agents

**Usage for Agents:**
- Reference for all Opulentia-specific workflows
- API authentication and rate limits
- Data models and schemas
- Error handling conventions

---

### use.opulentia.ai
**Category:** User Documentation / Knowledge Base

| Resource | Description | Last Updated |
|----------|-------------|--------------|
| Getting Started | Quick-start guides for new users | Current |
| Feature Documentation | How-to guides for each capability | Current |
| Release Notes | Changelog and new features | Current |
| FAQ | Frequently asked questions | Current |

**Access:** Public-facing documentation

**Usage for Agents:**
- Generate user-facing help content
- Reference feature explanations
- Pull latest product updates
- Surface relevant FAQs to users

---

## 🔧 Tool-Specific Documentation

### Attio
- **API Docs:** https://developers.attio.com
- **Webhook Reference:** https://developers.attio.com/docs/webhooks
- **Key User:** `hello@opulentia.ai`

### Slack
- **API Docs:** https://api.slack.com
- **Webhook Guide:** https://api.slack.com/messaging/webhooks
- **Block Kit Builder:** https://app.slack.com/block-kit-builder

### Outlook / Microsoft Graph
- **Graph API:** https://learn.microsoft.com/en-us/graph/api/overview
- **Mail API:** https://learn.microsoft.com/en-us/graph/api/resources/mail-api-overview
- **Calendar API:** https://learn.microsoft.com/en-us/graph/api/resources/calendar
- **Key User:** `hello@opulentia.ai`

### LinkedIn Sales Navigator
- **API Docs:** https://learn.microsoft.com/en-us/linkedin/shared/sales-navigator
- **Partner API:** https://developer.linkedin.com/docs/v2/sales-navigator-api

### Apollo
- **API Docs:** https://apolloio.github.io/apollo-api-docs
- **Enrichment API:** https://apolloio.github.io/apollo-api-docs/#people-enrichment

### AmpleMarkets
- **Help Center:** https://help.amplemarkets.com
- **API Docs:** Available upon request

### Happystance
- **Docs:** https://docs.happystance.ai (or internal equivalent)
- **Integration Guide:** Available via docs.opulentia.ai

---

## 📖 Citation Format

When referencing sources in agent outputs, use this format:

```
[Source: Tool Name - Page Title]
URL: https://...

Key points:
- Point 1
- Point 2
- Point 3
```

### Example Citation

```
[Source: Attio API - List Objects]
URL: https://developers.attio.com/docs/list-objects

Key points:
- Returns paginated list of objects
- Supports filtering by attributes
- Includes created_at and updated_at timestamps
```

---

## 🔄 Keeping Sources Current

### Update Cadence
| Source | Update Frequency | Responsible |
|--------|------------------|-------------|
| docs.opulentia.ai | As needed | Engineering Team |
| use.opulentia.ai | As needed | Product Team |
| External tool docs | Quarterly review | GTM Ops Team |

### Source Verification
1. Check `Last Updated` dates on external documentation
2. Validate API endpoints before use
3. Report broken links to GTM Ops Team
4. Update this document when sources change

---

## 📋 Quick Reference

### Opulentia Sources
```
docs.opulentia.ai     → Internal docs, API reference, integration guides
use.opulentia.ai      → User-facing docs, getting started, feature guides
```

### External Sources
```
developers.attio.com           → Attio API documentation
api.slack.com                  → Slack API reference
learn.microsoft.com/graph      → Outlook/Calendar API (Microsoft Graph)
developer.linkedin.com         → LinkedIn Sales Navigator API
apolloio.github.io             → Apollo API documentation
```

---

## 🔗 Related Documents

- [Tech Stack](./tech-stack.md) - Full tool inventory and usage
- [Data Sources](./data-sources/) - Integration-specific documentation
- [Playbooks](./playbooks/) - Step-by-step execution guides

---

## 📝 Notes for Agents

1. **Always cite sources** when providing information to users
2. **Verify URLs** before sharing with users
3. **Prefer internal sources** (docs.opulentia.ai) when available
4. **Cross-reference** multiple sources for critical information
5. **Report outdated sources** to maintain accuracy
