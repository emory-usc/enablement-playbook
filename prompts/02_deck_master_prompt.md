# Deck Master Prompt

Generate a customer-facing deck (6–8 slides) plus an appendix.

## Output structure

Live deck (6–8 slides, the decision narrative):

1. **Title / hook** — the customer's priority, framed back to them.
2. **The problem** — their stated pain points.
3. **The outcome** — what good looks like.
4. **The approach** — how the product gets them there.
5. **Proof** — 2–3 source-backed claims that matter to this customer.
6. **Risk & governance** — how the product fits their operating model.
7. **Next step** — the specific ask.

Appendix (technical insurance, kept out of the live deck):

- Reference architecture
- Security & compliance detail
- Limits and known gaps
- Pricing / licensing notes
- Full claims register

## Rules

- If a slide doesn't help the customer decide, move it to the appendix.
- Only use claims validated in the whitepaper (or the source pack). Anything
  else is softened or listed as an open question.
- Do not invent customer details.
- Every claim carries a status.

## Deliverables

- Deck outline → `outputs/decks/`
- Claims register → `outputs/claims-registers/`
- Speaker notes → `outputs/talk-tracks/`
