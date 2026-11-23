# Loop / Graph design

```mermaid
flowchart TD
 A[Collect paper source] --> B[Ingest: read / extract]
 B --> C[Check: claims, references, limits]
 C -->|Pass| D[Integrate paper note]
 C -->|Fail / uncertain| B
 D --> E[Update concept pages + links]
 E --> F[Update index + append log]
 F --> G[Query Wiki for teaching outline]
 G --> H[Draft HTML slides]
 H --> I[Slide check: traceability, clarity, navigation]
 I -->|Issues| G
 I -->|Pass| J[Final output]
 K[Periodic Lint] --> L[Check orphan pages, broken links, contradiction, stale info]
 L --> E
```

## What repeats?
- Ingest/check repeats for every new paper.
- Concept-page integration, index, and log updates recur.
- Slide checking can loop back to outline generation if unsupported claims or gaps are detected.
- Lint is a periodic maintenance cycle.

## Why?
Separate immutable source material from editable synthesis; verify before integration; keep links and index current; reuse compiled knowledge for queries instead of starting from scratch.
