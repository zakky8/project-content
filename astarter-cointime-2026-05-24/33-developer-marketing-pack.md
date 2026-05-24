# Developer Marketing Pack

**For:** Engineering team to publish on docs site + GitHub on launch day
**Purpose:** Convert the press launch into developer signups by giving builders something concrete to engage with at T-0

The single most important rule of developer marketing: **don't make them ask.** Quickstart, architecture, code samples, Discord channel — all ready, all linked, all working.

---

## I. Public docs site structure (recommended IA)

```
docs.astarter.io/
├── /                          # Landing — thesis + Quickstart link
├── /quickstart                # 5-min "deploy your first agent" walkthrough
├── /architecture              # The four-product stack + DeFAI overlay
├── /agents
│   ├── /concepts              # What is an agent, in our model
│   ├── /settlement            # How agent-to-agent settlement works
│   ├── /collateral            # Money Market for agent credit
│   └── /examples              # Sample agent implementations
├── /protocol
│   ├── /launchpad             # Launchpad / Launchpool reference
│   ├── /dex                   # DEX reference
│   ├── /money-market          # Money Market reference
│   └── /tech-service          # Tech Service Platform reference
├── /token                     # AA token model + utility
├── /multichain                # Multi-chain roadmap + integration paths
├── /rfcs                      # Request for Comment / RFC index
├── /security                  # Audit reports + bug bounty
├── /community                 # Discord, GitHub, contributors
└── /changelog                 # Release notes
```

---

## II. Quickstart (5-minute walkthrough)

```markdown
# Quickstart — Deploy Your First Agent on Astarter

## What you'll build
A minimal autonomous agent that:
- Holds AA as operating capital
- Settles a transaction with another agent
- Posts collateral to the Money Market
- Returns proceeds to its operator

Total time: ~5 minutes. Total cost: testnet only.

## Prerequisites
- A Cardano wallet (Nami / Eternl / Lace)
- 100 testnet AA (faucet link)
- Node.js 18+ and the Astarter SDK

## 1. Install the SDK

    npm install @astarter/agent-sdk

## 2. Initialize an agent

    import { Agent } from '@astarter/agent-sdk';

    const agent = new Agent({
      network: 'preview',          // testnet
      walletProvider: 'nami',
      operatingCapital: 100,        // AA
    });

## 3. Settle a transaction with another agent

    const result = await agent.settle({
      counterparty: 'addr_test...',
      amount: 5,
      asset: 'AA',
    });

    console.log(result.txHash);

## 4. Post collateral to the Money Market

    const position = await agent.collateralize({
      amount: 50,
      asset: 'AA',
      borrowAsset: 'iUSD',
      borrowAmount: 25,
    });

## 5. Return proceeds

    await agent.returnToOperator({
      amount: position.borrowed,
      asset: 'iUSD',
    });

## What's next
- Read the [Architecture Overview](/architecture)
- Try the [Sample Agent Implementations](/agents/examples)
- Join the developer Discord at [link]
- Propose an integration via [RFC template](/rfcs)
```

**Note:** SDK does not yet exist as written above. This is the *target* developer experience for the docs site by launch day. Engineering team to confirm shipping scope.

---

## III. Architecture diagram (visual + textual)

### Textual reference

```
┌─────────────────────────────────────────────────────────────────┐
│                    AI AGENT (the actor)                         │
│              autonomous reasoning + decision                     │
└──────────────────────┬──────────────────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────────────────────┐
│                  DEFAI EXECUTION LAYER                          │
│                  (financial primitives)                          │
│                                                                  │
│  ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐  │
│  │ LAUNCHPAD  │ │    DEX     │ │ MONEY MKT  │ │ TECH SVC   │  │
│  │  agent-    │ │ agent-to-  │ │  agent-    │ │  builder   │  │
│  │   native   │ │   agent    │ │   credit   │ │  tooling   │  │
│  │  issuance  │ │ settlement │ │ primitives │ │            │  │
│  └────────────┘ └────────────┘ └────────────┘ └────────────┘  │
│                                                                  │
│                  Anchored by AA token                            │
│       (unit of account · payment · governance · collateral)      │
└──────────────────────┬──────────────────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────────────────────┐
│                       DEPIN SUBSTRATE                           │
│         decentralized compute · physical infra · oracles         │
└─────────────────────────────────────────────────────────────────┘

         Anchored on Cardano · Multi-chain expansion in progress
```

### Visual version

To be generated as: `astarter-architecture-1200x900.png` (Quiet Substrate aesthetic, isometric three-layer stack with cyan signal on the Astarter execution layer).

---

## IV. GitHub README template

