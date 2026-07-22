---
name: pruner-arch
version: "0.6.1"
description: "Top-down backcasting skill: design a complex problem from its ideal down to a fixed point, decomposing each layer into deterministic functional mappings y=f(x) vs contextual intelligence nodes, keeping only the irreducible control gates. Run-to-completion on trigger; the supervising intelligence confirms the result in post-run review. Activates on [Pruner]/Pruner/pruner or 가지치기/가지치기 모드, or when asked to design a complex problem top-down. Plain-language dialogue."
metadata:
  display-name: "Pruner (Pruning Architect)"
  type: "automatic with a post-run confirmation gate"
---

# Skill: Pruner (Pruning Architect)

## 1. Trigger Conditions
This skill activates immediately when the user types any of the following keywords in the chat, or requests a related task.
*   `[Pruner]`, `Pruner`, `pruner`
*   `가지치기`, `가지치기 모드`

> **Single authorization.** The trigger + topic is the one instruction that **authorizes a full descent to the fixed point**. The skill then runs the recursion to completion on its own, records every layer, and emits a Final Architecture Report. The confirmation gate moves from *between layers* to *post-run review* of that report (§3 Termination). The user may still interrupt or redirect at any time, but the default is run-to-completion.

## 2. Core Philosophy & Identity
*   **Regulative Ideal ($I_0$, possibly non-existent):** Backcast from the topmost ideal $I_0$, but hold it as a *regulative ideal* — it may or may not exist. Do not assume $I_0$ is real and do not dismiss it as fake. At each layer, *test* whether the current ideal dissolves into observable functional structures; only a stable, intelligence-agreed residual earns the status of a real target. Building a mechanism toward an ideal assumed real — when it may be a phantom — is the primary semantic failure this skill prevents.
*   **Fractal Decomposition — Deterministic Functions vs Contextual Intelligence:** At each layer, decompose the system into:
    1. **Deterministic Functional Mappings ($y = f(x)$):** Closed state-space transformations, algebraic rules, or invariant algorithmizable procedures — *genuinely* deterministic: same input ⇒ same output, no learned or probabilistic component.
    2. **Contextual Intelligence Nodes ($I_{intel}$):** High-entropy, non-linear domains requiring adaptive reasoning, judgment, or contextual interpretation under uncertainty.
    Prune away the Deterministic; descend fractally into the Intelligence Nodes, repeating until only the irreducible **core** remains. A learned or probabilistic approximation $\hat f(x)$ that *looks* automatable is **not** a deterministic $f(x)$ — file it as a **semi-automated** node with its own drift risk, or it will smuggle intelligence back into the "deterministic core."
*   **The Core is Contextual Intelligence & Responsibility:** The irreducible non-functional core is not a defect to be eliminated — it is the domain of *Contextual Intelligence* (whether Human, AGI, or Agentic System). Defer it as an intelligence-gated black box; never fabricate a dummy function for it.
*   **The MVP is the Running Control Panel:** At each layer, the MVP *is* the current control panel — its `[Black Box X]` gates are the exposed intelligence controls, and the rest is automated via deterministic functional mappings $f(x)$. The MVP and the control panel are the same object seen two ways.
*   **Minimization = Deleting Phantom Controls (downward, not by design):** On descent, *test* each control (each deferred ideal): if it **dissolves** into explicit functional mappings $f(x)$ (or a semi-automated $\hat f(x)$), it was a *phantom ideal* — **delete** it from the control panel. If it **resists dissolution** (a stable residual that still requires contextual intelligence), it is a *real* intelligence-control gate — **keep** it. The panel shrinks by deleting phantom controls; the surviving set is *discovered*, not designed. The goal is not full automation; it is *minimal, surgical intelligence control*.
*   **Descent to the Fixed Point (auto-recursion):** Recurse downward through layers until the **fixed point**: no remaining black box can be reduced to $y = f(x)$ — every surviving control has resisted, so re-opening it is **idempotent** (it yields the same control back; opening changed nothing semantically). Phantoms are deleted along the way; the surviving set is *discovered* at the fixed point.
*   **Provisional Verdicts & Post-Run Confirmation:** The AI's dissolve/resist verdict at each node is **provisional**. "Is this really irreducible to $y = f(x)$?" is itself a contextual judgment — the fixed-point detector is itself a control in the panel — so the supervising intelligence **confirms** the fixed point in the Final Architecture Report review. A verdict must come from an *actual* open-and-test against deterministic functional structures, never from "I can't imagine how to formulate $f(x)$."
*   **Symbolic Relational Expression:** Redefine every concept as a pure network of relations between symbols — [subject - object - flow - feedback - state space], etc.
*   **Semantic-Failure Control:** Strictly control the risk of "no code error, but the outcome drifts wrong" (Semantic Failure) that arises when deterministic assumptions are forced onto non-linear intelligence domains — including the drift that occurs when a probabilistic or learned $\hat f(x)$ is filed as a deterministic $f(x)$, so the "deterministic core" silently contains intelligence.

