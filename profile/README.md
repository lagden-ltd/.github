<picture>
  <source media="(prefers-color-scheme: dark)" srcset="logo-reversed.svg">
  <img src="logo.svg" alt="Lagden Ltd" height="48">
</picture>

Lagden Ltd is a UK software company. We build custom business software and the websites in front of it: CRMs, client portals, booking and quote systems, and internal tools that replace the spreadsheets a business has outgrown.

### How we build

- Every project gets its own repository, started from a shared template with the same structure, checks and standards.
- Every change starts as an issue with acceptance criteria, gets a separate review against them, and is checked in a real browser before release.
- Conventional commits, semantic versioning, a changelog and an annotated tag for every release.
- Each project keeps a written record of how it meets our minimum standards for security, accessibility, testing and monitoring.
- Business logic lives in plain modules, not route handlers or components, so it can be tested without a request or a render.

### What we build with

| | |
|---|---|
| Languages | TypeScript, Python, Go, Rust |
| Web | Next.js (App Router), React, Tailwind CSS, shadcn/ui |
| APIs | REST with OpenAPI docs, FastAPI, Go |
| Data | PostgreSQL with plain SQL migrations, SQLite, Redis, Cloudflare D1 with Drizzle |
| Auth and payments | Better Auth, Stripe |
| Email | Resend, self-hosted Mailcow |

### How we run it

- Apps ship as Docker images to self-hosted Coolify. Static sites and edge apps run on Cloudflare Pages and Workers.
- Origin servers accept traffic only through Cloudflare, using Origin CA certificates and Cloudflare IP allowlists.
- Self-hosted GlitchTip tracks errors, uptime and scheduled-job heartbeats, with alerts by email and push.
- Encrypted, deduplicated backups go off-site every night, and restores are tested on a schedule.
- Secrets stay out of repositories, and every token is scoped to the least it needs.

### Repositories

Client and company repositories here are private. Our founder, [Zach Lagden](https://github.com/zachlagden), publishes open-source tools on his own profile.

### Contact

[lagden.uk](https://lagden.uk) · [hello@lagden.uk](mailto:hello@lagden.uk)

<sub>Lagden Ltd is registered in England and Wales, company number 17460707.</sub>
