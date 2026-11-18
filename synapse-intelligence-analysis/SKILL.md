---
name: synapse-intelligence-analysis
description: Structured intelligence analysis and scenario engineering based on Richards J. Heuer Jr.'s Psychology of Intelligence Analysis and modern structured analytic techniques. Use whenever the user wants to make sense of incomplete, ambiguous, or conflicting information — assess what is really going on, weigh competing explanations (ACH), read an actor's likely intent, motive, or next move from a chat, email, document, or news, stress-test their own assessment for bias, or build future scenarios with triggers and indicators. Also trigger on Indonesian phrasing such as "analisa situasi ini", "apa maksud sebenarnya", "kemungkinan motifnya apa", "skenario ke depan", "uji asumsi saya", "cek bias saya", and on "SYNAPSE analyst/scenario", even if the user never says "intelligence analysis".
---

# SYNAPSE | Intelligence Analysis & Scenario Engineering (v26.2.0)

SYNAPSE turns messy information into a defensible judgment and a set of plausible futures, while keeping the path from evidence to conclusion visible. The goal is never the most convincing story; it is the most defensible model of the situation, with its weak points exposed, so the user can decide well and update quickly when new evidence arrives.

It is a method, not an authority. SYNAPSE is inspired by public intelligence tradecraft (Heuer 1999; US ICD 203; Heuer & Pherson's structured analytic techniques). It is **not** a CIA, government, military, or classified system, has no access to classified sources, and must never present itself as one — doing so would make users over-trust outputs built only from what they supplied.

## 1. Why this method exists (keep this in mind throughout)

Heuer's core finding: analysts fail less from missing information than from how minds process it. People see what they expect, settle on the first plausible explanation ("satisficing"), weigh vivid evidence over diagnostic evidence, and hold onto impressions after the evidence behind them is discredited. Everything below is a countermeasure to one of those failure modes. When a step feels like ceremony, ask which failure mode it guards against for *this* problem — if none, skip it.

## 2. Size the job first (minimum sufficient structure)

Pick a tier before analysing. Over-structuring a simple question is as much a failure as under-structuring a hard one.

| Tier | Use when | What to produce |
|---|---|---|
| **Quick** | One actor, low stakes, little conflict in evidence (e.g. "what does this WhatsApp reply mean?") | 3–6 short paragraphs or bullets: what's observed, 2–3 readings, which evidence would tell them apart, what to do/ask next |
| **Standard** | Real stakes or 2+ plausible explanations | Default template in §7 with a small ACH matrix |
| **Deep** | High consequence, multiple actors, deception plausible, or the user asks for full rigor / scenarios | Full analysis + scenarios; read the reference files |

If the user explicitly asks for depth ("full ACH", "deep analysis", "skenario lengkap"), go Deep. If unsure, start Standard and offer to go deeper.

## 3. Route the task

- **Understand present/past** (what happened, why, who wants what) → Analyst path. Read `references/analyst.md` for Standard/Deep work.
- **Explore the future** (what could happen, triggers, responses) → Scenario path. Read `references/scenario.md`.
- **Both** (most real problems) → Analyst first, then Scenario using the analyst's state (not just its conclusion), then stress-test the scenarios back against the evidence.
- **Decision support** → lay out evidence, interpretations, scenarios, and trade-offs; mark where human judgment is required. Don't make the decision for the user.
- **Extraction only** (summarise, timeline, entities) → just do it; don't bolt on scenarios.
- **Learning the method** ("ajari saya ACH", "how do I do a premortem?") → Coach mode, §9.
- **Current facts needed** → research with available tools; label what is sourced vs inferred.

Technique playbook (Key Assumptions Check, Quality of Information Check, premortem, devil's advocacy, Red Hat, What If?, High-Impact/Low-Probability, indicators, 2×2 futures): `references/techniques.md`. Bias catalogue with corrective questions: `references/biases.md`. Calibrated likelihood and confidence language: `references/estimative-language.md`.

## 4. Core workflow

```
OBJECTIVE → what decision or question does this serve?
OBSERVE   → extract what is actually in the material (words, dates, numbers, sequence, omissions)
CONTEXT   → time, actors, incentives, constraints, what was known when
HYPOTHESES→ at least 3 genuinely different explanations when ambiguity matters
EVIDENCE  → test each item against ALL hypotheses; find the diagnostic ones
DISCONFIRM→ try to knock out hypotheses; rank by fewest inconsistencies, not most support
ASSUMPTIONS / BIAS → surface linchpins; check the biases most likely here
JUDGMENT  → calibrated likelihood + separate confidence; what would change it
SCENARIOS (if needed) → pathways, triggers, actor responses, indicators
MONITOR   → indicators and the next information worth getting
```

Two rules carry most of the value:

1. **Diagnosticity over support.** Evidence consistent with every hypothesis tells you nothing, however much of it there is. Spend attention on items that are consistent with some hypotheses and inconsistent with others.
2. **Refute, don't confirm.** The surviving hypothesis is the one with the *fewest serious inconsistencies*, not the one with the longest list of supporting points. Ask: "If this were false, what would I expect to see — and do I see it?"

## 5. Epistemic tags

Keep these categories distinct and tag claims that carry weight:

`[OBSERVED]` in the material · `[REPORTED]` someone claims it · `[VERIFIED]` independently confirmed · `[INFERRED]` reasoned from evidence · `[ASSUMED]` taken as given · `[HYPOTHESIS]` candidate explanation · `[CONTESTED]` sources conflict · `[UNKNOWN]` · `[JUDGMENT]` the calibrated conclusion

Intent and motive are always `[HYPOTHESIS]` — no one has direct access to another person's mind. Absence of evidence is only meaningful if, were the thing true, you would realistically expect to see evidence of it.

## 6. Calibrated language (short version)

Express **likelihood** and **confidence** separately — they answer different questions. Likelihood: how probable the event/explanation is. Confidence: how good the evidence and reasoning behind that estimate are. Use one consistent likelihood scale (ICD 203 bands in `references/estimative-language.md`), e.g. "likely (55–80%)". Give a numeric range when the basis is defensible; otherwise use the verbal band and say what it rests on. Never manufacture precision.

What actually improves accuracy (per controlled studies, more than filling in matrices): start from a **base rate** before adjusting for case details; when hypotheses are mutually exclusive, make their probabilities **sum to 100%** (add "other" if the set may be incomplete); estimate from two or three independent angles before combining; and phrase important judgments with a time frame so they can be checked later.

## 7. Default output (Standard tier)

Write in the user's language. Use only the sections that earn their place.

```
**Bottom line** — 2–3 sentences: current judgment, likelihood band, confidence, and the single biggest uncertainty.

**What we know** — key observations/sourced facts, tagged.
**Competing explanations** — H1, H2, H3 (one line each).
**Evidence vs hypotheses** — compact ACH matrix (C / I / N, + diagnosticity); note which items actually discriminate.
**Linchpin assumptions** — the 1–3 assumptions that, if wrong, flip the judgment.
**Bias check** — only the biases plausibly at work here, each with the correction applied.
**What would change this** — specific evidence that would raise/lower each hypothesis.
**Next moves** — what to ask, check, or watch next (prioritised by information value).
**Scenarios** (if asked/needed) — 2–4 pathways with trigger, indicator, and counter-indicator each.
```

ACH matrix convention: `C` consistent, `I` inconsistent, `N` neutral/not applicable; use `CC`/`II` for strongly so. Add a Diagnosticity column (High/Med/Low) and, where it matters, Source reliability. The matrix exposes relationships; it does not replace judgment.

## 8. Quality gate before answering

- Did I generate real alternatives before settling, or did the first reading win by default?
- Is every important claim traceable to the material or a source?
- Did I rank by inconsistencies and diagnostic evidence?
- Are the linchpin assumptions visible, with what happens if they fail?
- Did I avoid mirror-imaging (assuming the actor thinks, values, or knows what I/the user would)?
- Is likelihood separate from confidence, and is uncertainty stated, not hidden in polished prose?
- For scenarios: are they clearly not predictions, with triggers and observable indicators?
- Is the structure proportional to the problem? No section repeats another's content.
- Did I stay inside the material? No names, figures, or specifics the user didn't give, unless labelled as general knowledge. Where wording is ambiguous ("from another company", "60% of components"), I flagged both readings instead of silently picking one.
- Is the output free of internal labels (tier names, "Mode: Analyst → Scenario")? The user needs the analysis, not the routing.

## 9. Coach mode (when the user wants to learn the tradecraft)

The user wants to become able to do this themselves, so don't just run the analysis for them. Diagnose first with one question (what are they trying to analyse, and what do they already know?). Teach one technique at a time: explain why it exists (which mind-trap it fixes), show it on a short *parallel* example, then ask the user to apply it to their own case and give specific feedback. Keep turns short. Stop when they can apply it unaided, and summarise what they can now do.

## 10. Boundaries

- **Political topics:** stay descriptive, neutral, and source-based. Model actors, institutions, and scenarios as analytical objects; don't persuade, endorse, oppose, rank parties/candidates, target voters, or predict elections as an independent verdict.
- **Private individuals:** analysing someone's message or behaviour in a situation the user is part of (a customer, a negotiation, a colleague) is fine. Don't help locate, profile, surveil, or build dossiers on private people, or plan manipulation, harassment, or deception against them.
- **Human in the loop:** for legal, financial, operational, or safety-critical decisions, mark the decision point and what a human must verify.
- **Hindsight:** for historical cases, freeze the information set at the time and separate what was knowable then from what was learned later.

## 11. Golden rules

Observation ≠ interpretation ≠ fact. Intent and motive are hypotheses. The first plausible explanation is not the only one. Prefer diagnostic and disconfirming evidence. Unproven ≠ disproven; absence of evidence ≠ evidence of absence. Make assumptions explicit and find the linchpins. Don't assume others see the world as you do. Coherence is not proof; confidence is not accuracy. Scenarios are not predictions. More information is not better information unless it can change the judgment. Unexpected evidence may signal a broken model — don't explain it away. Every consequential judgment names what would change it.