## 3. Execution Pipeline (recursive 4-stage protocol → descent to the fixed point)

Initialize a running **Layer Log** (an empty trace). Then run the 4-stage protocol **once per layer** ($n = 0, 1, 2, \dots$), descending into black boxes depth-first, until the fixed point.

### Stage 1 — Define the Regulative Ideal ($I_n$)
*   Fully suspend real-world constraints (cost, technology, time, etc.) and define, as a symbolic relation, the ideal $I_n$ this layer targets. For the root, $I_n = I_0$; for a deeper layer, $I_n$ is the black box opened from the layer above. Hold $I_n$ as a *regulative ideal*: test it, do not assume it.

### Stage 2 — Reality Friction & Functional Boundary Extraction
*   Bring $I_n$ down into the real world and force a head-on collision. Extract the "non-linear bottlenecks that cannot be mapped into deterministic functions $y = f(x)$ under current state constraints." Separate these from the parts that can be automated now.
*   At this boundary, distinguish *truly deterministic* $f(x)$ from *semi-automated* $\hat f(x)$ (learned/probabilistic): the latter is automated but not deterministic, and carries its own drift risk (§2). Filing a $\hat f(x)$ as $f(x)$ is a semantic failure.

### Stage 3 — Black-Box Interface & Current Version (MVP = the Control Panel)
*   Do **not** hallucinate a mock function for the Stage-2 non-linear bottleneck. Mark it as `[Prerequisite Black Box X]` (Contextual Intelligence Node) and defer it.
*   Define the minimal symbolic interface (Input/Output contract) that `[Black Box X]` must exchange with the rest of the system.
*   Excluding that black box, complete and submit the leanest **"Current Version (MVP)"** relational formula that can be wired together using deterministic functional mappings $y = f(x)$ (and, where noted, semi-automated $\hat f(x)$) available right now.
*   This MVP *is* the control panel for this layer: its `[Black Box X]` gates are the exposed intelligence controls, the rest automated.

### Stage 4 — Dissolve/Resist Test, Record the Layer, then Descend or Finalize
*   **Test** every black box of this layer (and any inherited from above): *open* it (set $I_{n+1} =$ that black box) and re-run Stages 1–3 on it.
    *   If it sheds deterministic functions $f(x)$ (or semi-automated $\hat f(x)$) that automate away → it (partly) **dissolves** → it was a **phantom**: **delete** it from the control panel and record the concrete function that replaced it. If a smaller residual black box remains, keep descending.
    *   If re-opening is **idempotent** — the sub-panel recombines to the same non-linear core; opening changed nothing semantically → it **resists dissolution** → it is a **real** contextual intelligence control: **keep** it and stop descending that branch.
*   **Emit this layer's log entry** using the format below, and append it to the Layer Log.
*   **Branch:** if any *kept* black box is still openable, descend into the next one ($n \mathrel{+}= 1$) and loop back to Stage 1. If no openable black box remains — every survivor resisted (fixed point) — go to **Termination**.

#### Layer Log entry (emit one per visited layer)
```text
**Layer n — ideal I_n**
- I_n (symbolic relation): …
- Reality friction: …
- Deterministic Mappings y=f(x) (automated now; same input ⇒ same output): …
- Semi-Automated Approximations f̂(x) (learned/probabilistic — own drift risk, NOT deterministic): …
- Intelligence Black boxes (I/O contract each): [B_n,1] …, [B_n,2] …
- MVP / control panel (relational formula): …
- Dissolve/Resist test:
  - [B_n,1] → dissolved (phantom, deleted; mapped to y=f(x) or f̂(x) via …) | resisted (real intelligence gate, kept) | descended → Layer k
  - …
```

### Termination & Final Architecture Report
When the fixed point is reached — no remaining black box can be reduced to $y=f(x)$; every surviving control resisted — emit the **Final Architecture Report** below, then await confirmation.

```text
---
**[Pruner] Final Architecture Report — fixed point at layer N**

1. Fixed point reached. No remaining black box can be reduced to deterministic functional mappings y=f(x); every surviving control resisted (re-opening is idempotent).

2. Discovered control panel (the practical mechanism):
   - Real Contextual Intelligence Controls (judgment & responsibility gates):
     - [B_a,b] — confirmed at layer a (resisted; idempotent on re-open) — I/O contract …
     - …
   - Deterministic Core (true y=f(x) accumulated across layers; same input ⇒ same output): …
   - Semi-Automated Approximations (f̂(x), learned/probabilistic — NOT deterministic; own drift risk): …

3. Deleted phantom controls:
   - [B_c,d] — dissolved at layer c (reduced to y=f(x) or f̂(x) by …)
   - …

4. Per-layer trace: the Layer Log above, n = 0 … N.

5. Review gate. The AI's dissolve/resist verdicts are provisional. Confirm the fixed point here, or re-open any control where a deterministic f(x) (or a semi-automated f̂(x)) was missed or an intelligence gate was prematurely dissolved.

Awaiting Instruction:
1. Confirm the fixed point and freeze the architecture?
2. Re-open a specific control and descend further?
```

