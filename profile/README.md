# Portrait Architecture

A portfolio of independent software repositories demonstrating practical architecture knowledge across multiple stacks, languages, and architectural patterns. This is not a product company — each repository exists to showcase software design, development practices, and delivery quality.

## Mission

Demonstrate real-world backend and frontend architectures through small but functional products. Each repository is self-contained, Docker-first, and follows strict contracts for API design, frontend integration, testing, CI, observability, and documentation.

## Repositories

| Repository | Backend | Frontend | Architecture | Product Domain |
|---|---|---|---|---|
| [`components-vue`](https://github.com/portrait-architecture/components-vue) | — | Vue 3 + TypeScript + Storybook | UI Package (Design System) | Shared component library |
| [`symfony-vertical-slice-talent-api`](https://github.com/portrait-architecture/symfony-vertical-slice-talent-api) | PHP Symfony | React + TypeScript | Vertical Slice | ATS / talent management |
| [`node-event-driven-commerce-api`](https://github.com/portrait-architecture/node-event-driven-commerce-api) | Node.js + TypeScript | React + TypeScript | Event-Driven + Hexagonal | Checkout & order processing |
| [`python-clean-billing-api`](https://github.com/portrait-architecture/python-clean-billing-api) | Python FastAPI | React Native Expo | Clean Architecture | Subscription billing |
| [`symfony-hexagonal-inventory-api`](https://github.com/portrait-architecture/symfony-hexagonal-inventory-api) | PHP Symfony | Angular + TypeScript | Hexagonal | Inventory & reservations |
| `symfony-cqrs-mongodb-analytics-api` _(pending)_ | PHP Symfony + MongoDB | TBD | CQRS + Read Models | Operational reporting |

## Core Principles

- **Independence** — Every repo runs standalone with `make setup && make start`. No shared code via local paths.
- **Docker-first** — All services (API, frontend, database, queue broker) run via Docker Compose with configurable ports.
- **Contract-driven** — Shared standards for API errors, observability, testing, CI, package distribution, and documentation.
- **AI-agent-ready** — Each repo includes `AGENTS.md`, implementation blocks, product briefs, and architecture docs to guide AI-assisted development.
- **Source-available** — Code is publicly readable for portfolio review but not open-source. See individual repo licenses.

## Architecture Patterns Demonstrated

| Pattern | Repository |
|---|---|
| Vertical Slice Architecture | `symfony-vertical-slice-talent-api` |
| Hexagonal Architecture | `symfony-hexagonal-inventory-api`, `node-event-driven-commerce-api` |
| Clean Architecture | `python-clean-billing-api` |
| Event-Driven + Outbox + Idempotent Consumer | `node-event-driven-commerce-api` |
| CQRS + Read Models + MongoDB Projections | `symfony-cqrs-mongodb-analytics-api` |
| UI Package / Design System with Custom Elements | `components-vue` |

## Tech Stack Variety

**Backend**: PHP Symfony, Node.js, Python FastAPI

**Frontend**: React, Vue 3, Angular, React Native Expo

**Databases**: PostgreSQL, MongoDB

**Queue**: RabbitMQ

**Infrastructure**: Docker Compose, Makefile, GitHub Actions


## Governance

The central `docs/` directory contains cross-cutting standards shared by all repositories:

- **Contracts** — API contract, frontend contract, UI package contract, repository contract
- **Standards** — API errors, observability, testing, CI, security readiness, package distribution, code documentation
- **Architecture** — Principles, ADRs, project-level architecture decisions
- **AI Agent Guides** — Agent contract, implementation playbook, prompt library

Each product repository also maintains its own `docs/` with architecture decisions, implementation blocks, development plans, and product documentation.

## License

All repositories use a **Source-Available Portfolio License**. The code is publicly readable and cloneable for technical evaluation, but redistribution and commercial use are restricted. See the `LICENSE` file in each repository for details.

---

*Architecture is the product.*
