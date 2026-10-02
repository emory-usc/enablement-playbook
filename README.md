# Technical Enablement Kit

> Turn any product plus a customer situation into source-backed,
> customer-ready deliverables — without inventing facts or overpromising.

A reusable, prompt-driven enablement framework for technical sellers and
solution engineers working enterprise accounts. It converts a product and a
customer context into a mastery whitepaper, a tight customer-facing deck, and
the source validation needed to defend every technical claim.

The system is plain Markdown: prompt files you apply in order, intake templates
you fill in, and an `outputs/` tree where deliverables land. No install, no
build step — bring the files into the AI assistant of your choice and go.

## Why this exists

Enterprise customers evaluate products through a stricter lens than most. They
are not only asking "what does the product do?" — they are asking whether it
unlocks business value *while* reducing risk, meeting governance expectations,
satisfying security requirements, and fitting their operating model.

This kit helps you show up with material that is:

- customer-relevant and business-value first
- technically credible and source-backed
- risk, compliance, and governance aware
- concise enough for a customer conversation, deep enough for prep

## Core operating model

Each artifact has one job, and the orchestrator decides which to produce.

| Element | Role |
|---|---|
| Whitepaper | Product mastery — you learn the product deeply |
| Deck | Customer decision narrative — slides that drive a decision |
| Appendix | Technical insurance — depth, diagrams, limits kept out of the live deck |
| Claims register | Source validation — proof behind every technical claim |
| Source pack | Reusable, validated evidence library per product |
| Orchestrator | Workflow router — decides whitepaper, deck, or both |

Two principles run through everything: **the live deck is the customer decision
narrative; the appendix is the technical insurance.**

## Repository structure

```
enablement-playbook/
├─ README.md
├─ START_HERE.md
├─ prompts/
│  ├─ 00_shared_foundation.md
│  ├─ 01_whitepaper_master_prompt.md
│  ├─ 02_deck_master_prompt.md
│  └─ 03_orchestrator_prompt.md
├─ inputs/
│  ├─ customer_context_template.md
│  └─ product_request_template.md
└─ outputs/
   ├─ whitepapers/
   ├─ decks/
   ├─ claims-registers/
   └─ talk-tracks/
```

## Hard rules / guardrails

Non-negotiable. These keep deliverables defensible in a regulated environment.

- **No source, no strong claim.** If a claim can't be traced to a source, it
  can't be stated as fact.
- **No customer relevance, no live slide.** If a slide doesn't help the
  customer decide, move it to the appendix.
- **Do not invent customer details** — ever.
- **Do not overpromise** compliance, security, availability, performance,
  licensing, regional availability, private networking, roadmap, or integration
  support.
- **Mark assumptions clearly** and route unknowns to *Questions to Validate*.
- **Every claim carries a status** — `Confirmed`, `Needs validation`, or
  `Do not present`. Only `Confirmed` claims may be stated strongly.

## Getting started

1. Read `START_HERE.md`.
2. Copy the relevant template from `inputs/` and fill it in.
3. Apply `prompts/00_shared_foundation.md` and `prompts/03_orchestrator_prompt.md`,
   then the whitepaper and/or deck prompt.
4. Find your deliverables under `outputs/` and validate every claim against the
   source packs.
