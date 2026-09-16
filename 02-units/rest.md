# Unit: rest

**Rest** is how often a society pauses work for recovery. It is **not** the same variable as **week length**.

## Two parameters

1. **Cycle length** - e.g. 7 days, 8 days, or no named cycle.
2. **Rest count per cycle** - e.g. 1 rest day, 2 rest days, or fractional “rest density.”

Example: **6 work + 1 rest** inside a **7-day week** gives rest fraction \(1/7\). The same rest fraction could exist inside an **8-day** week as **6 work + 2 rest** (fraction \(2/8 = 1/4\)) - different social feel, same “one day off per 7 work days” if configured differently.

## Biological input

- Circadian rhythm → **nightly** rest (within-day).
- Ultradian → **within-night** structure.
- No robust law → “exactly one rest day every 7 civil days” is a **policy**, not a theorem.

The Soviet **continuous work week** (1929–1940) used **5-** then **6-day** cycles for factory rest - rest density chosen for shifts, not lunar quarters. Same separation of rest from “natural week length” ([why-seven.md](../05-synthesis/why-seven.md)).

## Rest without a week

Alternative: count **every Nth day** as rest (e.g. every 5th day) without grouping days into named weeks. Month and year still exist; only the **intermediate bundle** vanishes.

## Naming rest days

Avoid historical weekday names in Epact systems. Options:

- **Ordinal:** rest on day 7 of cycle.
- **Phase:** rest at **full moon** (ties to Lune/Dual).
- **Binary:** rest on `11` in a 3-bit day counter (Binary system).

## System defaults (preview)

| System | Rest rule (proposed) |
|--------|----------------------|
| Lune | 1 rest per quarter-phase week (by phase boundary, not weekday name) |
| Mix | 1 rest per 7- or 8-day week (last day) |
| Binary | 1 rest every 8 days (day 8) |
| Solar5 | 1 rest every 5 days |
| Dual | 1 rest per 7-day civil week; optional phase rest at full moon |

Details in each file under `04-systems/`.
