# Where epact goes

When two cycles are forced together, remainder must be stored somewhere.

## Decision flow

```mermaid
flowchart TD
  start[Two_cycles_mismatch]
  start --> q1{Must_weeks_stay_integer?}
  q1 -->|No| lune[Phase_quarter_week_Lune]
  q1 -->|Yes| q2{Lunar_month_must_close?}
  q2 -->|Yes| mix[Mix_plus_epact_day]
  q2 -->|No| q3{Priority_solar_year?}
  q3 -->|Strong| solar5[Solar5_leap_day]
  q3 -->|Binary_splits| binary[Binary_360_plus_epact]
  q2 -->|Both| dual[Dual_overlay]
```

## Epact sinks (flowchart)

Illustrative **day-equivalents per cycle** (not conserved flux):

```mermaid
flowchart LR
  LQ[Lunar_quarter_error]
  LQ -->|"0.53 d"| ED1[Epact_day]
  LQ -->|"0.38 d"| PI[Phase_instant]
  WY[Week_year_error]
  WY -->|"0.24 d"| LD[Leap_day]
  WY -->|"1.24 d"| ED2[Epact_day]
  MY[Month_year_error]
  MY -->|"7 mo / 19 y"| LM[Leap_month]
  BY[Binary_year_error]
  BY -->|"5.24 d"| EB[Epact_block]
```

| Source | Sink | Scale |
|--------|------|-------|
| Lunar quarter error | Epact day | ~0.53 d / lunation |
| Lunar quarter error | Phase instant | ~0.38 d / quarter |
| Week vs year | Leap day | ~0.24 d / year |
| Week vs year | Epact day | ~1.24 d / year |
| Month vs year | Leap month | 7 / 19 years |
| Binary 360 vs year | Epact block | ~5.24 d / year |

## ASCII

```
Mismatch type          Typical sink
─────────────────────────────────────
28 d vs 29.53 d month  → 1 epact day / lunation (Mix)
364 d vs 365.24 y      → 1–2 epact days / year (Dual civil)
360 d vs 365.24 y      → 5-day epact block (Binary)
7.38 d quarter         → phase instant OR 7/8 mix (Lune / Mix)
```

Details: [intercalation.md](../03-search/intercalation.md).
