# Mixed 59-day / 8-week pattern

Repeating block from [mix.md](../04-systems/mix.md): **5x7 + 3x8 = 59 days**.

## Week lengths (flowchart)

```mermaid
flowchart LR
  W1["W1 7d"] --> W2["W2 7d"]
  W2 --> W3["W3 8d"]
  W3 --> W4["W4 7d"]
  W4 --> W5["W5 7d"]
  W5 --> W6["W6 8d"]
  W6 --> W7["W7 7d"]
  W7 --> W8["W8 8d"]
```

Cumulative days: 7, 14, 22, 29, 36, 44, 51, **59**.

## Rest days (last day of each week)

```mermaid
flowchart TB
  R1["Day 7 W1 rest"]
  R2["Day 14 W2 rest"]
  R3["Day 22 W3 rest"]
  R4["Day 29 W4 rest"]
  R5["Day 36 W5 rest"]
  R6["Day 44 W6 rest"]
  R7["Day 51 W7 rest"]
  R8["Day 59 W8 rest"]
  R1 --> R2 --> R3 --> R4 --> R5 --> R6 --> R7 --> R8
```

## ASCII strip

```
|←7→|←7→|←──8──→|←7→|←7→|←──8──→|←7→|←──8──→|
  W1   W2    W3     W4   W5    W6     W7    W8
  R    R     R      R    R     R      R     R     (R = rest on last day)
```

Mean week = 59/8 = **7.375 d**.
