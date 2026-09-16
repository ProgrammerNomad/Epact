# Six systems: lunar vs solar priority

Subjective placement for **discussion** (0 = low, 1 = high). Not additional computed scores.

```mermaid
quadrantChart
    title Calendar systems lunar vs solar fidelity
    x-axis Low lunar --> High lunar
    y-axis Low solar --> High solar
    quadrant-1 "Lunar and solar strong"
    quadrant-2 "Lunar-first"
    quadrant-3 "Minimal astronomy"
    quadrant-4 "Solar-first"
    Lune: [0.92, 0.58]
    Mix: [0.78, 0.55]
    Dual: [0.88, 0.62]
    Hex: [0.48, 0.78]
    Binary: [0.12, 0.72]
    Solar5: [0.15, 0.88]
```

```
        High solar
            |  Solar5
            |  Binary
            |        Dual
            |   Lune  Mix
        Low solar +------------------ High lunar
```

## Complexity vs honesty

```mermaid
quadrantChart
    title Burden vs astronomical honesty
    x-axis Simple --> Complex
    y-axis Hides epact --> Exposes epact
    quadrant-1 "Simple and honest"
    quadrant-2 "Complex and honest"
    quadrant-3 "Simple but misleading"
    quadrant-4 "Complex and opaque"
    Solar5: [0.35, 0.45]
    Binary: [0.40, 0.70]
    Hex: [0.45, 0.80]
    Mix: [0.55, 0.85]
    Lune: [0.50, 0.95]
    Dual: [0.75, 0.90]
```

## Fallback bars (same intent as quadrants)

Criteria from [comparison.md](../05-synthesis/comparison.md), encoded 0-3:

```mermaid
xychart
    title "Lunar quarter fidelity 0-3"
    x-axis ["Lune", "Mix", "Dual", "Hex", "Binary", "Solar5"]
    y-axis "Score" 0 --> 3
    bar [3, 2, 3, 1, 0, 0]
```

```mermaid
xychart
    title "Integer circadian lock 0-3"
    x-axis ["Lune", "Mix", "Dual", "Hex", "Binary", "Solar5"]
    y-axis "Score" 0 --> 3
    bar [1, 3, 3, 3, 3, 3]
```

| System | Lunar (0-3) | Circadian lock (0-3) |
|--------|-------------|----------------------|
| Lune | 3 | 1 |
| Mix | 2 | 3 |
| Dual | 3 | 3 |
| Hex | 1 | 3 |
| Binary | 0 | 3 |
| Solar5 | 0 | 3 |

See system docs in [04-systems/](../04-systems/).
