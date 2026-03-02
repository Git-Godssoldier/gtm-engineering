# Case Study & Testimonial Frameworks

> Extracted and synthesized from ai-marketing-claude-code-skills — case-study-builder, testimonial-collector

---

## Part 1: Case Study Builder

### Context Loading Gates

**Before generating anything, collect all 8 fields:**

| Field | What to Collect |
|---|---|
| 1. Client | Industry, company size/stage, named or anonymized? |
| 2. Before | What was broken or painful? Any numbers? |
| 3. Actions | What did you specifically do? Scope, timeline, role |
| 4. After | **REQUIRED: at least one specific number** |
| 5. Timeline | How long to achieve the result? |
| 6. Quote | Direct client quote if available |
| 7. Naming | Can we name the client, or must we anonymize? |
| 8. Use case | Where will this be used? (proposals / website / LinkedIn) |

**Outcome Extraction Protocol — enforced:**

If the user says "results were good" or "things improved," stop and ask:
> "I need at least one number to make this credible. Pick one:
> - Revenue change (e.g., 'closed 3 new clients worth $15K')
> - Time saved (e.g., 'cut from 10 hours to 2 hours/week')
> - Lead volume (e.g., 'went from 0 to 5 inbound leads/month')
> - Rough estimate is fine — it doesn't have to be exact."

**Do not draft until you have at least one number.**

---

### Phase 1: Situation Analysis

Before drafting, reason through:

1. **Result strength:** Is the outcome a Tier 1 (hard metric), Tier 2 (soft metric), or Tier 3 (proxy)? This determines how confident the language should be.
2. **Hero check:** Is the story told from the client's perspective, or yours? Client = hero, you = guide.
3. **Tension check:** What made this hard? Without a challenge, there's no story — just a list.
4. **Format match:** Which use case did they specify? That determines which format to optimize.

**Tier system for results language:**

| Tier | Type | Example | Language |
|---|---|---|---|
| 1 | Hard metric | "Revenue +40%" | State directly |
| 2 | Soft metric | "Team finally aligned" | "For the first time in years..." |
| 3 | Proxy metric | "Enabled Series A close" | "Contributed to..." |
| 4 | Directional | "Noticeable improvement" | "Significant improvement in..." |

---

### Phase 2: The Hero Principle

**The client is the hero. You are the guide.**

Before writing, flip the framing:

❌ Wrong: "I built a content system that generated leads."
✅ Right: "Sarah went from scrambling to fill her pipeline to getting 3 inbound inquiries per week — all from a content system we built in 6 weeks."

Every format should be written from what the CLIENT experienced, not what YOU delivered.

---

### Phase 3: Three Formats

#### Format 1: Two-Liner (Proposals & Bios)

**Formula:** `[What was done] + [scale/scope] + [for who] + [result or timeframe]`

```
[Strong action verb] [what was delivered] for [specific client descriptor].
[Outcome metric] in [timeframe].
```

**Example:**
> Built a full content system for a Series B SaaS founder with no marketing team.
> 0 to 3 inbound leads/week in 6 weeks.

---

#### Format 2: Story Version (LinkedIn & Sales Calls)

**Structure — 4 paragraphs, 150–250 words:**

```
**Set the scene:** [Their situation when you arrived — 2-3 sentences with stakes]

**Show the complexity:** [What made this hard — 2-3 sentences]

**What happened:** [Specific actions taken — no feature lists, just moves]

**What changed:** [Outcome — the number + the transformation]
```

---

#### Format 3: Full Case Study (Website & Portfolio)

```markdown
# Case Study: [Client Name or Descriptor]

## The Challenge
[2-3 paragraphs: situation, stakes, what wasn't working]

## The Approach
[Phases or steps — what happened and in what order]

## The Results
[Metrics, before/after comparison, named outcomes]

## Key Details
- Client: [Named or "A [descriptor] company"]
- Industry: [Sector]
- Timeline: [Duration]
- Scope: [What was delivered]

## What Made This Different
[Unique angle, unexpected obstacle, or pivotal insight]

## Client Quote
> "[Testimonial — or placeholder if not yet collected]"
> — [Name], [Title]
```

---

### Phase 4: Self-Critique Pass (REQUIRED)

**Two-liner:**
- [ ] Does it have a specific number? (Not "improved results" — a real metric)
- [ ] Is it 2 sentences or fewer?
- [ ] Would someone scanning a proposal stop and read it?

