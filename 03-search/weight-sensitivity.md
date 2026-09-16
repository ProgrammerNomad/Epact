# Weight sensitivity

Integer scores are **not** a unique ranking of “the natural week.” They depend on how much weight you put on lunar vs solar vs scheduling terms.

Formulas: [scoring.md](../00-method/scoring.md). Table: [integer-weeks.md](integer-weeks.md).

## Score_int leaders (fixed weights)

| Rank | W | Score_int |
|------|---|-----------|
| 1 | 6 | 0.729 |
| 2 | 7 | 0.723 |
| 3 | 5 | 0.715 |
| 4 | 8 | 0.702 |

Gap **6 vs 7 = 0.006** - smaller than typical rounding in prose.

## Blend: lunar bundle vs solar/scheduling

Define:

\[
L(W) = 0.5\,M + 0.5\,Q_{\mathrm{prox}}, \quad G(W) = 0.5\,Y + 0.5\,D_{\mathrm{norm}}
\]

\[
\mathrm{Score}(\alpha) = \alpha\,L(W) + (1-\alpha)\,G(W), \quad \alpha \in [0,1]
\]

| α | Top W (Score(α)) | Reading |
|---|------------------|---------|
| 0.00 | **28** (0.978) | Year + divisibility dominate |
| 0.25 | **6** (0.857) | Mixed; 6 edges 28 |
| 0.50 | **6** (0.860) | Lunar half still favors 6 |
| 0.75 | **6** (0.864) | |
| 1.00 | **6** (0.867) | Pure lunar bundle |

**Crossover:** moving from **solar-heavy** (α→0) to **lunar-heavy** (α→1), leadership shifts from **long weeks with good Y** (e.g. 28) to **6**, then **7** is always slightly below 6 on \(L\) alone. To make **7** beat **6**, increase emphasis on **Q_prox** alone or on **S** (spring–neap), not the bundled \(L\) used here.

## Score_ref (refactored weights)

\[
\mathrm{Score\_ref} = 0.40\,L + 0.10\,S + 0.25\,Y + 0.25\,D_{\mathrm{norm}}
\]

| Rank | W | Score_ref |
|------|---|-----------|
| 1 | 6 | 0.828 |
| 2 | 8 | 0.757 |
| 3 | 5 | 0.733 |
| 4 | 28 | 0.731 |
| 5 | 7 | 0.724 |

Higher **Y** and **D** weight lifts **6** further above **7**.

## W=6 as system Hex

**6** wins or near-wins several weight vectors; the full calendar write-up is [hex.md](../04-systems/hex.md). Gap **6 vs 7 = 0.006** on Score_int remains inside hand-tuned weight noise - not proof that 6 is “the natural week.”

**Chart:** [weight-crossover.md](../06-visual/weight-crossover.md)

## Day-error vs ratio score

| W | M | E_moon (d) |
|---|-----|------------|
| 1 | 0.531 | 0.469 |
| 6 | 0.922 | 0.469 |
| 7 | 0.781 | 1.531 |
| 30 | 0.984 | 0.469 |

W=1 and W=30 look very different on **E_moon** but similar on **M**; do not use M alone as “lunation fit.”
