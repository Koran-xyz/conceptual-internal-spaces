# Portable Methodology and Platform Independence

**Status:** Working conceptual boundary for Paper 2

## 1. Design Goal

Dialogic Construction Methodology is designed to be **model- and implementation-agnostic**. It does not require access to model weights, source code, fine-tuning infrastructure, or a particular open-source LLM. It is intended to operate through the interface most broadly shared across heterogeneous AI systems: natural-language interaction.

This is a design objective, not yet an empirically established universal property.

## 2. Open-Source Independence

The methodology does not assume that the user can inspect or modify the underlying model. Therefore, its core procedure should in principle remain applicable to:

- proprietary hosted LLM services,
- open-source or open-weight models,
- local AI systems,
- platform-specific assistants,
- future systems that expose sufficiently capable natural-language interaction.

Open-source systems may provide additional experimental access, but such access is not a prerequisite of the methodology itself.

## 3. Portable Methodology, Not Portable Architecture

The central portability claim is not that one identical architecture must be copied across platforms.

Different environments may realize a required function through different structures. For example, a function may be realized through contextual/internal construction in one environment, an external shared artifact in another, or a hybrid arrangement elsewhere.

Accordingly, the target is better described as **Portable Methodology rather than Portable Architecture**.

What is intended to transfer is the construction process:

1. Human defines the problem and objective.
2. Human and AI develop candidate rules or structures through dialogue.
3. Candidates are examined for human-purpose consistency and operational coherence in the target environment.
4. Human governs adoption, rejection, or revision.
5. The selected construction is instantiated in a form available to that environment.
6. Observable behavior is evaluated.
7. Observations are returned to dialogue and may trigger reconstruction.
8. The construction trajectory is recorded.

The resulting implementation is allowed to differ across environments.

## 4. Relation to Functional Convergence

This distinction connects Paper 2 to the Functional Convergence hypothesis developed in Paper 1.

If heterogeneous AI environments can realize comparable rule-related functions through different structural realizations, then platform independence need not require structural identity.

The relevant question becomes:

> Can a common dialogic construction methodology produce functionally comparable outcomes across heterogeneous AI environments even when the resulting structures differ?

This is a testable bridge between the two papers.

## 5. Candidate Differentiation Axis

The literature review conducted so far indicates that none of the following alone is sufficient as a novelty claim:

- human-AI dialogue,
- iterative co-creation,
- mixed initiative,
- human final decision authority,
- natural-language programming,
- natural-language policy authoring,
- design rationale or traceability,
- build-evaluate-refine cycles.

The stronger candidate contribution is therefore the **combination and explicit methodological organization** of:

- a human-originated problem and objective,
- rule/structure discovery when the solution is not predetermined,
- iterative natural-language construction,
- proposals from either participant within the human-defined objective,
- explicit separation of human-purpose consistency from AI-environment operational coherence,
- human-governed adoption,
- deployment into the available target environment,
- observation-driven reconstruction,
- traceable construction trajectories,
- and a deliberate goal of model- and implementation-agnostic portability.

This combination remains a **candidate contribution**, not a confirmed novelty claim.

## 6. What Platform Independence Does Not Mean

Platform independence does not mean:

- identical outputs across all models,
- identical internal mechanisms,
- identical architectures,
- guaranteed compatibility with every AI system,
- bypassing platform safety policies or technical constraints,
- or independence from empirical validation.

Instead, it means that the methodology is intentionally defined above the level of any single model implementation and allows environment-specific structural realizations.

## 7. Revised Candidate Research Question

> **RQ-P:** Under what conditions can a natural-language dialogic construction methodology remain portable across heterogeneous AI environments while allowing the resulting rule or system structures to differ?

A related empirical question is:

> When structural realization differs across platforms, which intended functions remain comparable, which diverge, and why?

## 8. Provisional Paper 2 Positioning

A cautious positioning statement is:

> **Dialogic Construction Methodology is proposed as a human-initiated, natural-language-based method for discovering, constructing, evaluating, deploying, and revising rules or adaptive structures without requiring access to a particular model's source code, weights, or implementation. Rather than requiring portable architectures, it aims for a portable construction methodology whose resulting structures may adapt to the constraints of heterogeneous AI environments.**

This statement describes the intended methodological contribution. Claims of actual cross-platform portability require systematic empirical validation.

## 9. Terminology Note: Method Rather Than Fixed Form

The distinction between portable methodology and portable architecture also supports the intended meaning of the Japanese name **対話式言語理論**: the emphasis is on a method or way of constructing through dialogue rather than on prescribing one fixed structural form.

The English terminology remains provisional and should be finalized only after the conceptual and literature-positioning work is complete.
