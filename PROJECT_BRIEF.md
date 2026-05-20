# GREENPOW Website Project Brief

## Objective

Replace the existing WordPress site with a structured bilingual website for GREENPOW.

GREENPOW must be positioned as a carbon-aware cloud infrastructure company reducing the carbon footprint of cloud computing by optimizing where and when compute runs across public cloud, private cloud, VPS, hosting, and distributed infrastructure.

The website must support sales, partner development, investor conversations, and education around carbon-aware workload orchestration.

## Core Positioning

GREENPOW reduces cloud emissions by routing workloads using real-time carbon, energy, cost, and infrastructure signals.

The company should be presented as product-led infrastructure technology. It must not be reduced to managed hosting or generic IT services.

Core strategic themes:

- Carbon-aware workload scheduling.
- Multi-cloud and distributed infrastructure optimization.
- Public cloud, private cloud, VPS, hosting, and distributed compute selection.
- Scope 2 visibility and reduction.
- ESG and CSRD relevance.
- AI infrastructure for autonomous organizations.
- Sovereign and hybrid cloud options.
- Cost, performance, energy, and carbon optimization.

## Required Stack

Recommended implementation:

- Next.js
- TypeScript
- Tailwind CSS
- MDX or structured content files
- i18n routing
- Reusable templates
- Central Pipedrive form integration

The implementation should avoid hardcoded strategy content inside React components. Use the files in `context/` as the source of truth.

## Repository Structure Model

Use the repository as a layered knowledge system:

```txt
PROJECT_BRIEF.md        Approved project objective and website requirements.
AGENTS.md              Non-negotiable agent instructions.
context/               Approved website source material.
agent/                 Coding-agent workflow and build instructions.
rnd/                   Research and development bucket.
docs/decisions/        Accepted decisions.
docs/implementation/   Build handoffs and technical notes.
docs/superpowers/      Superpowers specs and implementation plans.
```

`rnd/` is intentionally separate from `context/`. It can inform future work, but it is not approved production truth until promoted into `context/`, this brief, or `docs/decisions/`.

## Language And Routing

Every page must exist in English and Spanish:

```txt
/en/...
/es/...
```

Language parity is mandatory. Every new English route must have a Spanish counterpart with the same layout, component structure, metadata, CTA structure, and form behavior.

## Main Navigation

```txt
Home
Technology
Products
Use Cases
Impact
Partners
Funding / Investors
About
Contact
```

## Core Routes

Recommended initial route map:

```txt
/en
/es
/en/technology
/es/technology
/en/products
/es/products
/en/products/public-cloud-optimization
/es/products/optimizacion-cloud-publica
/en/products/vps-web-hosting
/es/products/vps-hosting-web
/en/products/private-cloud
/es/products/cloud-privada
/en/products/ai-agents-infrastructure
/es/products/infraestructura-agentes-ia
/en/products/cortex
/es/products/cortex
/en/use-cases
/es/casos-de-uso
/en/use-cases/esg-csrd
/es/casos-de-uso/esg-csrd
/en/use-cases/ai
/es/casos-de-uso/ia
/en/use-cases/ecommerce
/es/casos-de-uso/ecommerce
/en/use-cases/sovereign-cloud
/es/casos-de-uso/cloud-soberana
/en/use-cases/legal
/es/casos-de-uso/legal
/en/impact
/es/impacto
/en/partners
/es/partners
/en/funding
/es/inversores
/en/about
/es/sobre-greenpow
/en/contact
/es/contacto
/en/privacy
/es/privacidad
/en/cookies
/es/cookies
/en/terms
/es/terminos
```

## Homepage

Hero:

```txt
Cleaner compute for the AI and cloud era.
```

Subhero:

```txt
GREENPOW reduces cloud emissions by routing workloads using real-time carbon, energy, cost, and infrastructure signals.
```

Homepage sections:

1. The problem: cloud decisions are static, but energy, cost, carbon, and performance are dynamic.
2. The solution: carbon-aware compute orchestration.
3. Products.
4. Use cases by industry.
5. Impact model: Scope 2, auto-offsetting, load shifting, and LCA.
6. Partners and accelerators.
7. CTA: Talk to us, become a partner, or contact investors.

## Product Structure

GREENPOW products should be organized as:

1. Public Cloud Optimization
   Carbon-aware workload routing, cloud cost optimization, and Scope 2 visibility.

2. VPS & Web Hosting
   Sustainable hosting, managed hosting, and business infrastructure migration from legacy hosting.

3. Private Cloud
   Sovereign, hybrid, enterprise-grade infrastructure.

4. AI Agents Infrastructure
   Cloud layer for autonomous organizations and AI-enabled workflows.

5. Cortex
   Static organizational memory layer for autonomous agents: context, institutional knowledge, process memory, and decision-support structure.

## Landing Page Verticals

Create repeatable industry landing pages for:

```txt
/en/use-cases/esg-csrd
/en/use-cases/ai
/en/use-cases/ecommerce
/en/use-cases/sovereign-cloud
/en/use-cases/legal
```

Each page must follow the same structure:

```txt
Hero
Problem
Why now
GREENPOW solution
Relevant product modules
Impact / carbon reduction angle
Compliance or business benefit
Use-case example
CTA
FAQ
```

## Forms

Required public forms:

```txt
Partner form
Investor form
Support form
General contact form
Demo / sales form
```

All forms must connect to Pipedrive through one central form handler. Do not create separate integration logic per form.

Recommended form fields:

```txt
name
email
company
role
country
interest_type
message
preferred_language
source_page
utm_source
utm_medium
utm_campaign
```

## Context File Map

```txt
/context
  /brand
    brandbook.en.md
    brandbook.es.md
  /sales
    ads-sales.en.md
    ads-sales.es.md
  /funding
    funding-angle.en.md
    funding-angle.es.md
  /impact
    impact-lca-mysx.en.md
    impact-lca-mysx.es.md
  /partners
    partners-affiliates.en.md
    partners-affiliates.es.md
  /legal
    cookies.en.md
    cookies.es.md
    privacy.en.md
    privacy.es.md
    terms.en.md
    terms.es.md
  /forms
    pipedrive-fields.md
  /products
    products.en.md
    products.es.md
  /verticals
    esg-csrd.en.md
    esg-csrd.es.md
    ai.en.md
    ai.es.md
    ecommerce.en.md
    ecommerce.es.md
    sovereign-cloud.en.md
    sovereign-cloud.es.md
    legal.en.md
    legal.es.md
```

## Agent Build Instructions

The coding agent must:

- Build a bilingual website in English and Spanish.
- Use structured context files as the source of truth.
- Use `agent/` files for workflow and build-sequence guidance.
- Treat `rnd/` as exploratory material, not approved public copy.
- Never create an English page without a Spanish counterpart.
- Keep design consistent across all sections.
- Use reusable page templates for products and verticals.
- Connect all forms to Pipedrive.
- Preserve legal pages: privacy, cookies, and terms.
- Present GREENPOW as product-led infrastructure technology, not only hosting or services.
- Make the mission clear: reduce the carbon footprint of cloud computing.
- Explain MySx as the algorithmic layer for moving compute based on carbon intensity, energy price, and infrastructure availability.
- Make Cortex understandable as organizational memory for autonomous agents.

## Definition Of Done

An initial build is complete when:

- English and Spanish route trees exist.
- Product and vertical pages use reusable templates.
- Homepage uses the positioning in this brief.
- Forms submit through one central Pipedrive handler.
- Legal routes exist in both languages.
- Context files remain the source of truth for strategic content.
- The site can be deployed from Replit or another Node-compatible host.