**Story version:**
- [ ] Is the client the hero (not the author)?
- [ ] Is there genuine tension — something that made this hard?
- [ ] Does the closing paragraph include the key metric?

**Full case study:**
- [ ] Does the Results section lead with numbers?
- [ ] Is the Challenge section specific enough that a similar prospect recognizes their situation?
- [ ] Is the client quote (or placeholder) present?

---

### Phase 5: Distribution Plan

| Format | Best locations | When to use |
|---|---|---|
| Two-liner | Proposals, email bios, LinkedIn About section | Any sales context |
| Story | LinkedIn post, podcast intros, sales call opener | Weekly content |
| Full case study | Website portfolio page, PDF download, RFP response | Late-stage buyer research |

---

## Part 2: Testimonial Collector

### Context Loading Gates

**Before proceeding, gather:**
- [ ] Client name, company, and industry
- [ ] Project type and specific deliverables
- [ ] Key results — push for at least one number ("even a rough estimate")
- [ ] Desired output format (short quote / medium paragraph / full narrative)
- [ ] Urgency (this week vs. building a library)

If results are vague (e.g., "things improved"), **stop and ask:**
> "Can you name one specific number — even a rough estimate? That's what makes a testimonial credible and usable."

---

### Quality Scoring Framework

Score the raw testimonial content before drafting:

| Dimension | Score 1 | Score 3 | Score 5 |
|---|---|---|---|
| **Specificity** | No details | Vague references | Specific named result |
| **Measurability** | "It was great" | "Noticeable improvement" | "40% increase in leads" |
| **Authentic Voice** | Sounds like ad copy | Slightly stilted | Reads exactly how a person talks |
| **Length** | Too short (no context) | Decent but thin | Enough for all 3 formats |

**Scoring rule:**
- 4+ on all 4 dimensions → ready to use
- ≤2 on any dimension → apply iteration protocol before delivering

---

### The Ask Templates

**Direct Ask:**
```
Subject: Quick favor (30 seconds)

Hey [Name],

Loved working on [project] with you — especially seeing [specific result].

Would you be open to sharing a quick testimonial I could use on my site?

No pressure. If yes, I can either:
A) Send you 3 questions to answer
B) Write a draft for you to approve/edit

Whatever's easier.
```

**Question Route:**
```
3 quick questions:
1. What was the situation before we worked together?
2. What changed or improved?
3. Would you recommend this to others? Why?
```

---

### Format Production

#### Short Format (2-liner)
```
"[One punchy outcome sentence — lead with the result]"
— [Name], [Title] at [Company]
```
**Use for:** Homepage, LinkedIn featured section, proposal proof points

#### Medium Format (2-3 sentences)
```
"[Problem or situation]. [What changed]. [Recommendation or result]."
— [Name], [Title] at [Company]
```
**Use for:** Services page, sales decks, email sequences

#### Long Format (Full narrative)
Structure:
1. Context paragraph (2-3 sentences on the situation)
2. Transformation paragraph (what happened during the engagement)
3. Results paragraph (outcomes, numbers, named wins)
4. Closing recommendation sentence

**Use for:** Case study pages, downloadable PDFs, high-trust sales assets

---

### Iteration Protocol

If the received testimonial scores ≤2 on any dimension, send this gentle follow-up:
```
"Thanks so much — this is great. One small ask: could you add one specific 
number or outcome? Even rough ('saved us about 5 hours a week') makes it 
much more compelling for other clients. Totally optional, but makes a real difference."
```

If a second request still yields nothing specific: use Tier 3 proxy language:
> "noticeable improvement in [area]" or "process now runs without manual oversight"

---

### Output Structure

```markdown
## Testimonial: [Client Name] — [Date]

### Quality Assessment
- Specificity: [X/5]
- Measurability: [X/5]
- Authentic Voice: [X/5]
- Length: [X/5]
- **Total: [X/20] — [Ready to use / Needs iteration]**

### Short Format (2-liner)
"[Quote]"
— [Name], [Title], [Company]

### Medium Format
"[Quote]"
— [Name], [Title], [Company]

### Long Format
[Full narrative]

### Placement Recommendation
[Where to use each format]

### Next Step
[Iteration note OR cross-reference to case-study-builder]
```

---

*Framework extracted from ai-marketing-claude-code-skills by Brian Wagner*