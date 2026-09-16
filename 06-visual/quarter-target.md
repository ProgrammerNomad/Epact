# Distance to lunar quarter (7.382647 d)

Target: mean **phase quarter** = synodic month / 4.

## Proximity score Q_prox(W)

```mermaid
xychart
    title "Quarter proximity Q_prox 1 = exact 7.383 d week"
    x-axis ["5", "6", "7", "8", "9", "10", "11", "12"]
    y-axis "Q_prox" 0 --> 1
    bar [0.677, 0.813, 0.948, 0.916, 0.781, 0.645, 0.510, 0.375]
```

## Integer vs exact quarter

```mermaid
xychart
    title "Week length in days vs exact quarter"
    x-axis ["Exact Q", "W6", "W7", "W8"]
    y-axis "Days" 6.5 --> 8.5
    bar [7.383, 6, 7, 8]
```

| | Days |
|---|------|
| Exact Q | 7.383 |
| W6 | 6 |
| W7 | 7 |
| W8 | 8 |

## Mixed mean (59/8 block)

```mermaid
pie showData
    title "59-day block week lengths"
    "7-day weeks 5" : 35
    "8-day weeks 3" : 24
```

Mean = 59/8 = **7.375 d** (11 min short of 7.383 d per week).

## ASCII

```
Exact quarter     7.383 d  |-----------------|  target
W=7               7.000 d  |--------------    |  short ~9.2 h / quarter
W=8               8.000 d  |-----------------|--+  long ~14.8 h / quarter
Mix 59/8          7.375 d  |----------------|   |  short ~11 min / week
```

See [mixed-weeks.md](../03-search/mixed-weeks.md).
