# Internal Comms Package

**For the Astarter team itself — not for external publication.** A launch fails internally before it fails externally. Everyone on the team should be able to (a) explain the new positioning in 30 seconds, (b) answer a friend or family member's questions, (c) handle a casual inbound from a journalist or investor without going off-message.

---

## I. All-Hands Memo (CEO → team, T-7 days before launch)

**Subject:** *Where we're going next — Astarter as the settlement layer for the AI Agent economy*

---

Team,

Next Wednesday we're going to announce the most consequential strategic update Astarter has made since the EMURGO joint venture in 2021. I want everyone aligned on the *why* before the *what* lands in public.

**The short version:**

We've spent four years building a four-product DeFi stack on Cardano. That stack — Launchpad, DEX, Money Market, Tech Service Platform — is the foundation of everything that comes next.

What we're announcing is not a pivot. It's a recognition: the financial primitives we built for human DeFi users are exactly what the next generation of autonomous AI agents will need to operate as economic actors. The market we built for is a subset of the market we're now addressing.

**Why now:**

The AI agent economy has crossed from theory into deployment. Olas-powered agents are real on Polymarket. Virtuals has crossed $2B in agent-linked volume. Fetch.ai's ASI:One has 150K+ deployed agents. The category exists, and almost no one is building at the settlement layer underneath it. That's the slot we're taking.

**What's launching:**

1. A long-form thesis piece in Cointime laying out the DeFAI category and our position in it
2. Our strategic alliance with UXLINK — the first credible public attempt to pair an execution layer with a distribution layer in this category
3. A coordinated multi-outlet, multi-language release across the next 7 days

**What I need from each of you:**

- **Everyone:** read the team FAQ attached and the talking points doc. Be ready to answer a friend asking "what does Astarter do now?"
- **Engineering:** the developer marketing pack drops at T-0; the Quickstart and architecture diagram are public the same hour
- **BD / partnerships:** outreach to the warm list begins T+1; we'll work from the ecosystem partner list together
- **Community:** Discord + Telegram cross-posts ready at T-0; you'll receive the pre-staged copy 24h before
- **Support:** standard responses to common questions, escalation path to comms for anything off-script
- **Operations:** legal sign-off on the press kit completes by Friday; please push if there's any slip

**What's *not* in this update:**

- TGE date
- Specific listing venues
- Multi-chain target chains by name

If anyone outside the team asks about these, the answer is *"We'll announce alongside the formal tokenomics publication."* No speculation, no even-friendly-hints. We've all watched projects die because someone on the team got chatty in a private DM.

**The next 90 days will matter more than the previous 12 months.** Every week we either ship something concrete or we don't. The world is watching for the proof points more than for the announcement itself.

I'm proud of what this team has built to get us to this position. Now we execute.

— [CEO]

---

## II. Team FAQ (everyone reads this before launch day)

### Q1. What's the simplest one-line explanation?
> *"Astarter is building the settlement layer for the AI Agent economy. We're the financial primitives autonomous agents need to operate as economic actors."*

### Q2. What if someone asks "isn't this just a pivot?"
> *"No. The four products we've built since 2021 are the foundation we're building on. We're not throwing them out — we're recognizing they apply to a much larger market than DeFi alone."*

### Q3. What if someone asks about TGE date or listing?
> *"Both will be announced alongside the formal tokenomics publication. I don't have a date to share."* Then change the subject. **Never speculate.**

### Q4. What if someone asks "what's DeFAI?"
> *"It's DeFi designed from the ground up for autonomous AI agents instead of human users. Different counterparties, different needs."*

### Q5. What if someone asks "why Cardano and not Ethereum or Solana?"
> *"We started on Cardano with EMURGO backing in 2021 and that's where our production stack runs. Multi-chain expansion is on the near-term roadmap — agents and DePIN are inherently cross-chain."*

### Q6. What if a journalist DMs me directly?
> *"Thanks for reaching out — I'll route you to our comms lead Zakky who can get you the right context."* Then immediately ping Zakky. **Do not freelance interviews.**

### Q7. What if an investor or VC asks me about cap table / valuation?
> *"That's a conversation for our CEO directly — let me make the introduction."* Then ping CEO. **Never discuss financials.**

### Q8. What if a community member is FUD-ing the announcement?
> Don't engage publicly. Forward to community lead. We have pre-written rebuttals in the crisis playbook.

### Q9. What if I see a typo or factual error in the published article?
> Ping Zakky immediately in the launch war room channel. Don't post about it publicly.

### Q10. What if someone asks why the TVL is small?
> *"We're explicitly building rails ahead of the traffic. The metrics that matter for the next two quarters are different from TVL."* See full version in `16-media-faq.md` Q15.

