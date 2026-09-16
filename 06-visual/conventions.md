# Visual conventions (GitHub + Cursor)

Epact diagrams must render in **GitHub** and **Cursor/VS Code** Markdown preview without custom CSS or JavaScript.

## Allowed diagram types (preferred)

| Type | Keyword | Notes |
|------|---------|--------|
| Flowchart | `flowchart` | Default for logic, timelines, unit trees |
| XY chart | `xychart` | Bar/line; **quote** categorical labels |
| Pie | `pie` | Weight breakdowns; auto colors |
| Quadrant | `quadrantChart` | **Quote** quadrant labels; avoid bare `+` |
| Sequence | `sequenceDiagram` | Rare; use when interaction order matters |

## Use with caution

| Type | Issue | Fallback |
|------|--------|----------|
| `sankey` | Experimental; CSV-like lines | Flowchart with edge labels |
| `gantt` | Date formats vary by viewer | Flowchart LR day strips |
| `timeline` | Strict `period : event` syntax | ASCII strip |

## Not on GitHub (do not use)

- `classDef`, `style`, `linkStyle`, `click`
- HTML `<span style="color:...">` or colored `<table bgcolor=...>` (stripped)

## Syntax checklist (every new block)

1. **Node IDs:** camelCase or underscores - no spaces (`weekSeven`, not `week 7`).
2. **Edge labels with special chars:** use quotes: `-->|"4x week"|`.
3. **xychart x-axis categories:** always quoted: `["W5", "W6", "W7", "W8"]`.
4. **Avoid Unicode math in Mermaid:** use ASCII `x`, `-`, not `×`, `−`.
5. **Negative bar values:** avoid; chart **absolute** values + sign in caption.
6. **Keyword:** prefer `xychart` over legacy `xychart-beta`.
7. **Fallback:** ASCII or table **directly under** each diagram in `06-visual/`.

## Emphasis without CSS

### GitHub alerts

```markdown
> [!IMPORTANT]
> One sentence that must not be missed.

> [!NOTE]
> Context or definition.

> [!TIP]
> Where to look next in the repo.
```

### Emoji legend (optional, consistent)

| Emoji | Meaning in Epact |
|-------|------------------|
| 🌑 | Lunar / phase |
| ☀️ | Solar / tropical year |
| ⚖️ | Tradeoff / epact remainder |
| 📅 | Civil integer grid |
| 💤 | Rest (not week length) |

Use sparingly in README and synthesis; not required in method/search prose.

## Validation

Before committing diagram changes:

1. Grep: `` ```mermaid `` - each block passes checklist above.
2. Preview in Cursor: [README.md](../README.md), [systems-quadrant.md](systems-quadrant.md), [month-closure.md](month-closure.md), [intercalation-flow.md](intercalation-flow.md).
3. Optional: paste block into [Mermaid Live Editor](https://mermaid.live).

## File placement

- **Deep charts:** [06-visual/](README.md) index.
- **One compact diagram** per core doc in `00-method` … `05-synthesis` and each `04-systems` file - link here for more.
