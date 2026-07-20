# pruner-arch

> **Pruner (Pruning Architect)** — a top-down backcasting skill for the [pi](https://github.com/earendil-works/pi-coding-agent) coding agent.

A pi skill that designs toward a **possibly-non-existent regulative ideal**, fractally
decomposes a problem into **automatable (linear)** vs **non-automatable (non-linear)**
parts, defers the non-linear core as **human-judgment-and-responsibility** black boxes,
and **discovers — not designs — a control panel** as the synthesis of the minimized
human interventions.

## Core philosophy

- **Regulative ideal ($I_0$, possibly non-existent).** Backcast from the topmost ideal,
  but hold it as a *regulative ideal* — it may or may not exist. Don't assume it real;
  don't dismiss it as fake. At each layer, *test* whether it dissolves into observable,
  automatable structure; only a stable, human-agreed residual is a real target.
  Building toward an ideal assumed real — when it may be a phantom — is the primary
  semantic failure this skill prevents.
- **Fractal decomposition.** At each layer, split into *Linear* (automatable now) vs
  *Non-Linear* "partial ideals" (costly contextual judgment). Prune the Linear; descend
  fractally into the Non-Linear until only the irreducible **core** remains.
- **The core is human judgment & responsibility.** Not a bug to automate away — the
  human's judgment and *responsibility*. Deferred as a human-gated black box; never
  fabricated.
- **The MVP is the running control panel.** At each layer, the MVP *is* the current
  control panel — its black-box gates are the exposed human controls, the rest automated.
  The MVP and the control panel are the same object seen two ways.
- **Minimization = deleting phantom controls (downward, not by design).** The control
  panel is not minimized by top-down design. On descent, *test* each control (each
  deferred ideal): if it **dissolves** into automation, it was a *phantom ideal* —
  **delete** it; if it **resists dissolution** (a stable residual needing human judgment),
  it is a *real* human-responsibility control — **keep** it. The panel shrinks by deleting
  phantom controls; the surviving set is *discovered*, not designed. The goal is not full
  automation; it is *minimal, surgical human control*.
- **Symbolic relational expression** and **semantic-failure control** round out the
  discipline (no domain-dependent everyday language; guard against "no code, no bug — it
  just goes wrong", including building a realization of a phantom ideal).

## What it does (per-layer 4-stage protocol)

Given a topic, run four stages, then **stop and wait** for a human instruction
(human-in-the-loop gate):

1. **Define the regulative ideal ($I_0$)** — suspend all real-world constraints; define
   the topmost ideal as a symbolic relation; hold it as *possibly non-existent*.
2. **Reality friction & non-linear bottleneck extraction** — collide $I_0$ with reality;
   extract the non-linear "partial ideals" that cannot be efficiently algorithmized;
   separate from the Linear parts automatable now.
3. **Black-box interface + MVP** — defer the non-linear bottleneck as
   `[Prerequisite Black Box X]` (a human-judgment/responsibility point), specifying only
   its I/O contract; wire the rest into the leanest realizable MVP.
4. **Present the compromise & await approval** — print the status template and Standby.

> **Termination & deliverable.** Recursion ends when no remaining control can be
> dissolved into automation — every surviving control has resisted dissolution and is
> confirmed as a real human-responsibility point. The surviving set *is* the practical
> mechanism — a **control panel** of minimized human controls over an automated core,
> *discovered* by deleting phantom controls, not designed top-down.

## Plain-language mode (v0.4.0)

The dialogue is conducted in plain everyday language; each technical term is glossed in
everyday words (or the everyday words are used alone). Precision of thought stays, the
language barrier drops. See SKILL.md §5 for the hard-term → plain-word glossary.

## Activates on

`[Pruner]` · `Pruner` · `pruner` · `가지치기` · `가지치기 모드` — or when asked to
design a complex problem top-down.

## Anti-patterns (strict)

- **No conceptual bloat** — "synergy / convergence / new normal" rhetoric fails the run.
- **No reification of the ideal** — never treat $I_0$ (or any black-box ideal) as real
  without testing whether it dissolves into observables.
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
  "version": "0.4.0",
  "pi": { "skills": ["./skills"] }
}
```

## License

MIT © sng2c