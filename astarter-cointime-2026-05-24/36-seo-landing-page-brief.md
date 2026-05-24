# SEO + Landing Page Brief

**For:** Astarter web team (or whoever owns astarter.io content)
**Purpose:** convert a single press spike into 12 months of organic discovery

A Cointime article generates a spike. SEO turns that spike into a tail.

---

## I. Target keywords (priority-ordered)

### Tier 1 — own these or lose them

| Keyword | Monthly search vol (est) | Current ranking | Target ranking |
|---|---|---|---|
| AI agent settlement | 1.5K | Not ranking | Top 3 |
| DeFAI | 8K | Not ranking | Top 5 |
| Web 4.0 crypto | 12K | Not ranking | Top 10 |
| AI agent infrastructure | 6K | Not ranking | Top 5 |
| autonomous AI agent economy | 2K | Not ranking | Top 3 |
| Cardano DeFi infrastructure | 4K | Not ranking | Top 10 |
| agent-to-agent settlement | 800 | Not ranking | Top 3 |
| AA token Cardano | 1K | Not ranking | Top 3 |
| Astarter token | 3K | Not ranking | Top 1 |

### Tier 2 — long-tail content opportunities

- "what is DeFAI"
- "how do AI agents transact on chain"
- "best AI agent crypto projects 2026"
- "DePIN AI agent infrastructure"
- "agent-collateralized credit"
- "DeFi for AI agents"
- "Astarter vs Olas vs Virtuals"
- "Astarter UXLINK partnership"
- "EMURGO portfolio companies"
- "Cardano AI projects"

### Tier 3 — defensive (own our own brand)

- "astarter" / "Astarter"
- "Astarter price" / "AA price"
- "Astarter review"
- "Astarter scam" (yes, defensive — own the SERP)
- "Astarter Twitter"
- "Astarter roadmap"

---

## II. Landing page hierarchy (recommended)

### astarter.io/ (homepage)
**Primary keyword:** AI Agent settlement infrastructure
**H1:** Settlement Infrastructure for the AI Agent Economy
**Above-fold copy:** Cardano-native financial primitives for autonomous AI agents — combining AI Agent, DePIN, and DeFAI under a single coordinated stack.
**CTAs:** [Read the thesis] [Quickstart for developers]
**Below-fold sections:** thesis · stack · alliance · token · roadmap · community

### astarter.io/defai
**Primary keyword:** DeFAI
**H1:** What Is DeFAI? The Settlement Layer for the AI Agent Economy
**Purpose:** rank for the category-defining term; become the canonical reference

### astarter.io/agent-settlement
**Primary keyword:** AI agent settlement / agent-to-agent settlement
**H1:** How Agent-to-Agent Settlement Works
**Purpose:** technical landing for builders + analyst-grade explainer

### astarter.io/web4
**Primary keyword:** Web 4.0 crypto
**H1:** Web 4.0 — The Agent Economy Layer of Crypto
**Purpose:** thought-leadership content rank

### astarter.io/uxlink-alliance
**Primary keyword:** Astarter UXLINK
**H1:** The Astarter × UXLINK Strategic Alliance
**Purpose:** own the partnership SERP + permanent landing for press

### astarter.io/token
**Primary keyword:** AA token Cardano
**H1:** The AA Token
**Purpose:** answer all common token questions in one place

### astarter.io/research
**Primary keyword:** DeFAI research / AI agent crypto research
**H1:** Astarter Research Desk
**Purpose:** home for thought-leadership pieces (`35-thought-leadership-original-data.md` lives here)

### astarter.io/vs/[competitor]
**Primary keyword:** Astarter vs [Olas / Virtuals / Fetch]
**H1:** Astarter vs [Competitor]: A Layer-Map Comparison
**Purpose:** comparison-SEO play; rank for SERPs people search before they commit

---

## III. On-page SEO checklist (every new page)

