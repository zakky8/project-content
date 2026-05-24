# project-content

Editorial + PR content for Astarter Web4 AI Agent project.

## Latest delivery — `astarter-cointime-2026-05-24/`

| # | File | Type | Purpose |
|---|---|---|---|
| 01 | `01-long-form-feature.md` | Long-form EN (~1,850w) | Cointime Insight format |
| 02 | `02-news-flash.md` | News flash EN (~245w) | Cointime flash format |
| 03 | `03-source-dossier.md` | Citations | Every claim → URL → tier |
| 04 | `04-analyst-notes-for-gk.md` | Notes | Findings + open items |
| 05 | `05-cn-long-form.md` | Long-form CN | PANews / BlockBeats voice |
| 06 | `06-cn-news-flash.md` | News flash CN | Flash format CN |
| 07 | `07-x-thread-en.md` | X/Twitter EN | 10-tweet thread |
| 08 | `08-x-thread-cn.md` | X/Twitter CN | 10-tweet thread |
| 09 | `09-telegram-en.md` | Telegram EN | Channel post |
| 10 | `10-telegram-cn.md` | Telegram CN | Channel post |
| 11 | `11-pitch-email-en.md` | Email EN | To Nicole / Cointime |
| 12 | `12-pitch-email-cn.md` | Email CN | To Nicole / Cointime |
| 13 | `13-panews-syndication.md` | Syndication EN | Data-heavy PANews variant |
| 14 | `14-press-release.md` | Press release EN | Newswire format |
| 15 | `15-headlines-bank.md` | Headlines bank | 20 candidates EN+CN |
| — | `design-philosophy.md` | Design philosophy | *Quiet Substrate* manifesto |
| — | `astarter-cointime-package.docx` | DOCX | Full package for GK |
| — | `astarter-cointime-package.pdf` | PDF | Same package, preview-friendly |
| — | `astarter-pitch-deck.pptx` | PPTX | 10-slide internal deck |
| — | `astarter-hero-1180x480.png` | Image | Hero banner |

## Workflow

1. GK reviews `.docx` / `.pdf` / `.pptx`, answers the 5 open items in `04-analyst-notes-for-gk.md`
2. Drafts updated based on GK feedback (commit per revision)
3. Final approved versions tagged `v1.0-cointime-ready`
4. Distribution:
   - **Long-form** → @Cointime curated channel
   - **News flash** → Cointime flash-news pipeline
   - **PANews syndication variant** → PANews / BlockBeats / TechFlow / 深潮
   - **Press release** → wire services
   - **X thread** → @AstarterDefiHub (composite hero image first)
   - **Telegram** → Astarter official TG (composite hero image first)

## Editorial discipline (per `C:\Users\rog\CLAUDE.md`)

- Primary sources only. Affiliate sites are starting points, never proof.
- Two-source minimum for any factual claim. Single-source claims marked UNVERIFIED.
- Exact quotes for any rule, number, or threshold.
- Every fact has `accessed_at_utc` and a tier.
- Contradictions logged, never silently resolved.

## Asset workflow notes

- Hero PNG has a clean reticle space top-left — **composite the real Astarter logo in Figma** before publishing. AI cannot render brand-specific marks reliably.
- PPTX uses the same *Quiet Substrate* palette (DEEP `#0F0820`, MIDV `#2D1B5F`, VIOLET `#6F00FF`, CYAN `#00E5FF`) so all assets are visually unified.
- PDF is generated from the .docx via `docx2pdf` — re-run `pip install docx2pdf && python -c "from docx2pdf import convert; convert('X.docx','X.pdf')"` after any edit.
