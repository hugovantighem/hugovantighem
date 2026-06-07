# Hugo Vantighem

**Principal engineer — building developer infrastructure and agentic systems.**

---

## Atome — Pure Flow Engine

A crash-safe, single-writer flow engine for event-driven applications. Group-commit fsync at **~22 000 items/s** local, **~33 000 items/s** on cloud Linux NVMe. Your business logic lives in a Sidecar you own; Atome guarantees ordering, durability, and idempotency.

```
Your Sidecar (Go / Python / Java)
      │  UDS
      ▼
 atome-engine  ──outbox──▶  NATS  ──▶  MongoDB (read model)
```

Community tier: free to deploy, ≤ 5 GB, 1 000 ops/s (No-Cliff mode at 500 ops/s — never drops writes). No registration required.

→ **[get-stratos-labs](https://github.com/get-stratos-labs)** — SDKs (Go · Python · Java) and sidecar templates are MIT.

---

## Stratos Brain — First-Pass Architectural Diagnostic

A multi-agent system (built on Claude Code) that turns a target repository into a set of bounded, specialised agents — exploration, architecture, reliability, concurrency, transactional integrity, security — followed by an adversarial **falsifier** pass that tries to disprove every finding before it ships.

Design principles:

- **Verified findings** — every finding carries a `file:line` reference validated against the actual repository.
- **Reproducible defects** — a reproduction path or trigger condition, typically spanning ≥ 2 files.
- **Counter-evidence on every finding** — the strongest argument *against* it, stated explicitly.
- **No repository scores** — no grades, no certifications, no security theater.

First-pass benchmark across **10 open-source repositories**:

| Metric | Value |
|---|---|
| Findings | 44 — 27 require an immediate fix · 8 recommended actions |
| Citations resolved to `file:line` | 89% |
| Falsifier kill rate | 4.1% — findings destroyed before delivery |
| Severity demotion rate | 13% — over-rated findings recalibrated down |
| Cross-analyst confirmation | 25% — findings independently surfaced by ≥ 2 agents |
| Run completion | 100% |

Published, anonymised, reproducible: **→ [First-Pass-Architectural-Reviews](https://github.com/hugovantighem/First-Pass-Architectural-Reviews)**

> Independent critique strongly encouraged. If a finding is wrong, say so — and say why.

### Calibration phase — looking for 5 testers

I run a full diagnostic on a project of your choice — a microservice, a side-project, or a public OSS repo for full confidentiality. In exchange: an honest, written critique of the report's quality and relevance.

→ Reach out on [LinkedIn](https://www.linkedin.com/in/hugo-vantighem-9669a14b).

---

## Links

- ⚙️ **Atome** — [get-stratos-labs](https://github.com/get-stratos-labs)
- 🔬 **Stratos Brain benchmarks** — [First-Pass-Architectural-Reviews](https://github.com/hugovantighem/First-Pass-Architectural-Reviews)
- ✍️ **Blog** — [medium.com/@hugo.vantighem](https://medium.com/@hugo.vantighem)
- 💼 **LinkedIn** — [hugo-vantighem](https://www.linkedin.com/in/hugo-vantighem-9669a14b)

---

Open to **Principal / Staff Engineer** positions and **architecture consulting** — remote or France-based. Reach out on LinkedIn.
