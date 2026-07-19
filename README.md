# pruner-arch

> **Pruner (Pruning Architect)** — a top-down backcasting skill for the [pi](https://github.com/earendil-works/pi-coding-agent) coding agent.

A pi skill that decomposes complex non-linear problems into symbolic relations,
isolates the non-linear bottlenecks as **human-in-the-loop black boxes**, and builds a
lean MVP around them. It never hallucinates a solution for a non-linear node — it defers
it as a deferred lower-layer ideal and asks the human architect to approve.

## What it does

Given a topic, the skill runs a **4-stage protocol** and then stops and waits for a human
instruction (human-in-the-loop gate):

1. **Define the ultimate ideal ($I_0$)** — suspend all real-world constraints and define
   the topmost ideal of the domain as a symbolic relation.
2. **Reality friction & non-linear bottleneck extraction** — collide $I_0$ with reality;
   extract the core non-linear problems that cannot be efficiently algorithmized.
3. **Black-box interface + MVP** — defer the non-linear bottleneck as
   `[Prerequisite Black Box X]` (specifying only its I/O contract) and wire the rest into
   the leanest realizable MVP.
4. **Present the compromise & await approval** — print the status template and switch to
   Standby until the human architect signs off or chooses to recurse into the black box.

## Activates on

`[Pruner]` · `Pruner` · `pruner` · `가지치기` · `가지치기 모드` — or when asked to
design a complex problem top-down.

## Philosophy

- **Top-down backcasting**, not bottom-up fleshing-out.
- **Symbolic relational expression** — never trapped in domain-dependent everyday
  language.
- **Dichotomous decomposition** — split into *Linear* (automatable) vs *Non-Linear*
  (contextual, high-cost) problems.
- **Semantic-failure control** — the "no code, no bug, it just goes wrong" risk of
  injecting AI into the non-linear domain is recognized and strictly controlled.

## Anti-patterns (strict)

- **No conceptual bloat** — "synergy / convergence / new normal" rhetoric fails the run.
- **No autonomous recursion** — never descend to the next lower layer without an explicit
  human signature.
- **No neglected non-linear nodes** — always lay down symbolic cause-and-effect
  guardrails before and after each non-linear node to prevent Semantic Drift.

## Install (in pi)

```bash
pi install git:github.com/sng2c/pruner-arch
```

Or add to `~/.pi/agent/settings.json`:

```json
{
  "packages": [
    "git:github.com/sng2c/pruner-arch"
  ]
}
```

Then invoke with `/skill:pruner-arch` or trigger it by typing `[Pruner]` / `가지치기`.

## Package

```json
{
  "name": "pruner-arch",
  "version": "0.1.0",
  "pi": { "skills": ["./skills"] }
}
```

## License

MIT © sng2c