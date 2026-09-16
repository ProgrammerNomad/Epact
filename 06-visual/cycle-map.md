# Cycle map

Mean periods in **mean solar days**. Edges show division or mismatch.

```mermaid
flowchart TB
  subgraph earth [Earth rotation]
    D[MeanSolarDay_1.000]
    Dsid[SiderealDay_0.997]
    Dtide[TidalDay_1.035]
  end

  subgraph moon [Moon]
    Syn[SynodicMonth_29.531]
    Sid[SiderealMonth_27.322]
  end

  subgraph derived [Derived]
    Q[LunarQuarter_7.383]
    SN[SpringNeap_14.765]
  end

  subgraph sun [Sun]
    Ty[TropicalYear_365.242]
  end

  Syn -->|exact_div_4| Q
  Syn -->|exact_div_2| SN
  Ty -.->|ratio_12.368_not_integer| Syn
  D -.->|not_multiple| Q
  Q -.->|not_integer| D
```

## Incommensurability (concept)

```mermaid
flowchart LR
  req1[Whole_solar_days]
  req2[Exact_lunar_quarters]
  req3[Fixed_clock_boundaries]
  req4[Exact_tropical_year]
  impossible[No_single_integer_W]

  req1 --> impossible
  req2 --> impossible
  req3 --> impossible
  req4 --> impossible
```

## ASCII fallback

```
Tropical year 365.242 d  ──×──  Synodic month 29.531 d  (ratio ≈ 12.368)
Synodic / 4 = 7.383 d    ──×──  Integer day grid      (7.383 ∉ ℤ)
Four × 7 d = 28 d         ──×──  One lunation          (−1.53 d)
```

See [00-method/impossibility.md](../00-method/impossibility.md).
