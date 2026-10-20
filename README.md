<div align="center">

# Hosein Hayati
### Backend Engineer | C# · .NET 10 · DDD · CQRS | Agentic / AI-assisted coding

[hoseinhayati.ir@gmail.com](mailto:hoseinhayati.ir@gmail.com) | [hoseinhayati.ir](https://hoseinhayati.ir) | [LinkedIn](https://linkedin.com/in/hosein-hayati) | [github.com/hoseinhayati](https://github.com/hoseinhayati)

English | [فارسی](README.fa.md)

[PDF](https://hoseinhayati.ir/resume_en.pdf) | [Word](https://hoseinhayati.ir/resume_en.docx)

</div>

---

I'm a backend engineer. I have been building with .NET since 2017, and I like owning a system end to end: architecture, data, integrations, deployment and monitoring.

## What I have actually shipped

### A high-volume transaction system · 2023–present

Sole developer, from a half-finished codebase to production. **200+ billion Toman** processed in roughly two years.

- **An append-only transaction log as the single source of truth**: every derived value can be rebuilt from recorded transactions, never from a cached column.
- **Value objects instead of primitives**, so invalid operations fail loudly at the domain boundary.
- **Idempotent handling** of third-party callbacks and client retries: duplicate requests have no side effects.
- **Concurrency control** on hot rows, added after a race condition surfaced in staging.
- **Automated nightly consistency checks**, written after one manual investigation took three days.
- Absorbed **10x growth** in volume through query tuning, Redis caching and background jobs; Serilog + ELK and an ops dashboard.
- Handed the system over to a six-engineer team through a documentation sprint.

### [Pishgamit](https://pishgamit.com) · founder, sole engineer · since 2017

A Persian technical publication I have run alone for nine years. 4,000+ articles, peak 157K monthly visits. Rebuilt from ASP.NET MVC onto .NET 8 with AI-assisted development and now running on .NET 10; day-to-day operations (SEO monitoring, publish scheduling, Telegram and Instagram) run with Claude. Nine years of maintenance taught me more about long-lived systems than any greenfield project ever did.

### Built with agentic coding

I ship apps with Claude Code (plus Cursor), and I keep the parts an agent can't do: choosing the approach, checking dependencies and licences, deployment, debugging and review.

- **[LifeBudget](https://lifebudget.hoseinhayati.ir/intro)**: my own web and Android budgeting app. Logs spending from bank SMS messages, tracks monthly and instalment credit separately, and has no foreign dependencies, so it works on Iran's national internet. ASP.NET Core, SQL Server, Kotlin.
- **[hoseinhayati.ir](https://hoseinhayati.ir/en)**: this resume site. .NET 10, Razor Pages, bilingual RTL/LTR, built with Claude Code.

## How I think about architecture

> Architecture is not a diagram. It is what decides how bad your worst on-call night gets.

I use Clean Architecture, DDD and CQRS because in practice they keep the cost of change low, not because they look good on a slide.

## Stack

`C#` `.NET 10` `ASP.NET Core` `EF Core` `Dapper` `SQL Server` `MongoDB` `Redis` `RabbitMQ` `Docker` `Blazor` `Serilog` `ELK` `Grafana` `Claude Code`

## Repositories

| Repo | What it is |
| --- | --- |
| [Wallet-API](https://github.com/Hoseinhayati/Wallet-API) | Open-source reference implementation: two .NET 8 services, Clean Architecture, CQRS with MediatR, DDD, unit tests. It demonstrates the architecture; it is not a production system. |

## Learning now

Event sourcing: rebuilding a small transactional service on it to learn where it pays off and where it does not. I have shipped state-based systems to production, not event-sourced ones.

---

<div align="center">

[hoseinhayati.ir](https://hoseinhayati.ir) · [LinkedIn](https://linkedin.com/in/hosein-hayati) · Tehran, Iran

</div>
