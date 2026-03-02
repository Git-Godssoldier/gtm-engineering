# Cold Outreach Sequence Framework

> Extracted and synthesized from ai-marketing-claude-code-skills — cold-outreach-sequence

---

## Core Philosophy

The word "cold" is the problem. Spray-and-pray templates don't work. 10 minutes of research + a specific reference = not cold anymore. This framework builds personalized outreach that feels warm.

---

## Research & Signal Assessment

### Before Writing Any Message — Run Research First

```bash
web_search('[Company] [Founder/Name] news 2026')
web_search('[Company] funding recent')
web_search('[Person name] [Company] LinkedIn')
```

### Signal Types (Ranked by Strength)

| Rank | Signal Type | Message Strength |
|------|-------------|------------------|
| 1 | Recent news event (funding, launch, hire, press) | Strongest |
| 2 | Recent LinkedIn post activity | Strong |
| 3 | Company stage/growth data | Medium |
| 4 | Role + industry awareness only | Weak (Tier 3) |

### Personalization Tier Assignment

| Research Result | Tier | Approach |
|---|---|---|
| Named signal (news + post + context) | Tier 1 | Fully custom, reference signal in every message |
| Company info + role context | Tier 2 | Template + personalized opener |
| No signals found | Tier 3 | Volume template, minimal customization |

**Constraint:** Do not write a Tier 1 message without a named specific signal from research. If search yields 0 signals, default to Tier 3 and say so explicitly.

---

## Sequence Templates

### 1. Connection Request (LinkedIn) — 300 chars max

**Formula:** `[Specific observation from research] + [Simple reason to connect]`

**Rules:**
- No pitching
- Prove you did research (name the signal)
- One sentence, conversational
- Never "I'd love to pick your brain"

**By signal type:**

```
Recent funding: "Congrats on the Series A — the [investor] backing is a smart signal. Would love to connect."

Recent post: "Your post on [specific topic] resonated — been thinking the same thing. Happy to connect."

News/launch: "Saw the [product] launch — [specific detail] is smart positioning. Would love to connect."
```

---

### 2. First Message (After Accept — Wait 24-48 Hours)

**Formula:** `[Thanks] + [Bridge to relevance] + [Light value] + [Soft question]`

**Template:**
```
Thanks for connecting. I work with [ICP description] on [specific outcome].

Curious — is [relevant function] something you own directly at [Company], 
or is that still founder-led?

Happy to share what I'm seeing work at similar-stage companies either way.
```

---

### 3. Follow-Up #1 (Day 7)

**Formula:** `[Light nudge] + [New signal or angle] + [Easy out]`

**Constraint:** Do NOT write "following up" with nothing new. Add one new piece:
- A relevant article or trend
- A related insight you recently had
- A connection to something they posted

**Template:**
```
Bumping this up — came across [specific article/trend/insight] and 
thought of your situation at [Company].

[One sentence on why it's relevant to them.]

Happy to share more if useful. If not, no worries.
```

---

### 4. Follow-Up #2 (Day 14)

Shift to email if LinkedIn hasn't converted, or try a different angle.

**Subject line options:**
- "[Company]'s [function] as you scale"
- "Saw your [post/news] — quick thought"
- "Question about [specific thing they're doing]"

**Email structure:**
```
[1-line hook tied to their specific situation]

[2-3 sentences: why you're reaching out + one proof point]

[Soft CTA — 1 sentence]
```

---

### 5. Break-Up Message (Day 21)

```
I'll assume timing isn't right — totally get it. 

If [relevant pain point] becomes a priority down the road, happy to reconnect. 
Best of luck with [specific thing they're working on based on research].
```

**Post-break-up action:** Add to 6-month re-engagement list with a resurface date.

---

## Self-Critique Checklist (REQUIRED)

After generating the full sequence, evaluate:

- [ ] Does every message reference the specific signal from research, or are they generic?
- [ ] Is the connection request under 300 characters?
- [ ] Does the first message ask a question (invite dialogue) rather than pitch?
- [ ] Does follow-up #1 add something genuinely new, or is it just "following up"?
- [ ] Does the break-up message reference something specific about their situation?
- [ ] Did I correctly assign the personalization tier, or am I over-personalizing a Tier 3 prospect?

---

## Pipeline Tracking Table

```
| Prospect | Company | Platform | Tier | Sent Date | Response | Stage | Next Action | Resurface Date |
|---|---|---|---|---|---|---|---|---|
| [Name] | [Co] | LinkedIn | 1 | [date] | — | Connection sent | Wait 24-48h | — |
| [Name] | [Co] | Email | 2 | [date] | — | First email sent | Follow-up Day 7 | — |
```

---

## Iteration Protocol

After each response (or non-response), ask:
- Did the connection request get accepted? If low acceptance rate → revise the observation line
- Did the first message get a reply? If no → was the question soft enough, or did it feel like a pitch?
- Did follow-ups get ignored? If yes → try a different angle or acknowledge the silence directly

---

## Output Structure Template

```markdown
## Outreach Sequence: [Prospect Name] — [Date]

### Research Summary
- Signal type: [news / post / company info / none]
- Signal found: "[Specific detail]"
- Personalization tier: [1/2/3]
- Source: [URL or platform]

### Sequence

**Connection Request (LinkedIn):**
[Text — max 300 chars]

**First Message (Day 1-2 after accept):**
[Text]

**Follow-Up #1 (Day 7):**
[Text]

**Follow-Up #2 (Day 14):**
Platform: [LinkedIn / Email]
Subject: [if email]
[Text]

**Break-Up (Day 21):**
[Text]

### Pipeline Entry
| Prospect | Company | Platform | Tier | Stage | Next Action | Resurface Date |
|---|---|---|---|---|---|--- |
| [Name] | [Co] | [Platform] | [Tier] | Connection sent | Wait 24-48h | — |

### Self-Critique Notes
[Any issues flagged + revisions made]
```

---

*Framework extracted from ai-marketing-claude-code-skills by Brian Wagner*