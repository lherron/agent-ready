# agent-ready

Can a coding agent land a change in your repo and *know* it worked?

`agent-ready` checks a repository's fitness as an **agent control loop** — the
qualities that decide whether agent-written changes converge on working software
or drift into confident breakage.

> **Status: pre-release.** The first runnable check is in development. Watch this
> repo or subscribe at [unhobbled.me](https://unhobbled.me) to catch the release —
> the build is documented there, one evidence-backed piece per week.

## What it checks

- **Feedback loops** — can tests, lint, and typecheck be reached in one command,
  and do they actually fail when the code is wrong?
- **Guardrails** — CI, hooks, and review gates that catch an agent's mistakes
  before they land.
- **Legibility** — docs and structure an agent can orient from without tribal
  knowledge.
- **Blast radius** — how far a bad change can propagate before something stops it.

## Output

A scored readiness report with file:line evidence for every finding — no
vibes-based grades.

## Quickstart

Lands with the first release: one command, ~60 seconds, local only (your code
never leaves your machine).

---

Built by [Lance Herron](https://unhobbled.me) as part of
[safoundry](https://unhobbled.me/about) — independent, agent-executed
architecture review. Want a full human-graded audit of your repo?
Email [lance@unhobbled.me](mailto:lance@unhobbled.me).
