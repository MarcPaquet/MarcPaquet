# Marc-Antoine Paquet

**Solutions Developer — Data Platforms**

I build data products for endurance sport, and tools for building and learning with coding agents.

## Projects

### Synapse — training platform for endurance coaches
Code private · [synapse-lab.app](https://synapse-lab.app/en)

A full platform for coaching staff: coaches centralize all their athletes' data in one place, then plan,
track and report from it. I'm currently working with the Fédération québécoise des sports cyclistes (FQSC)
and the Institut national du sport du Québec (INS Québec) to implement it.

- **Data:** each athlete's training, wellness and health data, from the apps and devices they already use
- **Planning:** season, block and week plans, planned versus actual, calendar integration
- **Tracking and reporting:** training load, performance metrics and trends per athlete
- **Aim:** prediction models built on that data

Delivered per organization: one instance and one database per client, not a shared SaaS.

**How it's built**
- Next.js (App Router) on Vercel; Postgres on Supabase, with access enforced by row-level security
- Python ingestion and analytics service on AWS Lambda, infrastructure in Terraform
- Provider adapters behind one ingestion seam
- One shared foundation (schema, analytics engine, design system); per-org apps derive from it

### agent-gates
Gates around coding agents: separate plan, build and review roles, a reviewer verdict file the
workflow requires, and merge and escalation decisions only a human can make.
Plain Python, no dependencies. [Repo](https://github.com/MarcPaquet/agent-gates)

### teach-loop
Claude Code skills that teach in an Obsidian vault: a lesson probes what the learner knows before it
plans, checks its facts against sources before teaching them, and hears the reasoning before giving a
verdict. A level moves only on evidence.
Three skills and one agent, all Markdown. [Repo](https://github.com/MarcPaquet/teach-loop)

## How I work
I build with Claude Code under the workflow agent-gates describes: written contracts, a separate
reviewer, human approval before merge.
