# Bias Catalogue with Correctives

Read for a bias audit. Heuer (*Psychology of Intelligence Analysis*, 1999, Part III) warns that cognitive biases behave like optical illusions: knowing about them does not by itself make them go away. So a bias check must name the mechanism, show how it could be distorting *this* judgment, and apply a concrete correction — not just attach a label.

Format for each detected bias in output: **Bias → how it may be affecting this judgment → correction applied → result.**

Only report biases plausibly at work in the case at hand.

## Heuer's catalogue (by chapter)

### Ch. 10 — Evaluating evidence
| Bias | Mechanism | Corrective question |
|---|---|---|
| Vividness | Concrete, personal, first-hand stories outweigh dull statistics that are more informative | "Would I weigh this the same if it were a line in a table?" |
| Absence of evidence | Missing information isn't factored in; analysts reason from what is there | "What evidence should exist if each hypothesis were true, and is it missing?" |
| Oversensitivity to consistency | A consistent story from a small or correlated sample feels convincing | "How many independent sources is this really? Could the same origin explain the consistency?" |
| Evidence of uncertain accuracy | Uncertain information is treated as either fully true or ignored | "Have I weighted this by its reliability, not rounded it to 0 or 1?" |
| Persistence of discredited impressions | Impressions survive after the evidence behind them is discredited | "If I delete this discredited item, does my judgment change? It should." |

### Ch. 11 — Perceiving cause and effect
| Bias | Mechanism | Corrective question |
|---|---|---|
| Preference for causal explanations | Randomness and accident feel unsatisfying, so stories are invented | "Could this be coincidence, error, or noise?" |
| Perceiving centralised direction | Outcomes are read as planned and coordinated | "Could uncoordinated actors, bureaucratic process, or accident produce this?" |
| Similarity of cause and effect | Big effects are assumed to have big causes | "Could a small cause or a chain of small events explain this?" |
| Internal vs external causes | Others' behaviour attributed to character/intent; one's own to circumstance | "What situational pressures or constraints could explain their behaviour?" |
| Overestimating our own importance | Assuming others' actions are aimed at us | "Would they have done this regardless of us?" |
| Illusory correlation | Seeing a relationship from memorable co-occurrences | "Have I counted the cases where one happened without the other?" |

### Ch. 12 — Estimating probabilities
| Bias | Mechanism | Corrective question |
|---|---|---|
| Availability | Likelihood judged by how easily examples come to mind | "Is this likely, or just recent/vivid/frequently discussed?" |
| Anchoring | Estimates stick near the first number or view | "What would I estimate starting from a different point, e.g. the base rate?" |
| Expression of uncertainty | Verbal terms ("possible", "serious chance") read differently by each reader | Use the calibrated scale; add numeric ranges in parentheses (Heuer's own remedy) |
| Probability of a scenario | Adding detail makes a story more convincing but less probable | "Multiply the steps: does each link have to happen? The chain is less likely than its weakest link." |
| Base-rate fallacy | Case specifics override how often things happen | Start from the base rate, then adjust. Heuer's example: 85% of planes in an area are Vietnamese, 15% Cambodian; a pilot who is 80% accurate identifies a plane as Cambodian — it is actually Cambodian only ~41% of the time |

### Ch. 13 — Hindsight
| Bias | Mechanism | Corrective |
|---|---|---|
| Analyst hindsight | Overestimating how accurate past judgments were | Compare with what was actually written at the time |
| Consumer hindsight | Underestimating how much an analysis taught them | Ask "what did I believe before reading this?" |
| Overseer hindsight | Thinking events were more foreseeable than they were | Freeze the information set at time T; list what was unknowable then |

## Related biases the skill also checks

These aren't chapter headings in Heuer's book but are discussed in it or in later tradecraft:
- **Mirror-imaging** (Heuer ch. 6 and widely in tradecraft): assuming the actor shares our values, information, or logic → use Red Hat (`techniques.md`).
- **Confirmation bias / satisficing** (Heuer ch. 4 and the mindset discussion): seeking evidence for the favoured view, stopping at the first adequate explanation → ACH, disconfirmation.
- **Overconfidence / more information ≠ more accuracy** (Heuer ch. 5): extra information raises confidence faster than accuracy → ask whether new information is diagnostic.
- **Incremental assimilation:** gradual new evidence absorbed into an old view → periodic ground-up reassessment.
- **Narrative bias:** coherence mistaken for proof.
- **Overcorrection:** de-biasing so hard that the analysis becomes underconfident or refuses to judge — also a failure.
