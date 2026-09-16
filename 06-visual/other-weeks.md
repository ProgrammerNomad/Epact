# Other week lengths (historical targets)

Maps **why** some cultures did not use 7 - same design knobs as Epact. Full table: [why-seven.md](../05-synthesis/why-seven.md).

```mermaid
flowchart TD
  start[What_matters_most]
  start --> moon{Moon_phases}
  moon -->|Yes| mixW[7_or_8_or_Mix]
  moon -->|No| solar{Solar_year}
  solar -->|Yes| tenW[5_or_10_Solar5]
  solar -->|No| market{Market_halves}
  market -->|Yes| eightW[8_Binary]
  market -->|No| restOnly{Rest_shifts}
  restOnly -->|Yes| fiveSix[5_or_6_rest]
  restOnly -->|No| overlay[Dual_overlays]
```

## ASCII

```
Priority          Example W    Epact file
─────────────────────────────────────────
Moon + integer    7, 8, mix    Mix, Lune
Solar year        5, 10        Solar5
Market / 2^n      8            Binary
Rest / factory    5, 6         rest.md
Several rhythms   3+5+7        Dual
Ritual counts     13, 20       cycles.md (not a civil week)
Global today      7            copied package (why-seven.md)
```
