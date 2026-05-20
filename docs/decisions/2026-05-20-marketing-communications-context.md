# Decision: Marketing And Communications Context

Date: 2026-05-20

## Decision

GREENPOW will maintain structured marketing and communications context across dedicated `context/` buckets instead of storing it as one large document.

## Added Context Areas

```txt
context/marketing/
context/audiences/
context/regions/
context/claims/
context/seo/
context/campaigns/
context/website/
context/design/
context/components/
```

## Rationale

Developers, designers, copywriters, Replit agents, and other AI agents need precise context for different kinds of work. Splitting the marketing context by responsibility reduces the risk that agents use the wrong material for product pages, regional pages, claims, campaigns, SEO, or component copy.

## Rules

- Use `context/marketing/` for the top-level marketing and communications frame.
- Use `context/audiences/` before writing persona or tier-specific content.
- Use `context/regions/` before writing Europe, LATAM, Spanish, or Portuguese market content.
- Use `context/claims/` before publishing environmental, ESG, compliance, or sustainability claims.
- Use `context/seo/` before creating editorial or search-focused content.
- Use `context/campaigns/` before creating campaign pages or campaign copy.
- Use `context/website/` before changing homepage messaging or website information architecture.
- Use `context/design/` before implementing visual style or design tokens.
- Use `context/components/` before writing reusable component copy.

## Consequences

Future agents should update the relevant context file first, then implement page or component changes from that source.
