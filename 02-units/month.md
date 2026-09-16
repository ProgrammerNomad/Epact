# Unit: month

“Month” is the most overloaded word in calendrics. Epact separates **astronomical months** from **bookkeeping months**.

## Astronomical options

| Month | Mean length (d) | Best for |
|-------|-----------------|----------|
| **Synodic** | 29.530589 | Phases, tides, visible Moon |
| Sidereal | 27.321662 | Star-aligned lunar motion |
| Tropical | 27.321582 | Ecliptic longitude |
| Anomalistic | 27.554550 | Distance / perigee |
| Draconic | 27.212221 | Eclipses, nodes |

**Default for lunar-facing systems:** **synodic**.

## Bookkeeping strategies

1. **True lunar month** - month ends on new moon (or full). Length varies ±~13 h around mean; mean still 29.530589 d.
2. **Fixed-length month** - e.g. 30 d or 29 d alternating; drift vs phases unless corrected.
3. **Twelfth of tropical year** - ~30.43685 d; solar-first, lunar-detached.
4. **Week-packing** - e.g. four 7-day weeks = 28 d (always short vs synodic).

## Error budget (four × 7-day weeks)

\[
4 \times 7 = 28\ \text{d} \quad vs \quad 29.530589\ \text{d} \Rightarrow \text{short by } 1.530589\ \text{d per month}
\]

About **18.4 h** per week of drift if you refuse intercalation - roughly **1.53 days per lunar month** accumulated.

Mixed 7/8 blocks reduce mean week toward 7.382647; see [mixed-weeks.md](../03-search/mixed-weeks.md).

## Relation to Metonic cycle

Tropical year / synodic month ≈ 12.368266. Convergent **19 years : 235 months** is the standard high-quality lunisolar fit. With [constants.md](../00-method/constants.md) means, **235 × synodic** and **19 × tropical** day-counts differ by **≈ 0.133 d (~3.2 h)** - close ratio, not exact days. The **6940 d** integer week grid is a separate civil approximation ([metonic-week-grid.md](../03-search/metonic-week-grid.md)). Week–month epact remains **large** unless mixed weeks or leap weeks are used.

## Month naming without history

- Ordinals: Month 1 … Month 12 (solar) or lunation index (lunar).
- Phase anchors: month opens at **new moon**.
- Epact display: days since last new moon (0–29).

## Historical fixed months + epact days

**12×30 + epagomenal days** (Egyptian civil year), French Republican **12×30 + 5/6**, and Maya **Haab 18×20 + 5** are real calendars that put the mismatch in **orphan days** at year-end - the same mechanism generalized as **epact days** in [intercalation.md](../03-search/intercalation.md). Not proof that 30-day months are “natural”; they are **bookkeeping + honesty about remainder**. See [sources.md](../00-method/sources.md).
