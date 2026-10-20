<div align="center">

# Hosein Hayati
### Senior .NET Backend Engineer | Wallets, Ledgers & Insurance Core Systems

[hoseinhayati.ir@gmail.com](mailto:hoseinhayati.ir@gmail.com) | [hoseinhayati.ir](https://hoseinhayati.ir) | [LinkedIn](https://linkedin.com/in/hosein-hayati) | [github.com/hoseinhayati](https://github.com/hoseinhayati)

English | [فارسی](README.fa.md)

[PDF](https://hoseinhayati.ir/resume_en.pdf) | [Word](https://hoseinhayati.ir/resume_en.docx)

</div>

---

**I work on systems where mistakes are expensive.**

Seven years on wallets, ledgers and insurance platforms — where a rounding error is a real person's real money.

## What I have actually shipped

### Digital wallet · Saman Insurance · 2023–present

Sole developer, from a half-finished codebase to production. **200+ billion Toman** processed in roughly two years.

- **Ledger as the single source of truth** — every balance is reconstructable from recorded transactions, never from a cached column.
- **Money as a value object** (amount + currency + rules), not a bare `decimal`. Cross-currency addition throws; it does not silently miscalculate.
- **Idempotency** across payment callbacks and user retries — duplicate gateway callbacks do not create duplicate money.
- **Concurrency control** on balance mutation, after a race condition duplicated funds in staging.
- **Automated nightly reconciliation**, written the night a 50,000-Rial mismatch cost three days of manual checks.
- Two wallet types (credit / cash), gateway deposits, referral credit, withdrawal, P2P transfer. Serilog + ELK, ops dashboard.

### Insurance systems

Premium-calculation engine for health-insurance issuance as an isolated, testable domain service. Integrations with national insurance APIs, with idempotency and explicit failure paths. Gold Unit-Link: event-driven microservices on .NET 6.

### [Pishgamit](https://pishgamit.com) · founder, sole engineer · since 2017

A Persian technical publication I have kept online for nine years. 4,000+ articles, peak 157K monthly visits, rebuilt from ASP.NET MVC onto .NET 8 with AI-assisted development and now running on .NET 10; day-to-day operations (SEO monitoring, publish scheduling, Telegram and Instagram) run with Claude. Nine years of maintenance taught me more about long-lived systems than any greenfield project ever did.

### Built with agentic coding

I ship production apps with Claude Code (plus Cursor), and I keep the parts an agent can't do: choosing the approach, checking dependencies and licences, deployment and review.

- **[Mahshahr Adventure](https://hoseinhayati.ir/en/portfolio/mahshahr-adventure)**: website for a bicycle shop with an online store, trip and camping sign-ups, and repair requests with tracking. Built 100% with vibe coding in about four months. .NET 10, EF Core, SQL Server.
- **[LifeBudget](https://lifebudget.hoseinhayati.ir/intro)**: my own web and Android budgeting app. Logs spending from bank SMS messages, tracks monthly and instalment credit separately, and works on Iran's national internet. ASP.NET Core, SQL Server, Kotlin.
- **[hoseinhayati.ir](https://hoseinhayati.ir/en)**: this resume site. .NET 10, Razor Pages, bilingual RTL/LTR, built with Claude Code.

## How I think about architecture

> Architecture is not a diagram. It is what decides how bad your worst on-call night gets.

I use Clean Architecture, DDD and CQRS because in practice they keep the cost of change low — not because they look good on a slide. In financial systems, "almost correct" means wrong.

## Stack

`C#` `.NET 10` `ASP.NET Core` `EF Core` `Dapper` `SQL Server` `MongoDB` `Redis` `RabbitMQ` `Docker` `Blazor` `Serilog` `ELK` `Grafana` `Claude Code`

## Repositories

| Repo | What it is |
| --- | --- |
| [Wallet-API](https://github.com/Hoseinhayati/Wallet-API) | Open-source digital wallet — .NET 8, two services (Wallet, Transaction), Clean Architecture, CQRS with MediatR, DDD, unit tests. A reference implementation of the architecture, not the production system. |

## Currently building

**`wallet-event-sourced`** — a second wallet, deliberately rebuilt on event sourcing to learn where it pays off and where it does not. Event store, projections and messaging as first-class infrastructure concerns.

Learning in the open: I have shipped state-based ledgers to production, not event-sourced ones. The README will say plainly which decisions are production-tested and which are experiments.

---

<div align="center">

[hoseinhayati.ir](https://hoseinhayati.ir) · [LinkedIn](https://linkedin.com/in/hosein-hayati) · Tehran, Iran

</div>

