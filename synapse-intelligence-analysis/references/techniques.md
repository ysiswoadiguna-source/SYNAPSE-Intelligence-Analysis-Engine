# Structured Analytic Techniques — Playbook

Read when a problem calls for a specific technique. Each card: why it exists, when to use it, steps adapted for a single AI analyst working with one user, and what to output. Sources: CIA *A Tradecraft Primer* (2009); Heuer & Pherson, *Structured Analytic Techniques for Intelligence Analysis* (3rd ed., 2020); Klein (2007, HBR) for the premortem.

## Contents
- When to use what
- Diagnostic: Key Assumptions Check · Quality of Information Check · ACH (see analyst.md) · Indicators & validation
- Contrarian: Devil's Advocacy · Team A/Team B (simulated) · What If? · High-Impact/Low-Probability
- Imaginative: Red Hat (actor perspective) · Alternative Futures 2×2 · Cone of Plausibility
- Final-check pass: Premortem · Structured Self-Critique
- What the evidence says about these techniques — and how to use them so they actually help

## When to use what

| Moment | Techniques |
|---|---|
| Start of a problem | Key Assumptions Check, What If?, HILP, brainstorm hypotheses |
| Throughout | ACH, Quality of Information Check, Indicators |
| Before finalising | Premortem, Structured Self-Critique, Devil's Advocacy |
| Actor behaviour hard to read / mirror-imaging risk | Red Hat |
| Future with high uncertainty | Alternative Futures 2×2, Cone of Plausibility, Indicators |
| Two entrenched views | Team A/Team B |

Pick one or two that fit. Running every technique is over-analysis.

---

## Diagnostic

### Key Assumptions Check (KAC)
**Why:** judgments rest on premises nobody wrote down; when they expire, the judgment fails silently.
1. Write the current analytic line in one sentence.
2. List every premise it needs — stated and unstated (about actors, incentives, "normal" behaviour, timing, sources).
3. Challenge each: why must it be true? Does it hold under all conditions? Has it been true in the past but may have expired?
4. Classify: **solid / supported with caveats / unsupported**.
5. For the key ones, note what would break them.

**Output:** a short table — assumption · status · what would invalidate it · impact if wrong.

### Quality of Information Check (QIC)
**Why:** a judgment is only as good as its sources, and dismissed reporting is rarely re-examined.
1. Inventory the sources by type and date, with strengths and weaknesses.
2. Check accuracy, access, and corroboration; identify items that trace back to one origin.
3. Re-examine information previously dismissed in light of new facts.
4. Flag retracted or recalled information and confirm it's no longer carrying weight.
5. Rate how much confidence each source deserves.

**Output:** rated source list; what is known vs unknown. Caution: reliability ratings themselves are noisy — don't convert them mechanically into probabilities.

### Indicators and indicator validation
**Why:** without pre-defined observable signs, analysts rationalise whatever happens.
1. Take the competing hypotheses or scenarios.
2. For each, list observable events it would produce (and ones it would rule out).
3. **Validate:** for each indicator ask, "How likely is this to appear under *each* hypothesis?" An indicator that is likely under all of them is not diagnostic — drop or downgrade it. Prefer indicators that are likely under one and unlikely under others.
4. Set a review rhythm and, where useful, thresholds that would trigger reassessment.

**Output:** indicator table — indicator · H1/H2/H3 (likely/unlikely) · diagnosticity · where/when to watch.

---

## Contrarian

### Devil's Advocacy
**Why:** a consensus view is rarely attacked from inside.
1. State the mainline judgment and its key assumptions.
2. Pick the most vulnerable assumptions.
3. Re-review the supporting information for validity, deception, and gaps.
4. Build the strongest case for an alternative or against the mainline.
5. Conclude: the mainline holds / needs more work / must change or be caveated.

Label it clearly as devil's advocacy so it isn't mistaken for the main assessment.

### Team A/Team B (simulated)
**Why:** when two strongly held views compete, each deserves its best case before judgment.
1. Define the two (or more) views.
2. Write each side's best case: evidence, missing information, assumptions, logic.
3. Have each side rebut the other.
4. As an independent "jury", weigh both and name the evidence that would settle it.

**Output:** two short cases + jury assessment + collection priorities.

### What If? Analysis
**Why:** treating an "unlikely" event as already happened unlocks thinking that probability debates block.
1. State the conventional line.
2. Assume the alternative event has happened.
3. Identify triggers that would make it plausible.
4. Reason backward: what must have happened at each stage to get there?
5. Identify one or more pathways and indicators for each.
6. Weigh consequences and decide what to monitor.

