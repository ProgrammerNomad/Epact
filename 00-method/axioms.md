# Axioms

Epact asks what **week length** (and the rest, month, and year rules tied to it) would follow if we only used **logic** and **measurable natural cycles**. Human calendar history is not evidence for or against any design.

## What “correct” means here

There is no single mathematically correct week length. **Correct** means: given explicit goals, a design **minimizes stated error** under stated constraints.

We treat a calendar as a **model** of nature, not nature itself. Every model leaves a **remainder** (epact).

## Constraints we refuse to drop (for the main search)

These are the requirements that fight each other:

1. **Whole days** - A civil day boundary aligns with the mean solar day (86400 s). Sub-day week boundaries are excluded from the primary integer search because they break “same clock time next cycle.”
2. **Repeat forever** - Rules must be periodic or rule-based, not “adjust by decree” every few years without a formula.
3. **Circadian lock** - For global civil time, week boundaries stay on **date** lines, not drifting through clock time each cycle.
4. **Multiple natural targets** - We simultaneously care about lunar phase (synodic month), lunar quarter (~7.38 d), spring–neap (~14.77 d), and the tropical year (~365.24 d).

We **do not** require all of these to be satisfied exactly. We require that **tradeoffs be visible**.

Default score weights encode **“if weeks should track the Moon”** - not a claim from [biology.md](../01-nature/biology.md) that humans have a 7-day clock.

## Constraints we treat as optional (explored in unit files)

- Named weekdays vs phase labels
- One global week vs latitude-local light time
- Whether a “week” exists at all
- Whether rest days must equal “week length”

## Evidence rules

| Allowed | Not allowed as justification |
|--------|------------------------------|
| Astronomical mean periods (IAU / ephemeris literature) | “Romans used eight days” |
| Tidal constituent periods | “God commanded six work days” |
| Biology under controlled conditions | “ISO week is standard” |
| Continued fractions, divisor structure, approximation error | “Monday is the start because culture says so” |

History may appear only to **reject** it: e.g. “We do not infer natural week length from the spread of the seven-day week.”

Other civilizations used **different week lengths** (4, 5, 6, 8, 10, 13, 20) for year, market, rest, or ritual - the same knobs Epact separates. That is **description of lock-in**, not proof that 7 is optimal. See [why-seven.md](../05-synthesis/why-seven.md).

## Design stance

- Prefer **Pareto optimality** over a single champion.
- Publish **residuals** (hours, days per century) beside every claim.
- Separate **unit definitions** (day, rest, week, month, year) - they need not be derived from one formula.

## Outputs of this project

1. A catalog of natural cycles ([01-nature/cycles.md](../01-nature/cycles.md)).
2. Explicit scoring ([scoring.md](scoring.md)) and searches ([03-search/](../03-search/)).
3. Six **complete** candidate systems ([04-systems/](../04-systems/)).
4. A comparison on the Pareto front ([05-synthesis/comparison.md](../05-synthesis/comparison.md)).
