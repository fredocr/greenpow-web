# Decision: Investment Context

Date: 2026-05-20

## Decision

GREENPOW will maintain dedicated investor-facing source material under:

```txt
context/investment/
```

## Rationale

The investment web experience has a different audience, proof standard, CTA structure, and claim risk than the general marketing website. Investor pages need to lead with cost, infrastructure efficiency, traction, unit economics, market timing, defensibility, and fundraising context, while treating climate impact as a measured advantage rather than a broad sustainability claim.

## Files

```txt
context/investment/investment-context.en.md
context/investment/technology.en.md
context/investment/metrics-and-claims.en.md
context/investment/business-model.en.md
context/investment/market-competition-moat.en.md
context/investment/fundraising.en.md
context/investment/team.en.md
context/investment/investor-faq.en.md
```

## Rules

- Use `context/investment/` for investor-facing websites, landing pages, data room pages, metric cards, and investor FAQs.
- Use `agent/investor-content-rules.md` when generating investor copy.
- Label every metric as achieved, observed, measured, modeled, projected, target, benchmark, R&D validated, or investor estimate.
- Do not present projected, modeled, or target metrics as achieved facts.
- Lead with cost, control, complexity, infrastructure efficiency, and enterprise readiness.
- Treat carbon performance as a measurable advantage, not the only investment reason.

## Naming Note

Investor materials use `MAIZX` for the optimization engine. Earlier website context references `MySx`. Future implementation should confirm the canonical public product name before publishing pages that mention either term.
