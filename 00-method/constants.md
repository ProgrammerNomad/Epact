# Constants

All primary values are in **mean solar days** unless noted. One mean solar day = **86 400 s** (SI).

Ephemeris values drift slowly (secular trends). This table uses modern mean values suitable for structural calendar design, not navigation at the arcsecond level.

## Rotation and “day”

| Quantity | Symbol | Value (mean solar days) | Notes |
|----------|--------|-------------------------|--------|
| Mean solar day | D | 1.000000 | Civil day basis |
| Mean sidereal day | - | 0.9972695664 | Earth spin vs fixed stars |
| Lunar day (tidal) | - | 1.035050 | ~24 h 50.5 min; Moon’s return overhead |

Sidereal day source: Earth rotation angle rate (IAU 2000); see USNO *Astronomical Constants* and IERS conventions.

## Moon (Earth–Moon system)

| Month type | Value (d) | Definition |
|------------|-----------|------------|
| **Synodic** | **29.530588861** | New moon → new moon (phases) |
| Sidereal | 27.321661554 | Orbit vs stars |
| Tropical | 27.321582252 | Orbit vs vernal point |
| Anomalistic | 27.554549886 | Perigee → perigee |
| Draconic | 27.212220815 | Node → node |

## Derived lunar intervals

| Name | Formula | Value (d) |
|------|---------|-----------|
| Lunar quarter (phase) | synodic / 4 | **7.382647215** |
| Spring–neap half-cycle | synodic / 2 | **14.765294430** |
| Fortnight (approx.) | synodic / 2 | 14.765… |

Spring tides occur near new and full moon; neaps near first and third quarter - tied to the **synodic** month, not the sidereal month alone.

## Sun and year

| Quantity | Value (d) | Notes |
|----------|-----------|--------|
| **Tropical year** | **365.242190402** | Equinox to equinox (mean) |
| Sidereal year | 365.256363004 | Orbit vs stars |

## Ratios used in continued-fraction thinking

| Ratio | Decimal | First useful convergents (denominator = years or months) |
|-------|---------|----------------------------------------------------------|
| Tropical year / synodic month | 12.368266… | 19 years ≈ 235 months (Metonic) |
| Synodic month / lunar quarter | 4 (exact) | Quarter is exactly ¼ synodic in mean astronomy |
| Lunar quarter / solar day | 7.382647… | See [mixed-weeks.md](../03-search/mixed-weeks.md) |

## Biology (order-of-magnitude, not SI definitions)

| Rhythm | Typical period | Role in Epact |
|--------|----------------|---------------|
| Circadian (free-run) | ~24.2 h | Locks to light; defines **rest within a day**, not week length |
| Ultradian (sleep) | ~90–110 min | Sub-day structure only |
| Infradian (sleep duration) | multi-day, individual | Not a universal 7 d clock |
| Menstrual (approx.) | ~29.5 d | Near synodic month; not a week driver |

## Reference notes

Full bibliography and history pointers: [sources.md](sources.md).

## Working precision

In prose and tables, **four decimal places** on days is enough for week-length search. Residuals for winning approximations should also be stated in **hours per cycle** where intuitive.