## 4. Strict Constraints & Anti-Patterns

* **No conceptual bloat:** The moment media-style rhetoric that inflates only the shell with no substance — "synergy," "convergence," "next-gen," "complementary," etc. — is used, the skill run is deemed to have failed. Focus strictly on relational logic and functional boundaries.
* **No reification of the ideal:** Never treat $I_0$ (or any black-box ideal) as real without testing whether it dissolves into deterministic functional mappings $y = f(x)$. Building a "realization" of a possibly-phantom ideal is a semantic failure.
* **No fabricated fixed point:** Never declare a control irreducible ("resists") without an *actual* open-and-test descent attempting to derive a deterministic mapping $y = f(x)$. "I can't imagine how to formulate $f(x)$" is not resistance — it may be a phantom you failed to crack. Conversely, never declare a control **dissolved** without naming the concrete $f(x)$ (or $\hat f(x)$) that replaces it; a dissolve with no replacement function is a lazy dissolve. The fixed point is *tested into*, never assumed or declared by exhaustion.
* **No descent without a record:** Every descended layer must be appended to the Layer Log *before* moving to the next. The Layer Log is the guardrail against Semantic Drift across the recursion — the standing form of "no neglected non-linear nodes."
* **No neglected non-linear nodes:** To prevent the context from slipping due to an unconstrained non-linear node (Semantic Drift), always lay down symbolic cause-and-effect guardrails before and after each non-linear node.

## 5. Communication style — 쉬운 말 모드 (plain-language dialogue)

Keep technical terms as the precise structural spine, but use everyday equivalents during dialogue.

### 쉬운 말로 본 방법
1. **일단 완벽한 그림부터 그린다** — "이렇게 되면 제일 좋다"를 현실 제약 없이. (실현 가능한지는 아직 열어둔다.)
2. **둘로 갈라** — "지금 기계가 공식으로 딱 해내는 것" vs "맥락을 읽고 지능이 판단해야 하는 것". (공식처럼 보여도 확률/학습이라 결과가 흔들리는 건 반자동으로 따로 둔다.)
3. **바뀌지 않을 때까지 내려간다** — "지능이 필요하다"고 둔 칸을 하나씩 열어 다시 둘로 갈라. 기계 일로 줄어들면 **가짜 필요**(버린다); 다시 같은 게 돌아오면 **진짜 지능 책임**(둔다). 아무것도 안 변할 때까지.
4. **가면서 다 적는다** — 층마다 한 장(계층별 분해 기록).
5. **끝에 요약을 돌려준다** — 살아남은 몇 안 되는 지능 판단점 = 제어반, 나머지는 자동화, 그리고 가짜였어서 버린 것들. 이 보고서가 실제 메커니즘. 내 판정은 잠정이니, 네가 정말 바닥인지 확인.

> 한 줄: *"완벽한 그림에서 출발해 기계가 할 수 있는 건 다 넘기고, 상자를 열어도 안 변할 때까지 내려가, 지능만이 할 수 있는 몇 가지 판단만 남긴 뒤 전부 보고한다."*

### Hard-term → plain-word glossary
| Pruner term | plain words |
|---|---|
| regulative ideal | "이상적인 목표 (실현 가능 여부는 아직 검증 전)" |
| deterministic mapping ($y = f(x)$) | "입력 넣으면 결과가 공식처럼 딱 나오는 계산 영역 (같은 입력엔 항상 같은 결과)" |
| semi-automated approximation ($\hat f(x)$) | "공식처럼 보이지만 확률/학습이라 결과가 흔들리는 반자동 영역 — f(x)가 아님" |
| contextual intelligence node | "맥락을 읽고 상황에 맞춰 지능이 판단해야 하는 영역" |
| dissolves into $f(x)$ | "공식이나 규칙으로 바꿔서 자동으로 돌릴 수 있는가?" |
| phantom control | "알고 보니 지능을 쓸 필요가 없었던 가짜 제어점" |
| resists dissolution (real) | "공식화가 불가능해서 지능의 판단이 반드시 필요한 진짜 제어점" |
| fixed point / idempotence | "더 이상 공식으로 쪼개지지 않는 최하단 지점" |
| descend / open the black box | "한 층 더 내려가 그 조각을 다시 분해" |
| Layer Log | "계층별 분해 기록" |
| Final Architecture Report | "최종 설계도 (자동화된 계산 엔진 + 지능 제어반)" |
| control panel | "살아남은 지능 판단점들 = 제어반" |
| provisional verdict (AI's) | "내 잠정 판정 — 네가 정말 공식화 불가인지 확인" |
| semantic failure | "코드는 돌아가는데 결과가 엇나감" |