# Opulentia Outbound Sequencing Strategy — Assessment & Enhancement

> Assessment of current playbook content against proven frameworks, with critiques and enhancements for improved performance

---

## Executive Summary

Your outbound playbook is **well-structured and strategically sound** — you have clear ICP definitions, strong messaging pillars, and a logical 8-touch cadence. However, several enhancements drawn from our sequencing frameworks can significantly improve response rates, personalization quality, and operational discipline.

This document provides:
1. **Critiques** — Specific gaps or weaknesses in the current playbook
2. **Enhancements** — Proven frameworks and tactics to address each gap
3. **Implementation recommendations** — Where to apply changes

---

## Critique #1: Signal Research Protocol Is Implicit, Not Enforced

### The Gap
Your playbook references signals ("Noticed your team just posted a Head of AI Operations role") but provides **no research protocol** for finding those signals before outreach. Without structured research, reps may default to generic observations or miss the strongest signals.

### Our Framework: Research-First Approach

```bash
# Before writing ANY message, run:
web_search('[Company] [Founder/Name] news 2026')
web_search('[Company] funding recent')
web_search('[Person name] [Company] LinkedIn')
```

### Signal Strength Ranking (Tier 1/2/3)

| Rank | Signal Type | Message Strength |
|------|-------------|------------------|
| 1 | **Recent news event** (funding, launch, hire, press) | Strongest |
| 2 | **Recent LinkedIn post activity** | Strong |
| 3 | Company stage/growth data | Medium |
| 4 | Role + industry awareness only | Weak (Tier 3) |

### Personalization Tier Assignment

| Research Result | Tier | Approach |
|---|---|---|
| Named signal (news + post + context) | **Tier 1** | Fully custom, reference signal in every message |
| Company info + role context | **Tier 2** | Template + personalized opener |
| No signals found | **Tier 3** | Volume template, minimal customization |

**Constraint:** Do not write a Tier 1 message without a named specific signal from research. If search yields 0 signals, default to Tier 3 and say so explicitly.

### Enhancement: Add to Your Playbook

> **Before any outreach sequence, reps must complete research and assign a tier.** This determines message customization level and prevents over-personalizing prospects who warrant a template approach.

---

## Critique #2: LinkedIn Connection Notes Lack Structure

### The Gap
Your playbook mentions "LinkedIn Connect with a short personalized note" but provides **no formula, character limit, or examples** for what makes a good connection note. Connection notes that pitch get rejected; notes that show research get accepted.

### Our Framework: 300-Character Connection Formula

**Formula:** `[Specific observation from research] + [Simple reason to connect]`

**Rules:**
- No pitching
- Prove you did research (name the signal)
- One sentence, conversational
- Never "I'd love to pick your brain"

### Examples by Signal Type

```
Recent funding: "Congrats on the Series A — the [investor] backing is a smart signal. Would love to connect."

Recent post: "Your post on [specific topic] resonated — been thinking the same thing. Happy to connect."

News/launch: "Saw the [product] launch — [specific detail] is smart positioning. Would love to connect."
```

### Enhancement: Add LinkedIn Connection Framework

**Target:** 25–40% accept rate. If below this, the observation line needs work.

---

## Critique #3: Email Templates Are Strong But Could Use Signal Tier Adaptations

### The Gap
Your email variants (Enterprise vs. SMB) are well-crafted, but they apply the same structure regardless of how strong the signal is. A Tier 1 signal (specific news) warrants different framing than a Tier 3 signal (role-based assumption).

### Our Framework: Tier-Based Adaptation

**Tier 1 (Strong Signal):**
- Open with the specific signal in the first line
- Reference it again in the P.S. or follow-up
- Higher personalization, more specific CTA

**Tier 2 (Moderate Signal):**
- Lead with industry/role context, not specific news
- Use "teams like yours" language
- Still specific, but less granular

**Tier 3 (No Signal):**
- Use the "problem-first" approach without specific reference
- Focus on the pain point broadly
- Acknowledge you're reaching out cold: "Not sure if this is relevant, but..."

### Enhancement: Add Signal Tier Guidance to Email Copy Section

Add a note to each email step clarifying: "If using a Tier 1 signal, customize [ bracketed section]. If Tier 3, use generic version."

---

## Critique #4: Missing Self-Critique Checklist

### The Gap
Your iteration framework reviews metrics at the campaign level but provides **no per-sequence quality check** for reps to validate their own outreach before sending.

### Our Framework: Required Self-Critique Checklist

After generating the full sequence, evaluate:

- [ ] Does every message reference the specific signal from research, or are they generic?
- [ ] Is the LinkedIn connection request under 300 characters?
- [ ] Does the first message ask a question (invite dialogue) rather than pitch?
- [ ] Does follow-up #1 add something genuinely new, or is it just "following up"?
- [ ] Does the break-up message reference something specific about their situation?
- [ ] Did I correctly assign the personalization tier, or am I over-personalizing a Tier 3 prospect?

