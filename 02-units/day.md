# Unit: day

The **day** is the atomic unit of civil scheduling. Every other unit is a counted bundle of days (or a parallel overlay).

## Candidates for “one day”

| Definition | Period | Pros | Cons |
|------------|--------|------|------|
| **Mean solar day** | 86400 s | Global clocks agree; stable date line. | Ignores sundial variation. |
| **True solar day** | varies | Local noon alignment. | Uneven; bad for networks. |
| **Sidereal day** | 0.99727 solar d | Star observations. | 366.26… per year; awkward civil grid. |
| **Tidal (lunar) day** | 1.03505 solar d | Coastal rhythm. | Latitude/coast dependent; drifts vs clocks. |
| **Light day** | 0–24 h by season/latitude | Ecological daylight. | Fails at poles; not portable. |

**Epact default:** **mean solar day** for all five systems in `04-systems/`.

## Sub-day structure (informative, not week drivers)

- **Circadian** entrainment → wake/sleep within solar day.
- **Ultradian** sleep cycles → 90–110 min; no impact on choice of \(W\).

## Polar and high-latitude note

If “day” means **sun above horizon**, winter contains **zero** such days inside the Arctic/Antarctic circle. A universal calendar cannot use light-day as the only day without **dual labels** (clock day vs photoperiod index).

## Design questions

1. Does the date roll at **midnight local**, **UTC**, or **solar noon**?
2. Are **leap seconds** ignored (POSIX style) or applied (rare discontinuity)?

Epact assumes **smooth mean solar days**; leap-second policy is out of scope but acknowledged as tiny epact on the rotation scale.
