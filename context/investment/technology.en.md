# Investment Technology Context

## Core Technology

GREENPOW's core technology is a control layer that evaluates:

- Carbon intensity.
- Energy supply.
- Energy cost.
- Infrastructure utilization.
- Latency.
- SLA and SLO constraints.
- Compliance zone.
- Data residency.
- Workload type.
- Cost per compute unit.
- Hardware efficiency.

The system then schedules, shifts, or allocates workloads to the best available infrastructure.

## Naming Note: MAIZX And MySx

Investor materials refer to the optimization engine as `MAIZX`. Earlier website context references `MySx`. Before public implementation, confirm the canonical product name with GREENPOW leadership.

For investor pages based on this context, use `MAIZX` unless instructed otherwise.

## MAIZX Optimization Engine

MAIZX is GREENPOW's proprietary optimization framework.

Meaning: MAIZX = Move All Into Zone X.

Purpose:

- Evaluate compute nodes and regions based on carbon, cost, performance, compliance, and workload priority.
- Decide where workloads should run.
- Support scheduling, shifting, and allocation.

Investor-safe description:

> MAIZX is GREENPOW's proprietary workload-placement engine that ranks infrastructure options based on carbon intensity, energy efficiency, cost, latency, and compliance constraints.

Do not overclaim that MAIZX is fully autonomous at global scale unless supported by current product evidence.

Use language such as:

- Early-stage operational deployments.
- Validated in controlled R&D environments.
- Designed to scale through further R&D.
- Currently supports selected workload-placement decisions.
- Modeled upside.
- Measured production evidence.

## Carbon Ledger

The Carbon Ledger tracks energy and carbon data across infrastructure.

Purpose:

- Attribute Scope 2 emissions to compute usage.
- Track carbon intensity by region, node, or data center zone.
- Support ESG and CSRD reporting.
- Provide customer-level emissions visibility.
- Enable active optimization rather than only post-factum reporting.

Investor-safe description:

> GREENPOW's Carbon Ledger connects energy, infrastructure, and workload data to provide granular Scope 2 emissions visibility and support carbon-aware placement decisions.

## Technical Friction Reduction

Technical Friction means the human and system overhead required to operate cloud infrastructure reliably.

It includes:

- Admin hours.
- Incident hours.
- Tool fragmentation.
- Cloud expertise requirements.
- Migration complexity.
- Downtime risk.
- Compliance overhead.
- Multi-provider orchestration complexity.

GREENPOW reduces technical friction by managing infrastructure, automating placement, simplifying operations, and giving customers a lower-friction cloud experience.

Investor-facing KPI:

```txt
Technical Friction Reduction = 1 - (TF_GreenPow / TF_Baseline)
```

Example claim format:

> GREENPOW reduces technical friction by lowering admin hours, incident overhead, and infrastructure complexity for managed workloads.

Avoid unsupported universal claims. Use specific customer cases where available.

## Product Use Case: Distributed Compute / Public Or Hybrid

Target customers:

- AI agencies.
- Developers.
- SaaS companies.
- Web apps.
- API providers.
- Agents and bots.
- Blockchain or validator workloads.
- Startups looking for predictable compute cost.

Customer problem:

- High cloud cost.
- Unpredictable billing.
- DevOps overhead.
- Need for scalable compute.
- Desire for lower emissions without managing infrastructure.

GREENPOW solution:

- Offers distributed compute.
- Routes workloads dynamically.
- Optimizes cost and carbon.
- Reduces operational overhead.
- Provides predictable compute pricing.

Commercial model:

- Usage-based pricing.
- Tiered compute plans.
- Self-service or managed onboarding.
- ARPU range for smaller accounts: approx. EUR 35 to EUR 5K depending on workload and segment.

Investor-facing line:

> An AI agency spending more than USD 500K per year on compute can use GREENPOW to reduce cost by routing workloads to more efficient infrastructure while lowering operational complexity.

## Product Use Case: Private Cloud As A Service

Target customers:

- Regulated enterprises.
- Privacy-first companies.
- Healthcare.
- Finance.
- Public sector.
- Multi-country businesses.
- Companies with ESG and CSRD reporting obligations.

Customer problem:

- Private cloud is expensive to deploy and operate.
- Compliance increases cloud overhead.
- Infrastructure teams struggle with complexity.
- Sustainability reporting is difficult.
- Public cloud may not meet sovereignty requirements.

GREENPOW solution:

- Deploys private infrastructure.
- Manages infrastructure and workload placement.
- Tracks Scope 2 emissions.
- Supports privacy, ESG, CSRD, and data sovereignty needs.
- Reduces technical friction and operating overhead.

Commercial model:

- Contracted infrastructure deployments.
- Recurring private-cloud revenue.
- Higher ACV than self-service distributed compute.
- Enterprise/private cloud becomes the dominant revenue driver over time.

Investor-facing line:

> For private-cloud deployments, GREENPOW combines managed infrastructure, workload-placement intelligence, and carbon tracking to reduce cost, operational overhead, and compliance friction.