- [ ] Title tag: 50–60 chars, includes primary keyword first
- [ ] Meta description: 140–160 chars, includes primary keyword + CTA verb
- [ ] H1: includes primary keyword, exactly one H1 per page
- [ ] H2s: 4–6, include secondary keywords naturally
- [ ] First paragraph: primary keyword in first 100 words
- [ ] Internal links: 3–5 to other Astarter pages
- [ ] External links: 2–3 to authoritative sources (Messari, Decrypt, EMURGO)
- [ ] Alt text on every image, includes relevant keyword
- [ ] URL slug: short, keyword-aligned, hyphen-separated
- [ ] Canonical URL set
- [ ] OG image: 1200×630, branded (use existing Twitter card from visual system)
- [ ] Twitter card meta (`summary_large_image`)
- [ ] Structured data: `Article` / `Organization` / `Product` as appropriate
- [ ] Page load time: <2s on 4G
- [ ] Mobile-responsive (test on iPhone SE)
- [ ] No 404s; no chains of redirects
- [ ] Sitemap.xml updated
- [ ] robots.txt allows indexing (except admin areas)

---

## IV. Structured data (schema.org)

### For homepage and main landing pages

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Astarter",
  "url": "https://astarter.io",
  "logo": "https://astarter.io/assets/logo.png",
  "description": "Settlement infrastructure for the autonomous AI Agent economy.",
  "sameAs": [
    "https://twitter.com/AstarterDefiHub",
    "https://medium.com/@AstarterDefiHub",
    "https://github.com/astarter"
  ],
  "foundingDate": "2021-09-16",
  "founders": [
    { "@type": "Organization", "name": "EMURGO" }
  ]
}
```

### For research / thought-leadership pieces

```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "The DeFAI Layer Map",
  "datePublished": "2026-05-24",
  "author": { "@type": "Organization", "name": "Astarter Research Desk" },
  "publisher": { "@type": "Organization", "name": "Astarter", "logo": {...} },
  "image": "https://astarter.io/og/defai-layer-map.png",
  "description": "Original analysis on the four-layer architecture of the AI Agent economy..."
}
```

### For product / token pages

```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "AA Token",
  "brand": "Astarter",
  "category": "Cryptocurrency",
  "description": "Native token of Astarter — fixed 100M supply, settlement and governance utility."
}
```

---

## V. Content gap analysis

These pieces should exist by T+30 to fully cover the SEO opportunity:

| Asset | Target keyword | Priority |
|---|---|---|
| /defai (canonical explainer) | DeFAI | P0 |
| /agent-settlement (how it works) | agent-to-agent settlement | P0 |
| /web4 (thought-leadership canonical) | Web 4.0 crypto | P0 |
| /research/defai-layer-map (this piece) | DeFAI research | P0 |
| /vs/olas, /vs/virtuals, /vs/fetch | Astarter vs X | P1 |
| /uxlink-alliance | Astarter UXLINK | P1 |
| /token (full FAQ + utility) | AA token | P1 |
| /developers (quickstart hub) | Astarter SDK | P1 |
| /blog/ai-agent-economy-explained | AI agent economy | P2 |
| /blog/depin-explained | DePIN | P2 |
| /press (press kit hub) | Astarter press | P2 |
| /research/quarterly-letter | AI agent infrastructure research | P2 |

---

## VI. Link building (earned, not bought)

### Tier 1 backlink targets

| Source | Approach | Expected difficulty |
|---|---|---|
| Cointime article (launch piece) | Already aligned | Easy |
| CoinDesk piece (if embargo lands) | Earned via embargo | Medium |
| Decrypt piece | Earned via outreach | Medium |
| CoinGecko / CoinMarketCap project page | Ensure current and complete | Easy |
| DefiLlama protocol page | Ensure current | Easy |
| Messari project profile | Submit update with new positioning | Easy |
| Cardano Foundation ecosystem map | Confirm inclusion | Easy |
| EMURGO portfolio page | Confirm inclusion | Easy |
| Arbitrum / Sol AI & DePIN ecosystem maps | Submit (when multi-chain ships) | Medium |

### Tier 2 backlink targets

- DePIN Hub directory submission
- AI Agent project directories (multiple)
- Cardano DeFi directories
- Crypto job board listings (engineering hires)
- Conference speaker pages (when speaking slots land)
- Podcast episode show-notes pages
- KOL personal blogs that cover us
- Reddit submissions (already in `19-reddit-posts.md`)

### Anti-pattern: don't do these

- Buying backlinks from PBN / link farms
- Paid placements that aren't disclosed
- Comment spam on other crypto sites
- Forum signature backlinks
- Anything Google's spam filter would catch

---

## VII. Analytics + tracking

### Must-track events

- Pageviews per landing page (weekly cohort)
- Quickstart completions (developer signups proxy)
- "Read full thesis" CTA clickthrough rate
- Outbound clicks to Cointime article
- Newsletter signups
- Discord / Telegram joins from /community page
- GitHub stars on main repo

### Must-track funnel

1. Search / press click → landing page
2. Landing page → read full thesis OR Quickstart
3. Read / Quickstart → community join OR newsletter signup
4. Community / newsletter → ongoing engagement

Measure conversion rate at each step. If conversion >5% at each step, the funnel is healthy. If <2% at any step, that's the optimization priority.

### Tools

- **Plausible** (recommended over GA for privacy + simplicity)
- **Search Console** (free, indispensable)
- **Ahrefs / Semrush** (paid — for keyword tracking)
- **Bing Webmaster Tools** (free, complements Google)

---

## VIII. SEO timeline

### T-7 to T-0 (pre-launch)
- All new landing pages live (homepage redesign, /defai, /agent-settlement, /web4, /uxlink-alliance)
- Structured data deployed
- Sitemap submitted to Search Console
- OG / Twitter card meta in place
- Internal linking audit complete

### T+0 to T+7 (launch wave)
- Submit Cointime article URL to Search Console for indexing
- Submit /uxlink-alliance to Search Console
- Monitor branded search volume spike
- Triage any 404s or broken links surfaced by launch traffic

### T+7 to T+30 (consolidation)
- Publish /research/defai-layer-map (thought-leadership canonical)
- Publish /vs/[Olas/Virtuals/Fetch] comparison pages
- First backlink outreach round
- First retro on what ranked and what didn't

### T+30 to T+90 (compounding)
- Weekly publishing rhythm (one piece per week)
- Backlink expansion
- Iterate on top-performing pages (refresh content, expand)
- Begin to track ranking improvements for Tier 1 keywords

---

## IX. Performance targets

| Metric | T+30 | T+90 | T+180 |
|---|---|---|---|
| Indexed pages | 25 | 60 | 100+ |
| Branded search volume | +200% baseline | +400% baseline | +600% baseline |
| Tier 1 keyword rankings (avg) | 30 | 15 | 8 |
| Organic monthly visitors | 5K | 25K | 60K |
| Referring domains | 30 | 80 | 200 |
| Newsletter signups (from organic) | 200 | 1K | 3K |

Targets are aggressive but achievable given the category is currently SEO-under-claimed.

---

## X. Critical anti-patterns

- **Don't keyword-stuff.** Modern search rewards natural language; stuffing penalizes.
- **Don't duplicate content** across regional sites without `hreflang` tags.
- **Don't ship pages with auto-generated AI content.** Google penalizes detectable AI content at scale.
- **Don't gate the long-form thesis** behind email signup. Make it free and shareable; the SEO + amplification benefit dwarfs the email captures.
- **Don't redirect everything to one super-page.** Distribute SEO equity across the page hierarchy.
- **Don't ignore mobile.** ~70% of crypto search traffic is mobile.
- **Don't ignore the SERP feature opportunities** — featured snippets, People Also Ask, knowledge panels. Optimize content for these explicitly.
