# Composite week scores (W = 1 … 30)

Weights: [scoring.md](../00-method/scoring.md) **Score_int** (no +0.10 circadian constant).

## Top candidates (bar)

```mermaid
xychart
    title "Score_int by week length top values"
    x-axis ["5", "6", "7", "8", "10", "14", "28"]
    y-axis "Score" 0.55 --> 0.75
    bar [0.715, 0.729, 0.723, 0.702, 0.632, 0.602, 0.559]
```

## Full range (line)

```mermaid
xychart
    title "Score_int W=1 to 30"
    x-axis [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30]
    y-axis "Score" 0.35 --> 0.75
    line [0.412, 0.486, 0.605, 0.555, 0.715, 0.729, 0.723, 0.702, 0.617, 0.632, 0.550, 0.528, 0.541, 0.602, 0.562, 0.566, 0.425, 0.490, 0.405, 0.452, 0.420, 0.430, 0.441, 0.502, 0.435, 0.519, 0.463, 0.559, 0.444, 0.546]
```

## ASCII leaderboard

```
W=6  ████████████████████ 0.729  ← Score_int leader
W=7  ███████████████████▊ 0.723  ← best quarter proximity
W=5  ███████████████████▌ 0.715  ← strong Y
W=8  ███████████████████  0.702  ← binary scheduling
```

Legacy Score (+0.10 C): 6=0.829, 7=0.823, 5=0.815.

Full table: [integer-weeks.md](../03-search/integer-weeks.md).
