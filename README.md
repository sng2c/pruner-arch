# pruner-arch

> **Pruner (Pruning Architect)** — a top-down backcasting skill for the [pi](https://github.com/earendil-works/pi-coding-agent) coding agent.

A pi skill that designs toward a **possibly-non-existent regulative ideal**, fractally
decomposes a problem into **deterministic functional mappings $y=f(x)$** vs
**contextual intelligence nodes** ($I_{intel}$), defers the non-linear core as
**intelligence-gated** black boxes, and **discovers — not designs — a control panel**
as the synthesis of the minimized intelligence controls. Learned/probabilistic
approximations $\hat f(x)$ are filed as **semi-automated** with their own drift risk,
never as deterministic $f(x)$. It **recurses downward to the fixed point** (no
remaining black box reduces to $y=f(x)$; every survivor resists, re-opening is
idempotent), keeps a **per-layer Layer Log**, and emits a **Final Architecture
Report**; the supervising intelligence authorizes the full descent via the trigger
and confirms the fixed point in post-run review.

## Core philosophy

- **Regulative ideal ($I_0$, possibly non-existent).** Backcast from the topmost ideal,
  but hold it as a *regulative ideal* — it may or may not exist. Don't assume it real;
  don't dismiss it as fake. At each layer, *test* whether it dissolves into observable
  functional structures; only a stable, intelligence-agreed residual is a real target.
  Building toward an ideal assumed real — when it may be a phantom — is the primary
  semantic failure this skill prevents.
- **Fractal decomposition.** At each layer, split into *Deterministic* ($y=f(x)$,
  automatable now, same input ⇒ same output) vs *Contextual Intelligence* nodes
  (high-entropy, non-linear domains). Prune the Deterministic; descend fractally into
  the Intelligence Nodes until only the irreducible **core** remains. A learned or
  probabilistic $\hat f(x)$ that *looks* automatable is **not** a deterministic $f(x)$ —
  file it as semi-automated with its own drift risk.
- **The core is contextual intelligence & responsibility.** Not a defect to eliminate —
  the domain of *Contextual Intelligence* (Human, AGI, or Agentic System). Deferred as
  an intelligence-gated black box; never fabricated.
- **The MVP is the running control panel.** At each layer, the MVP *is* the current
  control panel — its black-box gates are the exposed intelligence controls, the rest
  automated. The MVP and the control panel are the same object seen two ways.
- **Minimization = deleting phantom controls (downward, not by design).** The control
  panel is not minimized by top-down design. On descent, *test* each control (each
  deferred ideal): if it **dissolves** into $f(x)$ (or $\hat f(x)$), it was a *phantom
  ideal* — **delete** it; if it **resists dissolution** (a stable residual needing
  contextual intelligence), it is a *real* intelligence-control gate — **keep** it. The
  panel shrinks by deleting phantom controls; the surviving set is *discovered*, not
  designed. The goal is not full automation; it is *minimal, surgical intelligence
  control*.
- **Symbolic relational expression** and **semantic-failure control** round out the
  discipline (no domain-dependent everyday language; guard against "no code error, but
  the outcome drifts wrong", including the drift from filing a $\hat f(x)$ as $f(x)$).

## What it does (recursive 4-stage protocol → descent to the fixed point)

Given a topic, the trigger authorizes a **full descent to the fixed point**. The skill
keeps a **Layer Log** and runs the 4-stage protocol once per layer ($n = 0, 1, 2, \dots$),
descending into black boxes depth-first, until the fixed point:

1. **Define the regulative ideal ($I_n$)** — suspend all real-world constraints; define
   the ideal as a symbolic relation; hold it as *possibly non-existent*. ($I_0$ at the
   root; $I_n$ is the black box opened from the layer above for deeper layers.)
2. **Reality friction & functional boundary extraction** — collide $I_n$ with reality;
   extract the non-linear bottlenecks that cannot be mapped to deterministic $y=f(x)$;
   separate from the automatable parts, and at this boundary distinguish truly
   deterministic $f(x)$ from semi-automated $\hat f(x)$ (learned/probabilistic, own drift
   risk).
3. **Black-box interface + MVP** — defer the non-linear bottleneck as
   `[Prerequisite Black Box X]` (a contextual-intelligence node), specifying only its
   I/O contract; wire the rest into the leanest realizable MVP (the control panel for
   this layer).
4. **Dissolve/resist test, record, then descend or finalize** — open each black box and
   re-run Stages 1–3 on it: if it sheds $f(x)$/$\hat f(x)$ it was a **phantom** (delete,
   naming the replacement); if re-opening is **idempotent** it **resists** (keep, real
   control). **Emit the layer's log entry**. If any kept box is still openable, descend
   and loop; else the fixed point is reached.

> **Termination & deliverable.** Recursion ends at the fixed point — no remaining control
> can be reduced to $y=f(x)$; every survivor resisted, re-opening is idempotent. The
> surviving set *is* the practical mechanism — a **control panel** of minimized
> intelligence controls over a deterministic core (plus a semi-automated $\hat f(x)$
> layer with its own drift risk), *discovered* by deleting phantom controls, not designed
> top-down — and delivered as the **Final Architecture Report** with the full per-layer
> trace, for the supervising intelligence to confirm in post-run review.

## Plain-language mode (v0.6.1)

The dialogue is conducted in plain everyday language (쉬운 말 모드); each technical term
is glossed in everyday words (or the everyday words are used alone). Precision of
thought stays, the language barrier drops. See SKILL.md §5 for the hard-term → plain-word
glossary and the plain-language walkthrough.

## Activates on

`[Pruner]` · `Pruner` · `pruner` · `가지치기` · `가지치기 모드` — or when asked to
design a complex problem top-down.

## Anti-patterns (strict)

- **No conceptual bloat** — "synergy / convergence / next-gen / complementary" rhetoric
  fails the run.
- **No reification of the ideal** — never treat $I_0$ (or any black-box ideal) as real
  without testing whether it dissolves into deterministic $y=f(x)$.
- **No fabricated fixed point** — never declare a control irreducible ("resists")
  without an *actual* open-and-test descent that tried to derive $y=f(x)$; "I can't
  think of how to formulate $f(x)$" is not resistance. Conversely, never dissolve a
  control without naming the concrete $f(x)$ (or $\hat f(x)$) that replaces it. The fixed
  point is *tested into*, never assumed.
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
  "version": "0.6.1",
  "pi": { "skills": ["./skills"] }
}
```

## License

MIT © sng2c