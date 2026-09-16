# Intercalation and epact placement

When two cycles are forced into one grid, the mismatch must live somewhere. **Epact** is that remainder made explicit.

## Mechanisms

| Mechanism | What is inserted | Typical scale | Good for |
|-----------|-------------------|---------------|----------|
| **Leap day** | 1 solar day | ~4 y (Gregorian-like) | Tropical year |
| **Leap month** | 1 synodic month | ~3 y (lunisolar) | Month–year |
| **Leap week** | 7 (or W) days | rare proposals | Week–year |
| **Epact day** | Day outside week count | each month or lunation | Week–month |
| **Accepted drift** | nothing | unbounded | Low-precision cultures |
| **Phase reset** | re-label at new moon | every lunation | Lune / Dual overlay |

## Week–month epact

Force four integer weeks per lunation (28 d base):

\[
\delta_m = 29.530589 - 28 = 1.530589\ \text{d} \approx 36.7\ \text{h/month}
\]

Options:

1. **Epact day(s)** - 1–2 days per month not belonging to week 1–4 (or named “Epact”).
2. **Alternating 8th week** - third week is 8 days once per month (pattern-dependent).
3. **Mixed 7/8** - reduce mean error to ~0.5 d then one epact day ([mixed-weeks.md](mixed-weeks.md)).

## Week–year epact

Uses **round**(365.242 / W) weeks per year (same as \(Y(W)\) in [scoring.md](../00-method/scoring.md)), not floor.

| W | Weeks/yr (round) | Days/yr | Δ vs 365.242 (d) |
|---|------------------|---------|------------------|
| 5 | 73 | 365 | −0.242 |
| 6 | 61 | 366 | +0.758 |
| 7 | 52 | 364 | −1.242 |
| 8 | 46 | 368 | +2.758 |
| 8 | 45 | 360 | −5.242 |

**W=7:** ~1.24 d short per year → epact days or leap week.

**W=6:** ~0.76 d **long** per year → better Y score than 7; occasional omitted day or 60-week year variant.

**W=8:** 46×8 = 368 is closer solar fit than 45×8 = 360. **Binary** chooses 360 + epact block **by design**, not because 8-day weeks require 45 weeks.

## Month–year epact (Metonic family)

Ratio tropical year / synodic month = 12.368266…

Convergent **19 years = 235 months**; error ~2 h over 19 y. Lunisolar calendars insert **7 leap months per 19 years**.

This does **not** resolve week–month epact. Metonic fixes **year ↔ month**; Epact project week layer is orthogonal.

## Leap week (concept)

Insert an entire **W-day week** every N years to absorb \(\delta_y\).

Example for W=7, \(\delta_y \approx 1.242\) d:

- 1.242 / 7 ≈ 0.177 leap weeks per year → one leap week every ~5.65 years.

Rare in real-world calendars; documented here as logical option.

## Unassigned epact days

Days with **no week number** (only month day index or “Epact” label):

- Preserves integer weeks elsewhere.
- Honest about non-nesting ([impossibility.md](../00-method/impossibility.md)).
- Used in **Mix** and **Binary** year-end handling.

## Drift as policy

Accept that phases walk through the civil grid:

- No leap month; moons ignored for civil dates.
- Phases remain observable but **not** synchronized.

**Binary** and **Solar5** lean solar; **Lune** rejects drift for phases.

## System mapping

| System | Primary epact handler |
|--------|------------------------|
| Lune | Phase-defined boundaries; sub-day epact absorbed in quarter definition |
| Mix | 29/30 month pair in 59 d; Metonic 6940-d grid ([metonic-week-grid.md](metonic-week-grid.md)) |
| Binary | 360-day year + 5.242 epact days (or 5-day epact week) |
| Solar5 | Leap day every 4 years (approx) |
| Dual | Civil epact rules + independent lunar epact on overlay |
| Hex | Leap **week** (61 vs 60 weeks/year); 8-year 7×366 + 1×360 mean |

Details in `04-systems/*.md`.
