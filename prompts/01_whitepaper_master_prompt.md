# Whitepaper Master Prompt

Generate a product-mastery whitepaper for a solution engineer.

## Output structure

1. **Executive summary** — 3–4 sentences on what the product is and why it
   matters to the customer's business.
2. **What the product does** — capabilities, framed as outcomes, not features.
3. **How it works** — architecture at a level an architect can reason about.
4. **When to use it / when not to** — honest fit and limits.
5. **Risk, compliance, and governance** — security model, data handling,
   regulatory considerations.
6. **Competitive / decision context** — where it wins, where it doesn't.
7. **Technical Claims Register** — every strong claim with its source and a
   status (`Confirmed` / `Needs validation` / `Do not present`).
8. **Questions to Validate** — open items, marked as assumptions.

## Rules

- Every `Confirmed` claim must cite a source.
- Soften or list `Needs validation` claims as open questions.
- Never include a `Do not present` claim in customer-facing content.
- Do not invent facts. If a capability is unknown, say so.

## Deliverables

- Whitepaper → `outputs/whitepapers/`
- Claims register → `outputs/claims-registers/`
- One-page cheat sheet → `outputs/talk-tracks/`
