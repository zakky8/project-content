# project-content

Editorial + PR content for Astarter Web4 AI Agent project.

## Structure

```
astarter-cointime-2026-05-24/
├── 01-long-form-feature.md         # ~1,850 words — Cointime Insight format
├── 02-news-flash.md                # ~245 words — Cointime flash format
├── 03-source-dossier.md            # Every claim → URL → tier (CLAUDE.md spec)
├── 04-analyst-notes-for-gk.md      # Material findings, open items, pitch logistics
└── astarter-cointime-package.docx  # All of the above packaged for GK review
```

## Workflow

1. GK reviews `.docx`, answers the 5 open items in `04-analyst-notes-for-gk.md`
2. Drafts updated based on GK feedback (commit per revision)
3. Final approved versions tagged `v1.0-cointime-ready`
4. Submit long-form via @Cointime curated channel; flash via flash-news pipeline

## Editorial discipline (per `C:\Users\rog\CLAUDE.md`)

- Primary sources only. Affiliate sites are starting points, never proof.
- Two-source minimum for any factual claim. Single-source claims marked UNVERIFIED.
- Exact quotes for any rule, number, or threshold.
- Every fact has `accessed_at_utc` and a tier.
- Contradictions logged, never silently resolved.
