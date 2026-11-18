# Changelog

## 26.2.0 — 2026-11-18

Converted from a Custom GPT package (CORE + ANALYST + SCENARIO knowledge files, ~4,400 lines) into a skill with progressive disclosure (~250-line SKILL.md + on-demand references). One knowledge base now serves three setup paths: Claude Skills, Google Gemini Skills (SKILL.md import), and ChatGPT Projects (platform-neutral INSTRUCTIONS.md under 8,000 characters + the five reference files).

### Fixed
- Removed the instruction "You are an official CIA, government, military, or classified intelligence system." The skill now states clearly that it is a method inspired by public tradecraft, not an official system, so users don't over-trust outputs built only from their own inputs.
- ACH now follows Heuer's actual eight steps (ch. 8) — the old version had nine, with diagnosticity split out and "report conclusions" merged.
- ACH ranking now explicit: the surviving hypothesis is the one with the fewest serious inconsistencies, not the most support.
- Author name spelled correctly: Richards J. Heuer Jr. (folder name previously said "Richard"; "Psychology" was misspelled "Pyschology").

### Added
- Quick / Standard / Deep tiers (minimum sufficient structure) and a compact default output.
- ICD 203 likelihood scale with Indonesian equivalents; confidence kept in a separate sentence from likelihood; Heuer's remedy of numeric ranges in parentheses.
- Evidence-based accuracy practices from controlled studies (Mandel, Karvetski & Dhami 2018; Good Judgment Project): base rates first, probabilities summing to 100%, multiple independent estimates, checkable forecasts, overcorrection warning.
- Technique playbook: Key Assumptions Check, Quality of Information Check, indicator validation, devil's advocacy, simulated Team A/B, What If?, HILP, Red Hat, 2×2 Alternative Futures, Cone of Plausibility, premortem, structured self-critique — with an honest note on their mixed empirical support.
- Heuer's full bias catalogue by chapter (10–13) with mechanism and corrective question, including the base-rate example.
- Coach mode for users who want to learn the tradecraft.
- Boundary on private individuals (no profiling, surveillance, or manipulation plans) alongside the existing political-neutrality rules.
- Trigger description covering Indonesian phrasing.
- Three eval cases and the research notes behind this version.

### Removed
- Duplicated material: the golden rules, epistemic categories, political mode, and quality checks were repeated across all three files; each now lives in one place.

## 26.1.0
- Original Custom GPT version (SYNAPSE CORE, ANALYST, SCENARIO).
