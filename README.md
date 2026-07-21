# pruner-arch

> **Pruner (Pruning Architect)** — a top-down backcasting skill for the [pi](https://github.com/earendil-works/pi-coding-agent) coding agent.

A pi skill that designs toward a **possibly-non-existent regulative ideal**, fractally
decomposes a problem into **automatable (linear)** vs **non-automatable (non-linear)**
parts, defers the non-linear core as **human-judgment-and-responsibility** black boxes,
and **discovers — not designs — a control panel** as the synthesis of the minimized
human interventions. It **recurses downward to the fixed point** (no remaining black box
dissolves; every survivor resists, re-opening is idempotent), keeps a **per-layer Layer
Log**, and emits a **Final Architecture Report**; the human authorizes the full descent
via the trigger and confirms the fixed point in post-run review.

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

## What it does (recursive 4-stage protocol → descent to the fixed point)

Given a topic, the trigger authorizes a **full descent to the fixed point**. The skill
keeps a **Layer Log** and runs the 4-stage protocol once per layer ($n = 0, 1, 2, \dots$),
descending into black boxes depth-first, until the fixed point:

1. **Define the regulative ideal ($I_n$)** — suspend all real-world constraints; define
   the ideal as a symbolic relation; hold it as *possibly non-existent*. ($I_0$ at the
   root; $I_n$ is the black box opened from the layer above for deeper layers.)
2. **Reality friction & non-linear bottleneck extraction** — collide $I_n$ with reality;
   extract the non-linear "partial ideals" that cannot be efficiently algorithmized;
   separate from the Linear parts automatable now.
3. **Black-box interface + MVP** — defer the non-linear bottleneck as
   `[Prerequisite Black Box X]` (a human-judgment/responsibility point), specifying only
   its I/O contract; wire the rest into the leanest realizable MVP (the control panel for
   this layer).
4. **Dissolve/resist test, record, then descend or finalize** — open each black box and
   re-run Stages 1–3 on it: if it sheds Linear parts it was a **phantom** (delete); if
   re-opening is **idempotent** it **resists** (keep, real control). **Emit the layer's log
   entry** (running per-layer report). If any kept box is still openable, descend and loop;
   else the fixed point is reached.

> **Termination & deliverable.** Recursion ends at the fixed point — no remaining control
> can be dissolved; every survivor resisted, re-opening is idempotent. The surviving set
> *is* the practical mechanism — a **control panel** of minimized human controls over an
> automated core, *discovered* by deleting phantom controls, not designed top-down — and
> delivered as the **Final Architecture Report** with the full per-layer trace, for the
> human to confirm in post-run review.

## Plain-language mode (v0.5.0)

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
- **No fabricated fixed point** — never declare a control irreducible ("resists")
  without an *actual* open-and-test descent that wired real linear structure into it; "I
  can't think of how to automate it" is not resistance. Conversely, never dissolve a
  control without naming the concrete automation that replaces it. The fixed point is
  *tested into*, never assumed.
- **No descent without a record** — every descended layer is appended to the Layer Log
  before moving on; the log is the guardrail against Semantic Drift across the recursion.
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
  "version": "0.5.0",
  "pi": { "skills": ["./skills"] }
}
```

## License

MIT © sng2c