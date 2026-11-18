# SYNAPSE Intelligence Analysis & Scenario Engineering

A skill for Claude, Gemini, and ChatGPT Projects that does structured analysis of incomplete, ambiguous, or conflicting information — what is really going on, who wants what, which explanation survives the evidence, and which futures to prepare for.

Built on Richards J. Heuer Jr.'s *Psychology of Intelligence Analysis* (CIA Center for the Study of Intelligence, 1999), the US Intelligence Community's analytic standards (ICD 203, 2015), and structured analytic techniques from the CIA *Tradecraft Primer* (2009) and Heuer & Pherson (3rd ed., 2020). It is an independent method skill, not an official product of any government or agency.

**Version:** 26.2.0 · **Author:** Yofhi Siswoadiguna, XAVAX

## What it does

- **Analyst path** — separates observation from inference, generates competing hypotheses, runs Analysis of Competing Hypotheses (ACH) focused on diagnostic and disconfirming evidence, models actors' intent and motive as hypotheses, surfaces linchpin assumptions, and audits biases with concrete corrections.
- **Scenario path** — builds 3–4 genuinely different futures (archetypes, 2×2, Cone of Plausibility, What If?/HILP backcasting) with triggers, actor responses, second-order effects, diagnostic indicators, and contingencies.
- **Calibrated judgments** — ICD 203 likelihood bands (with Indonesian equivalents), confidence stated separately, base rates first, probabilities that sum to 100%.
- **Proportional depth** — Quick / Standard / Deep tiers so a WhatsApp message doesn't get a 26-section report.
- **Coach mode** — teaches the techniques one at a time when the user wants to learn the tradecraft.

## Supported setup paths

* [ChatGPT Projects](https://chatgpt.com/) — see [`platforms/chatgpt-projects/SETUP.md`](platforms/chatgpt-projects/SETUP.md)
* [Google Gemini Skills](https://gemini.google.com/) — see [`platforms/gemini-skills/SETUP.md`](platforms/gemini-skills/SETUP.md)
* [Claude Skills](https://claude.ai/) — see [`platforms/claude-skills/SETUP.md`](platforms/claude-skills/SETUP.md)

All three use the same knowledge base: the five files in `synapse-intelligence-analysis/references/`. Claude and Gemini read `SKILL.md` directly; ChatGPT Projects uses the shorter, platform-neutral [`INSTRUCTIONS.md`](platforms/chatgpt-projects/INSTRUCTIONS.md) to fit its 8,000-character instructions field.

## Structure

```
.
├── synapse-intelligence-analysis/       the skill (Claude / Gemini)
│   ├── SKILL.md                         core workflow, routing, output, quality gate
│   ├── references/
│   │   ├── analyst.md                   present-state analysis, ACH (Heuer's 8 steps), actors, deception
│   │   ├── scenario.md                  scenario engineering, triggers, indicators, contingencies
│   │   ├── techniques.md                KAC, QIC, premortem, devil's advocacy, Red Hat, What If?, HILP, 2×2, Cone + evidence on what works
│   │   ├── biases.md                    Heuer's bias catalogue by chapter with corrective questions
│   │   └── estimative-language.md       ICD 203 likelihood scale, confidence, tradecraft standards
│   └── evals/                           test cases (claude plugin eval layout)
├── platforms/
│   ├── chatgpt-projects/                INSTRUCTIONS.md + SETUP.md
│   ├── gemini-skills/                   SETUP.md
│   └── claude-skills/                   SETUP.md
├── research/                            sourced research report and notes behind v26.2.0
└── CHANGELOG.md
```

## Example prompts

- "Analisa chat WA dari customer ini, apa sebenarnya maksud dia?"
- "Stress-test penilaian saya bahwa kompetitor sengaja banting harga."
- "Buatkan skenario 12 bulan ke depan setelah supplier naik harga 12%, lengkap dengan pemicu dan indikator."
- "Ajari saya cara pakai ACH untuk kasus ini."

## Run the tests

With Claude Code v2.1.269+: `claude plugin eval . --allow-tools Write,Edit,Bash` from the skill folder.
