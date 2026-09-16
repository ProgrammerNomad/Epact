# Unit: year

The **year** anchors seasons and long-term repetition. Epact uses the **tropical year** for Earth-bound life (agriculture, insolation).

## Mean tropical year

\[
Y = 365.242190402\ \text{mean solar days}
\]

(residual vs calendar grids stated in days or hours per century in system files)

## Sidereal vs tropical

- **Tropical:** equinox precession built in - **seasons** repeat on this scale.
- **Sidereal:** fixed stars - astronomy; seasons drift on ~26 ky precession cycle if used naively for seasons.

Solar-first systems (Binary, Solar5) may ignore lunar months entirely; lunar-first systems (Lune, Mix, Dual) still need **year epact** via leap months (Metonic family) or drift.

## Seasons

Four seasons from equinoxes/solstices are **unequal in day count** because:

- Orbit is elliptical (Earth moves faster near perihelion - currently northern winter slightly shorter in days than summer, in the sense of orbital speed effects on solstice-to-solstice intervals).

A calendar may:

- use **quarter-years** of ~91.31 d mean each, or
- mark ** astronomical instants** only (no equal-season months).

## Week–year coupling

| W | Weeks per year (365.242 / W) | Nearest integer |
|---|------------------------------|-----------------|
| 5 | 73.048 | 73 |
| 6 | 60.874 | 61 |
| 7 | 52.177 | 52 |
| 8 | 45.655 | 46 |

\(W=5\) minimizes fractional error to the year among small integers - relevant to **Solar5**.

## Intercalation locus

Year epact can be absorbed by:

- leap **day** (solar),
- leap **month** (lunisolar),
- leap **week** (rare designs),
- **unassigned epact days** (see [intercalation.md](../03-search/intercalation.md)).

Each candidate system chooses one primary mechanism.
