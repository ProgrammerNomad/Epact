# Score components (W = 5, 6, 7, 8)

Same weights as [scoring.md](../00-method/scoring.md). Compare **why** totals differ.

## Moon alignment M(W)

```mermaid
xychart
    title "M(W) lunar month fit"
    x-axis ["W5", "W6", "W7", "W8"]
    y-axis "M" 0.5 --> 1
    bar [0.906, 0.922, 0.781, 0.691]
```

| W | M |
|---|---|
| 5 | 0.906 |
| 6 | 0.922 |
| 7 | 0.781 |
| 8 | 0.691 |

## Quarter proximity Q_prox(W)

```mermaid
xychart
    title "Q_prox(W) closeness to 7.383 d"
    x-axis ["W5", "W6", "W7", "W8"]
    y-axis "Q_prox" 0.6 --> 1
    bar [0.677, 0.813, 0.948, 0.916]
```

## Tropical year alignment Y(W)

```mermaid
xychart
    title "Y(W) tropical year fit"
    x-axis ["W5", "W6", "W7", "W8"]
    y-axis "Y" 0 --> 1
    bar [0.952, 0.874, 0.823, 0.655]
```

## Divisibility D_norm(W)

```mermaid
xychart
    title "D_norm(W) scheduling splits"
    x-axis ["W5", "W6", "W7", "W8"]
    y-axis "D_norm" 0 --> 1
    bar [0.333, 0.833, 0.333, 0.750]
```

## Score_int (same four W)

```mermaid
xychart
    title "Score_int(W)"
    x-axis ["W5", "W6", "W7", "W8"]
    y-axis "Score" 0.68 --> 0.74
    bar [0.715, 0.729, 0.723, 0.702]
```

## Stacked intuition (ASCII)

```
Component      W=5    W=6    W=7    W=8
─────────────────────────────────────────
M (moon)       ███    ███    ██     ██
Q (quarter)    ██     ██▊    ███▊   ███▋
Y (year)       ███▊   ███▊   ██▋    ██▌
D (divide)     █      ██▊    █      ██▌
─────────────────────────────────────────
Score_int      .715   .729   .723   .702
```

W=6 leads **Score_int**; W=7 wins **quarter** and **S**; W=6 wins **Y** over 7; W=5 wins **Y** among small W.