```markdown
# Astarter — Settlement Infrastructure for the AI Agent Economy

> Cardano-native DeFi infrastructure for autonomous AI agents.
> AI Agent + DePIN + DeFAI under a single coordinated stack.

[![Docs](https://img.shields.io/badge/docs-astarter.io-blue)](https://docs.astarter.io)
[![Discord](https://img.shields.io/discord/...)](https://discord.gg/astarter)
[![Twitter](https://img.shields.io/twitter/follow/AstarterDefiHub)](https://twitter.com/AstarterDefiHub)

## What is Astarter?

Astarter is the settlement layer for the autonomous AI Agent economy. We provide the financial primitives — issuance, liquidity, credit, governance — that autonomous AI agents need to operate as economic actors on-chain.

## Why?

DeFi was built for human counterparties. Agents can't improvise when settlement breaks. They need deterministic settlement, predictable fees, and primitives that compose without permission. That's what we're building.

## Stack

- **Launchpad** — agent-native issuance and incentive coordination
- **DEX** — on-chain liquidity and price discovery
- **Money Market** — collateralized lending including agent-issued credit
- **Tech Service Platform** — builder tooling for agent deployment

## Quickstart

5 minutes to deploy your first agent: [docs.astarter.io/quickstart](https://docs.astarter.io/quickstart)

## Documentation

Full docs: [docs.astarter.io](https://docs.astarter.io)

## Contributing

We accept contributions via the RFC process:
1. Read the [contributor guide](CONTRIBUTING.md)
2. Open an RFC in this repo
3. Discuss in the developer Discord channel
4. Submit PR following the RFC outcome

## Security

- Audit reports: [docs.astarter.io/security](https://docs.astarter.io/security)
- Bug bounty: [link]
- Disclosure: security@astarter.io

## Community

- Discord: [discord.gg/astarter](https://discord.gg/astarter)
- Telegram: [t.me/astarter](https://t.me/astarter)
- Twitter: [@AstarterDefiHub](https://twitter.com/AstarterDefiHub)
- Newsletter: [astarter.io/subscribe](https://astarter.io/subscribe)

## License

[License — to be confirmed by legal]

## Acknowledgments

Astarter was founded as a joint venture with EMURGO in 2021.
```

---

## V. Contributor / RFC template

```markdown
# RFC-XXXX: [Title]

**Status:** Draft / Discussion / Accepted / Rejected
**Author:** [@github-handle]
**Created:** YYYY-MM-DD
**Tracking issue:** #...

## Summary
One-paragraph description of what this RFC proposes.

## Motivation
Why are we doing this? What problem does it solve?
Which Astarter product or layer does it affect?

## Detailed design
The bulk of the RFC. Explain the design clearly enough that:
- Someone familiar with Astarter could implement it
- The trade-offs are explicit
- The interfaces / APIs are concrete

## Rationale and alternatives
- Why is this design the best choice?
- What other designs were considered?
- What is the cost of doing nothing?

## Drawbacks
What could go wrong? What could break?

## Unresolved questions
What's still open for discussion?
```

---

## VI. Developer Discord channel charter

**Channel:** `#developers`
**Purpose:** Technical questions, RFC discussion, integration support, bug reports

**Rules pinned at top:**

```
WELCOME TO ASTARTER DEVELOPERS

This channel is for technical conversation. Please:

✅ Ask code-specific questions with code snippets
✅ Reference docs links when relevant
✅ Use threads for multi-message discussions
✅ Tag @dev-team for issues that need engineering response
✅ Open a GitHub issue for bugs you've reproduced

❌ Don't ask token price / TGE questions here (use #general)
❌ Don't post sponsored content or unrelated projects
❌ Don't share private keys, seeds, or sensitive info — ever

Office hours: every Wednesday 16:00 UTC in #dev-stage
Bug bounty: see security@astarter.io
```

---

## VII. Code samples library (target structure)

```
github.com/astarter/examples/
├── /minimal-agent              # Quickstart code
├── /agent-collateral           # Money Market collateral example
├── /agent-to-agent-payment     # Settlement walkthrough
├── /multi-agent-coordination   # 3+ agents collaborating
├── /agent-credit-issuance      # Borrowing as an agent
├── /cross-chain-agent          # Multi-chain integration sample
└── /production-deployment      # Production-ready template
```

Each sample includes: README, runnable code, test data, expected output, troubleshooting section.

---

## VIII. Developer launch sequencing

### T-0 (press launch day)
- [ ] Docs site live with Quickstart + Architecture
- [ ] GitHub README updated to new positioning
- [ ] Developer Discord channel charter pinned
- [ ] Architecture diagram PNG live on docs landing
- [ ] At least 2 code samples in the examples repo
- [ ] Blog post: "Building on Astarter — Developer Overview"

### T+7
- [ ] Office hours session (recorded, posted)
- [ ] First RFC published (could be from team or external)
- [ ] Developer-specific newsletter blast

### T+14
- [ ] Bug bounty announced (or refreshed)
- [ ] First external integration spotlight (if available)

### T+30
- [ ] Developer survey: what's missing in the docs?
- [ ] Quickstart improvements based on actual usage data
- [ ] First contributor recognition post

---

## IX. Developer marketing metrics to track

| Metric | T+7 target | T+30 target |
|---|---|---|
| Docs site unique visitors | 1,000 | 5,000 |
| Quickstart completions | 50 | 250 |
| GitHub stars on main repo | 100 | 500 |
| Discord developer channel members | 100 | 400 |
| Code sample clones | 20 | 100 |
| RFC submissions (external) | 0 | 2 |
| Inbound integration requests | 2 | 10 |

If we miss these floors, the issue is usually one of three things: (a) Quickstart isn't actually 5 minutes, (b) docs are too abstract, (c) there's no real working SDK behind the docs.

---

## X. Anti-patterns for developer marketing

- Marketing copy on technical pages — devs leave immediately
- "Documentation coming soon" placeholders
- Code samples that don't actually run
- Discord channels with no engineering presence
- Bug reports that go unanswered for >72 hours
- Architecture diagrams that show marketing layers, not actual system layers
- Token / price mentions on technical pages
- Required signup to view docs