### Q11. Can I share the announcement on my personal Twitter?
> Yes, after T-0. Use the pre-approved copy from `21-linkedin-exec-posts.md` or the X thread, or write your own using the voice guide in `28-brand-guidelines.md`. **Never share before the embargo lifts.**

### Q12. Can I screenshot internal Slack / TG conversations about this?
> No.

### Q13. What if I get asked about UXLINK's roadmap?
> *"I'd defer to UXLINK on their own roadmap. From the Astarter side, our role in the alliance is [execution layer + financial primitives]."*

### Q14. What's the elevator pitch length?
> 15 seconds: *"Settlement layer for autonomous AI agents, built on a 4-year Cardano DeFi stack."*
> 30 seconds: *"Astarter is a Cardano-native infrastructure platform. We've been running a four-product DeFi stack since 2021 — Launchpad, DEX, Money Market, Tech Service Platform. Last week we announced we're repositioning the stack as the settlement layer for the autonomous AI agent economy, in alliance with UXLINK. The thesis: agents don't need better models, they need better financial rails."*

### Q15. What if I'm at a conference and someone wants to "chat with the founder"?
> Take the contact, promise an intro, ping CEO. Don't be the founder.

---

## III. Role-specific talking points

### For engineering team

When asked technical questions:
- Architecture diagram is in `architecture-diagram.png` — share that
- "How does agent settlement actually work technically?" → *"The Money Market is being extended with agent-collateralization primitives. Full technical RFC is on docs site as of [launch date]."*
- "Cardano vs Solana for this?" → *"Different tradeoffs. Cardano's eUTXO model has advantages for deterministic settlement; we're also planning EVM/Solana deployment for cross-chain agent reach."*
- "When can I build on this?" → *"Quickstart at [docs URL] live as of today. Discord developer channel open."*

### For BD / partnerships team

When in inbound partner conversations:
- Use the partner amplification list in `27-stakeholder-map.md` § V
- "Can you do a joint announcement with us?" → *"Likely yes. Let's scope timing and co-marketing assets. Co-marketing kit at [link]."*
- "Can you integrate our product?" → *"Technical integration paths through the Tech Service Platform. Let's get our engineering teams on a call."*

### For community team

- Pinned message ready in Discord + TG (use `20-discord-announcement.md`)
- Common community Qs answered with on-brand language from `16-media-faq.md`
- FUD escalation to comms within 30 minutes of detection
- Welcome new members with link to the long-form feature once published

### For support team

If a user asks about money market positions, ISPO status, or AA holdings:
- Existing product positions are unaffected by the announcement
- ISPO participants: see specific holder comms (`31-community-holder-comms.md`)
- AA token utility expanding, not changing — no action required from existing holders
- Escalate to ops if a user reports a specific account / transaction issue

### For executive team

- All press-facing comms route through Zakky (comms lead)
- Investor inquiries route through CEO
- Conference / podcast bookings route through Zakky + CEO scheduling
- Personal LinkedIn posts using `21-linkedin-exec-posts.md` variants only

---

## IV. All-Hands Slide Deck Outline (15-minute presentation, T-3 days)

| # | Slide | Owner |
|---|---|---|
| 1 | Cover — "What we're announcing on [date]" | CEO |
| 2 | The thesis in one sentence | CEO |
| 3 | Why now — the agent economy timeline | CEO |
| 4 | What we're announcing — the UXLINK alliance | CEO |
| 5 | What the press will say (key articles, headlines) | Comms |
| 6 | What you need to know (team FAQ summary) | Comms |
| 7 | What you need to do — role by role | Department heads |
| 8 | The next 90 days (comms roadmap summary) | Comms |
| 9 | What we're NOT saying yet | CEO |
| 10 | Open floor / Q&A | All |

**Length:** 15 min presentation + 30 min Q&A. Record for anyone unable to attend.

---

## V. Pre-launch checklist (T-7 days)

- [ ] All-hands meeting scheduled
- [ ] Team FAQ distributed
- [ ] Role-specific talking points sent to each team lead
- [ ] Legal review of public-facing copy complete
- [ ] Embargo partner confirmed
- [ ] Drop-day war room channel created
- [ ] War room attendees confirmed
- [ ] Community team has pre-staged copy
- [ ] Engineering team has reviewed architecture diagram
- [ ] CEO has cleared 4 hours of calendar for launch day
- [ ] Backup spokespeople identified if CEO unavailable

---

## VI. Post-launch debrief (T+7 days)

Internal-only debrief covering:

- What landed (Tier 1 / 2 outlets, KOL pickup, sentiment)
- What missed (what we expected vs. what happened)
- Process learnings (what worked in the war room, what didn't)
- Net-new asset gaps surfaced by the launch
- Phase 2 priorities

Format: 30-minute meeting + written summary distributed within 48 hours.

**Critical:** the debrief is honest. If we underperformed, we say so. Internal credibility is built by honest reflection, not victory-lap framing.
