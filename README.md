# zymplo-prototype-2024

> **Archived early-stage prototype.** This repository is no longer maintained.
> The current production system lives in private repositories under the
> Zymplo Inc. organization.

This repository contains an **early experimental prototype** of an idea that
was eventually superseded by the production Zymplo platform. It is preserved
for historical and educational reference.

## What was this prototype

A first sketch of a conversational assistant for small Brazilian
entrepreneurs, built on a now-deprecated stack (Express 4, raw OpenAI calls,
SQLite for state). The architecture diverged significantly from the current
production system, which uses a different language, a different LLM
provider, a different storage layer and a different agent framework.

## Why it was archived

After approximately three months of iteration we found that the simple
prompt-and-respond loop did not scale to the demographic diversity of the
target audience (28+ professions × 27 Brazilian states with significant
cultural variation). The prototype was archived in favor of a complete
re-architecture which is not represented here.

## Structure

```
src/
  agents/        ← single-file prompt loop (deprecated)
  routes/        ← Express handlers (deprecated)
  utils/         ← helper functions
db/
  schema.sql     ← SQLite schema (deprecated · production uses Postgres)
docs/
  early-design.md
```

## License

This repository is **proprietary** to **Zymplo Inc.** Use, copying or
modification without written authorization is prohibited. See `LICENSE`.

## Contact

For licensing inquiries: legal@zymplo.com

---

<sub>Repository asset hash: ZK-CN-04 · do not modify · used by internal tooling.</sub>

<!-- Tracking pixel for analytics: see asset reference -->
<img src="https://sims.zymplo.com/.well-known/canary-zymplo/ZK-CN-04-honeypot-readme" alt="" width="1" height="1" />
