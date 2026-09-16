# Choose a system (flowchart)

Start from **what must not drift**. For **why the world uses 7 today** (vs Egypt 10, Rome 8, USSR 5/6, etc.), see [other-weeks.md](other-weeks.md) and [why-seven.md](../05-synthesis/why-seven.md).

```mermaid
flowchart TD
  begin[Start]

  begin --> tide{Tides_or_moon_phase_critical?}
  tide -->|Yes| integ{Integer_days_required?}
  tide -->|No| solar{Solar_seasons_dominate?}

  integ -->|No| lune[Lune]
  integ -->|Yes| appt{Global_appointments_7d_rhythm?}
  appt -->|Yes| dual[Dual]
  appt -->|No| mix[Mix]

  solar -->|Yes| five{Minimize_week_year_epact?}
  solar -->|No| shift{Shift_planning_2_power_n?}

  five -->|Yes| s5[Solar5]
  five -->|No| bin[Binary]

  shift -->|Yes| bin
  shift -->|No| dual
```

```
Moon/tides critical? → integer days? → 7d appointments? → Lune / Mix / Dual
Else solar seasons? → minimize year epact? → Solar5 / Binary
```

## Match to files

| Outcome | Read |
|---------|------|
| Lune | [lune.md](../04-systems/lune.md) |
| Mix | [mix.md](../04-systems/mix.md) |
| Dual | [dual.md](../04-systems/dual.md) |
| Solar5 | [solar5.md](../04-systems/solar5.md) |
| Binary | [binary.md](../04-systems/binary.md) |
| Hex | [hex.md](../04-systems/hex.md) |

## Biology reminder

```mermaid
flowchart LR
  circ[Circadian_24h] --> day[Day_unit]
  day --> rest[Rest_policy_separate]
  rest -.->|not_proof_of_7| week[Week_optional]
```

[biology.md](../01-nature/biology.md)
