# Why seven days became global

Epact’s main question is **what week length nature and logic allow** ([README.md](../README.md)). This note asks a different one: **why does almost everyone use a 7-day civil week now?** History here is **description of lock-in**, not proof that 7 is the correct week ([axioms.md](../00-method/axioms.md)).

## Direct answer

**No. Not every civilization used seven days.** The world looks the same today because later people **copied and converted**, not because every culture independently measured the same number.

| Mechanism | What it produces | Can arise independently? |
|-----------|------------------|---------------------------|
| **Lunar quarter** (~7.382647 d) | A temptation to count **~7 or ~8** whole days | Yes, wherever people watch the Moon |
| **Named 7-day civil week** | Weekday names + regular rest + law and trade | Spreads by **contact** (religion, empire, ISO) |

Watching the Moon can suggest “about a week” in many places. A **global identical Monday-style grid** is **path dependence**: one package replaced other local cycles.

## Other week lengths (same knobs as this research)

These are **design choices** - the same targets Epact scores. This is not a full history survey; it shows 7 was never the only civil answer.

| Place / system | Week (days) | Why (first principles) | Epact analogue |
|----------------|-------------|------------------------|----------------|
| Egypt (decades) | **10** | Split the **solar year** (36×10 = 360 + leftover days) | [Solar5](../04-systems/solar5.md) - year-first |
| China (xun) | **10** | Administrative **decade** inside the month | Solar-first, not lunar quarter |
| Rome (nundinae) | **8** | **Market** cycle; 8 = 2³ for halves | [Binary](../04-systems/binary.md) |
| French Republican | **10** | Decimal year; **reject 7** on purpose | Solar5 / year grid |
| USSR (1929–40) | **5**, then **6** | Factory **rest** and continuous shifts | [Rest](../02-units/rest.md) - rest ≠ week-from-Moon |
| Maya / Mesoamerica | **13**, **20** | Ritual counts, not lunation ÷ 4 | Extra cycles ([cycles.md](../01-nature/cycles.md)), not a lunar week |
| Java / Bali | **5** (+ overlapping 3, 7) | Market + ritual **overlays** | [Dual](../04-systems/dual.md) |
| West Africa (e.g. Yoruba) | **4**, sometimes **8** | Market interval | Rest/market density, not 7.38 d |

**Why they differed:** they optimized **year, market, rest, or ritual** - not “nearest integer to 7.38.” Change the weights, change the winner ([weight-sensitivity.md](../03-search/weight-sensitivity.md)).

**Why most disappeared:** the 7-day **package** (names + rest + empire/religion/ISO) won on **coordination cost**, not on a better score. Local weeks were not copied into 7 from each other; **7 was copied onto them**.

## Nature: why 7 is a candidate (not why it won globally)

Synodic month ÷ 4 = **7.382647…** mean solar days ([constants.md](../00-method/constants.md)).

If you want whole days, lunar phase, and clock-locked boundaries:

- **7** is the closest integer **below** the quarter.
- **8** is the closest **above**.
- Four × 7 days = 28 d → **1.53 d short** of one lunation every month if you force four equal weeks.

Biology does **not** pick 7 ([biology.md](../01-nature/biology.md)). On **Score_int**, **6** ranks slightly above **7** ([integer-weeks.md](../03-search/integer-weeks.md)); **6** also has a **stronger year term (Y)** than 7. Calendar write-up: [hex.md](../04-systems/hex.md).

## Lock-in: why the package spread

Three stacked choices, then diffusion:

1. **Seven wanderers** (Sun, Moon, five planets) → seven named days. That counts **bodies**, not 7.38 d.
2. **Rest glued to 7** (Sabbath-style) → rest *density* fused to week *length* ([rest.md](../02-units/rest.md)).
3. **Empire, conversion, ISO** → once markets, worship, and law share one grid, switching cost beats astronomy.

## What Epact adds

Humans picked **one** integer (7) and forced months and years around it. A stronger integer construction in this repo is **not** “always 7”: it is **7 and 8 mixed**, 29/30-day months, and the Metonic **6940-day** grid ([metonic-week-grid.md](../03-search/metonic-week-grid.md)).

**Short version:** Nature almost chose **7.38 d**. Some places rounded to **7** or **8**. Others used **4, 5, 6, 8, 10, 13, 20** for year, market, rest, or ritual. The planet looks like 7 because that **package was copied onto** the others.

## See also

- [comparison.md](comparison.md) - Pareto front for designed systems
- [choose-a-system.md](../06-visual/choose-a-system.md) - pick by priority (moon vs solar vs market)
- [other-weeks.md](../06-visual/other-weeks.md) - diagram of historical targets

## Sources

Historical claims: [sources.md](../00-method/sources.md). Astronomy: [constants.md](../00-method/constants.md).
