# Marc-Antoine Paquet

I build data products for endurance sport, and the tooling I use to build them with coding agents.

## Projects

### Synapse — training analytics for endurance coaches
Code private · [synapse-lab.app](https://synapse-lab.app/en)

The aim is to gather each athlete's training, sleep and wellness data from the devices and apps they
already use, centralize it in one platform, and then build prediction models on top of it. Today it
gives a club's coaches one dashboard with training load and trends per athlete.
Delivered per organization: one instance and one database per client, not a shared SaaS.

**How it's built**
- Next.js (App Router) on Vercel; Postgres on Supabase, with access enforced by row-level security
- Python ingestion and analytics service on AWS Lambda, infrastructure in Terraform
- Provider adapters for Garmin, Oura and Intervals.icu behind one ingestion seam
- One shared foundation (schema, analytics engine, design system); per-org apps derive from it

### agent-gates
Gates around coding agents: separate plan, build and review roles, a reviewer verdict file the
workflow requires, and merge and escalation decisions only a human can make.
Plain Python, no dependencies. [Repo](https://github.com/MarcPaquet/agent-gates)

## How I work
I build with Claude Code under the workflow agent-gates describes: written contracts, a separate
reviewer, human approval before merge.

## Contact
[LinkedIn](https://linkedin.com/in/marc-antoine-paquet-93393b187)