### Enhancement: Add Self-Critique Checkpoint

> Reps must complete the checklist before enrolling any contact in the sequence. Use this as a quality gate in your Attio workflow.

---

## Critique #5: Phone Talk Tracks Are Good But Lack "One New Thing" Rule

### The Gap
Your phone scripts are clear, but they don't emphasize the **"add one new thing" principle** — each call should bring a new data point, not just repeat the email content.

### Our Framework: Phone Call Improvement

For Day 8 and Day 15 calls:

- **Day 8:** "I shared some data on ROI earlier this week" — add a NEW metric or case study not in the email
- **Day 15:** Reference a different use case than previous calls

**Constraint:** Never call with nothing new to say. If you've already shared your best case study, find another before calling.

### Enhancement: Add "New Thing" Requirement to Talk Tracks

Update Call 2 and Call 3 to explicitly include one new data point not mentioned in previous touchpoints.

---

## Critique #6: No Pipeline Tracking Table

### The Gap
You reference Attio setup but don't provide a **tracking table** for reps to manage individual prospect journeys, signal tiers, and resurface dates.

### Our Framework: Pipeline Tracking Table

```
| Prospect | Company | Platform | Tier | Sent Date | Response | Stage | Next Action | Resurface Date |
|---|---|---|---|---|---|---|---|---|
| [Name] | [Co] | LinkedIn | 1 | [date] | — | Connection sent | Wait 24-48h | — |
| [Name] | [Co] | Email | 2 | [date] | — | First email sent | Follow-up Day 7 | — |
```

### Enhancement: Add Pipeline Tracking Table

> Track every prospect with signal tier and resurface date. Tier 3 prospects with no response should be re-engaged at 6 months with a fresh signal search.

---

## Critique #7: Breakup Email Could Reference Specific Situation

### The Gap
Your breakup email is strong ("graceful, open"), but it's generic. Our framework references something specific about their situation based on research — this significantly increases breakup reply rates (typically 3–5%).

### Our Framework: Situation-Specific Breakup

```
I'll assume timing isn't right — totally get it. 

If [relevant pain point] becomes a priority down the road, happy to reconnect. 
Best of luck with [specific thing they're working on based on research].
```

### Enhancement: Add Research Reference to Breakup

Update Step 8 to include one specific reference based on what you learned during research (their initiative, their team's focus, etc.).

---

## Critique #8: Missing LinkedIn Follow-Up Formulas

### The Gap
Your sequence includes LinkedIn Connect (Day 1) and InMail (Day 11), but **no formula for the LinkedIn message after connection** (the first DM that goes to someone who's already accepted you).

### Our Framework: Post-Accept Message (Day 2–3)

**Formula:** `[Thanks] + [Bridge to relevance] + [Light value] + [Soft question]`

**Template:**
```
Thanks for connecting. I work with [ICP description] on [specific outcome].

Curious — is [relevant function] something you own directly at [Company], 
or is that still founder-led?

Happy to share what I'm seeing work at similar-stage companies either way.
```

### Enhancement: Add Post-Accept LinkedIn Message

Add this as an automatic follow-up when a connection is accepted (triggered by Attio workflow).

---

## Summary of Enhancements

| Area | Current State | Enhancement | Impact |
|------|--------------|-------------|--------|
| Signal research | Implicit | Research-first protocol + tier assignment | Better personalization quality |
| LinkedIn notes | Undefined | 300-char formula + examples | Higher accept rates (target 25–40%) |
| Email adaptation | Two variants | Tier-based customization | Higher reply rates |
| Quality check | Campaign-level only | Per-sequence self-critique checklist | Better message quality |
| Phone calls | Generic | "One new thing" requirement | More compelling calls |
| Tracking | Attio mentioned | Pipeline table with tiers + resurfaces | Operational discipline |
| Breakup | Generic | Situation-specific reference | Higher breakup reply rate (3–5%) |
| LinkedIn DM | Missing | Post-accept formula | Doubles LinkedIn conversion |

---

## Recommended Implementation

1. **Week 1:** Add signal tier assignment to your research process; create Attio workflow to auto-assign tier based on enriched data
2. **Week 2:** Add LinkedIn connection formula and post-accept message to sequence
3. **Week 3:** Add self-critique checklist as quality gate; add pipeline tracking table
4. **Week 4:** Run first 50 contacts through enhanced sequence; measure against your existing benchmarks

---

## Additional Opportunities

Your playbook could benefit from deeper integration with:

- **Meeting prep framework** — For converting outreach replies to booked meetings
- **Go Mode autonomous execution** — For running the full sequence with guardrails
- **Case study frameworks** — For enriching value-add touchpoints with specific proof points

Let me know if you'd like me to generate any of these enhancements as standalone refinements or integrated into a revised version of the full playbook.