# Sources

Epact uses **mean modern values** for astronomy and **standard calendar-history references** for civil-time claims. History citations are **description of lock-in**, not proof of a natural week ([axioms.md](axioms.md)).

## Astronomical constants

| Quantity | Typical source | Used in |
|----------|----------------|---------|
| Synodic month (mean) | Chapront-Touzé & Chapront lunar theory; summaries e.g. Wikipedia *Lunar month* (29.530588861 d) | [constants.md](constants.md), scoring |
| Tropical year (mean) | Simon et al. 1994; IAU/Paris Observatory summaries (~365.24219 d) | [constants.md](constants.md), scoring |
| Earth rotation / sidereal day | IERS conventions; USNO *Astronomical Constants* | [constants.md](constants.md) |
| PDG / IAU roundings | 365.242189 d tropical (equinox-to-equinox, 2020-era tables) | Residual discussion only |

Secular drift (tidal slowing, etc.) is noted in [open-questions.md](../05-synthesis/open-questions.md); this repo does not retune constants over millennia.

## Calendar history (non-exhaustive)

General references for week length, intercalation, and reform calendars:

- E. G. Richards, *Mapping Time: The Calendar and Its History* (Oxford University Press).
- D. E. Duncan, *Calendar: Humanity’s Epic Struggle to Determine a True and Accurate Year* (Avon/HarperCollins).

Topic → where Epact mentions it:

| Topic | Epact file | Typical coverage in references above |
|-------|------------|--------------------------------------|
| Roman **8-day nundinae** (market week) | [binary.md](../04-systems/binary.md), [why-seven.md](../05-synthesis/why-seven.md) | Republican/Imperial market cycles vs later 7-day week |
| **7-day week** diffusion (Judaism, Christianity, empire, ISO) | [why-seven.md](../05-synthesis/why-seven.md), [glossary.md](../glossary.md) | Hellenistic/Roman adoption; modern global standard |
| Egyptian **10-day** decades; **12×30 + epagomenal** year | [why-seven.md](../05-synthesis/why-seven.md), [month.md](../02-units/month.md) | Old Kingdom through Ptolemaic administrative year |
| Chinese **xun** (10-day) | [why-seven.md](../05-synthesis/why-seven.md) | Traditional lunisolar administration |
| French Republican **décade** (10-day) and decimal **day** | [why-seven.md](../05-synthesis/why-seven.md), [solar5.md](../04-systems/solar5.md), [day.md](../02-units/day.md) | 1793–1805 reforms |
| Soviet **continuous work week** (5- then 6-day, 1929–1940) | [why-seven.md](../05-synthesis/why-seven.md), [rest.md](../02-units/rest.md) | Early Soviet calendar experiments |
| Maya **Haab** (18×20+5), **Tzolkʼin** (13×20 ritual) | [why-seven.md](../05-synthesis/why-seven.md), [month.md](../02-units/month.md) | Mesoamerican parallel counts |
| Java/Bali **pawukon** (overlapping 3/5/7-day layers) | [why-seven.md](../05-synthesis/why-seven.md), [dual.md](../04-systems/dual.md) | Balinese calendar overlays |
| West African market intervals (e.g. 4/8 days) | [why-seven.md](../05-synthesis/why-seven.md) | Ethnographic market rhythms |
| **Hijri** lunar year (~354.37 d); Hebrew/Chinese **Metonic-family** leap months | [year.md](../02-units/year.md) | Lunisolar vs pure lunar year |
| Day epoch: sunset, sunrise, midnight; unequal hours | [day.md](../02-units/day.md) | Babylonian, Egyptian, Roman hour systems |

Do not treat these references as endorsement of any single week length; they document **human choices** and **diffusion**.

## Biology (order-of-magnitude)

Circaseptan and related claims: see primary literature summarized in [biology.md](../01-nature/biology.md). Epact does not use biology to prove W=7.