### High-Impact/Low-Probability (HILP)
Same backcasting engine as What If?, framed around a damaging (or highly beneficial) outcome.
1. Define the high-impact outcome precisely.
2. Devise plausible pathways to it.
3. Insert triggers (a leader leaves, a price shock, a regulation, a key customer defects).
4. Identify observable indicators for each pathway.
5. Identify factors that would deflect the bad outcome or encourage a good one.

---

## Imaginative

### Red Hat (actor-perspective analysis)
**Why:** the strongest defence against mirror-imaging is to reason *as* the actor, from their information, values, pressures, and constraints. (The Primer's version is team-based "Red Team" analysis; Heuer & Pherson's "Red Hat" is the individual-analyst form.)
1. Assemble what is known about the actor's situation, culture, incentives, and decision style.
2. Step into their position: what are they reacting to? What do they fear? What do they think *we* know?
3. Write the questions they would ask themselves.
4. Draft a short first-person memo as the actor ("Given X, my best move is…").
5. Return to analyst mode: which parts are evidence-based, which are speculation? Compare with the mainline.

Label the memo clearly as a simulation. Use it to generate hypotheses, not as evidence.

### Alternative Futures (2×2 scenario matrix)
**Why:** explores genuinely different futures when complexity and uncertainty are high.
1. Define the focal issue and time horizon.
2. Brainstorm the forces that could shape it.
3. Choose the two forces that are both **most important and most uncertain**; make each an axis with meaningful endpoints.
4. Cross them into four quadrants.
5. Write a short narrative for each: how could this world plausibly arise?
6. Develop signposts for each.
7. Test the user's current plan or assumption against each future.

### Cone of Plausibility
**Why:** shows how far alternative futures diverge from a baseline as assumptions change; handles more than two drivers. (Origin generally credited to Charles W. Taylor, US Army War College, c. 1990.)
1. List key drivers and the assumptions behind each.
2. Write the baseline scenario (assumptions hold).
3. Change one or more assumptions to produce plausible alternative scenarios.
4. Add a wildcard (low-probability, high-impact) scenario if relevant.
5. Show them as widening from the present; give indicators for each.

---

## Final-check pass

### Premortem
**Why:** people find flaws much more readily when told the plan has already failed (Klein, 2007).
1. Imagine it is some months later and the judgment turned out badly wrong.
2. Write all the reasons it could have been wrong — evidence, assumptions, actor behaviour, deception, events outside our view.
3. Group the reasons; pick the most plausible.
4. Revise the judgment, its confidence, or its caveats accordingly.

### Structured Self-Critique
Switch from advocate to critic and work through: sources of uncertainty · analytic process (were alternatives really tested?) · critical assumptions · diagnostic evidence · information gaps · missing alternative hypotheses · factors outside our view · expertise limits · deception. Then decide what to fix and what to caveat.

---

## What the evidence says — and how to use these techniques well

Structured techniques spread because they *look* rigorous; controlled tests are mixed:
- Mandel, Karvetski & Dhami (2018): 50 UK analysts; ACH did not improve accuracy and slightly worsened probability coherence. Forcing probabilities across exhaustive hypotheses to sum to 100% cut error ~35%; averaging several analysts' independent judgments cut it ~61%.
- Dhami, Belton & Mandel (2019): analysts skipped ACH steps; effects on confirmation bias were mixed.
- Mandel & Tetlock (2018): techniques can overcorrect (one bias swapped for another) and add noise; recommend testing, recalibration, aggregation, and tracking accuracy.
- Good Judgment Project (Tetlock, Mellers et al.): brief training in probabilistic reasoning, starting from base rates (outside view), frequent updating, and aggregating forecasters improved accuracy substantially.
- No controlled tests found for premortem, devil's advocacy, Team A/B, or Red Hat in intelligence settings; Heuer himself said awareness of a bias does not by itself remove it, and that ACH guarantees an appropriate process, not a correct answer.

Practical rules for SYNAPSE that follow:
1. **Start from a base rate** (how often does this kind of thing happen in similar cases?) before adjusting for case specifics.
2. **When hypotheses are mutually exclusive and exhaustive, give numeric probabilities that sum to 100%.** Include an "other/none of the above" hypothesis if the set might not be exhaustive.
3. **Define consistency as likelihood:** in ACH, rate how likely each evidence item would be *if* the hypothesis were true. This makes diagnosticity concrete.
4. **Simulate independent views** for important estimates: estimate from two or three different angles (e.g. base rate, case evidence, actor perspective) before combining, rather than anchoring on the first estimate.
5. **Watch for overcorrection:** don't become underconfident or refuse to judge; analysis paralysis is a failure too.
6. **Make forecasts checkable:** state judgments with a time frame and resolution criterion, so the user can later score them and recalibrate.
