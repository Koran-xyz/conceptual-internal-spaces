# Paper 2 — Exact-Combination Prior-Art Search

Status: Working research note — novelty not yet established
Date: 2026-09-03

## Purpose

This note tests whether the current proposed combination behind 対話式言語理論 (working English label still provisional) already appears as a substantially equivalent established methodology under another name.

The target combination is intentionally narrow:

1. a human originates and defines the problem and intended objective;
2. the candidate rule or structure is not assumed to be known in advance;
3. human and AI use iterative natural-language dialogue to generate and revise candidate rules or structures;
4. proposals may come from either side, but adoption remains human-governed;
5. candidate proposals are evaluated along at least two distinguishable dimensions: fit to the human-defined objective and operational reasonableness in the AI environment;
6. an adopted rule or structure is actually instantiated or used;
7. observable consequences are fed back into later dialogue and reconstruction;
8. the trajectory from problem to proposal, decision, implementation, observation, and reconstruction is treated as an analyzable research object.

## Closest work found in this search

### 1. DesignerlyLoop (DIS 2026)

DesignerlyLoop is a particularly close adjacent result. It addresses iterative and nonlinear human–LLM design, separates design intent from LLM reasoning, lets users reorganize/correct/regenerate reasoning, and propagates refined intent or reasoning into subsequent decisions.

Overlap:
- iterative human–LLM construction;
- evolving human intent;
- explicit manipulation and revision of AI-supported reasoning;
- propagation of earlier decisions into later design work.

Important difference for the present research question:
- its principal object is design-intent formulation and curated reasoning in a design interface;
- it does not, from the material inspected here, establish the exact proposed methodology of discovering natural-language behavioral rules/AI structures, instantiating those rules in an AI environment, observing their behavioral consequences, and recursively using those consequences as evidence for reconstruction.

This substantially narrows any novelty claim. “Iterative dialogue that progressively forms intent or structure” cannot itself be claimed as new.

### 2. Human–AI iterative physical/design refinement

Recent HCI work studies LLM-generated designs that are physically instantiated, evaluated, fed back to an LLM, and iteratively refined by a human designer.

Overlap:
- proposal → implementation → evaluation → feedback → refinement is clearly not unique;
- empirical results can be returned into a human–AI construction loop.

Difference:
- the artifact is a domain design rather than a natural-language rule/AI-governance structure;
- therefore the generic closed-loop pattern cannot be the novelty. Any contribution must be specific to rule/structure construction, governance, operationalization, and traceable reconstruction.

### 3. Learned natural-language rules for human–AI teams (Mozannar et al., 2023)

This work learns local natural-language rules describing when humans should collaborate with or ignore AI suggestions, based on discovered regions in data, and teaches those rules to humans.

Overlap:
- natural-language rules;
- human–AI collaboration;
- rule discovery rather than merely rule transcription.

Difference:
- rules are algorithmically learned/described from behavioral/data regions for onboarding;
- the inspected description does not use the proposed human-defined-problem → dialogic candidate construction → human adoption → AI-environment instantiation → observation → dialogic reconstruction methodology.

This means “discovering natural-language rules” alone is also not a defensible novelty claim.

### 4. Co-constructive LLM dialogue research

SIGDIAL work investigates whether LLMs can participate in co-constructive explanation dialogues, including monitoring/scaffolding and use of dialogue context.

Overlap:
- dialogue as a co-constructive process;
- mutual development rather than one-shot instruction following.

Difference:
- the constructed object is understanding/explanation, not a rule or system structure that is subsequently instantiated and behaviorally observed.

Thus “co-construction through dialogue” cannot itself be claimed as new.

### 5. Human–AI shared-workspace and sensemaking research

Recent work also studies shared workspaces that support human steering, AI response visualization, fact checking, and iterative sensemaking.

Overlap:
- externalized shared state;
- iterative human–AI sensemaking;
- traceable context and revision.

Difference:
- these systems focus on sensemaking and workspace interaction rather than the full lifecycle of discovering, adopting, operationalizing, observing, and reconstructing natural-language AI rules/structures.

### 6. DialogLab and conversational rule authoring

DialogLab supports authoring conversational scenes, agent personas, group structures, turn-taking rules, and transitions.

Overlap:
- natural-language/conversational system configuration;
- explicit rules and agent/group structures.

Difference:
- the primary problem is authoring and testing conversational scenarios, not discovering initially unknown governance/behavioral structures through the proposed human-governed recursive construction process.

## Negative finding from this search

Within the sources located and inspected in this search, I did **not** identify a peer-reviewed or clearly established methodology that obviously matches all eight elements of the target combination as one named method.

This is **not evidence that no such work exists**. Search coverage is incomplete, terminology varies across HCI, requirements engineering, AI alignment, design science, interactive machine teaching, end-user programming, policy authoring, and agent engineering, and future searches may locate closer precedents.

Therefore the paper should use language such as:

> “We did not identify, in the literature reviewed to date, a method explicitly combining these elements.”

It should **not** say:

> “This is the first method to…”

without a systematic review capable of supporting that statement.

## Major refinement: the generic loop is not novel

The current search makes one point especially clear:

> Build → evaluate → feedback → revise is already common across design and human–AI collaboration research.

Likewise, none of these components alone is a plausible novelty claim:
- natural-language dialogue;
- co-creation;
- mixed initiative;
- human final authority;
- design rationale/traceability;
- natural-language rules;
- iterative refinement;
- implementation followed by evaluation.

The contribution, if supported, must be in the **specific organization and operationalization of these components for discovering and reconstructing AI rules/structures**.

## Sharpened candidate contribution

A more defensible candidate contribution is:

> A human-governed dialogic construction method for cases in which the problem and objective are human-defined but the appropriate AI rule or structure is initially unknown. The method treats natural-language interaction not merely as an interface for specifying a predetermined artifact, but as the medium through which candidate rules/structures are generated, evaluated, selected, operationalized, behaviorally observed, and recursively reconstructed. The resulting construction trajectory is retained as research evidence.

This is still a **candidate contribution**, not an established novelty claim.

## Proposed formal cycle

The working cycle should now be represented as:

**Human problem definition**
→ **Human objective / constraints**
→ **Dialogic exploration**
→ **Candidate proposal (human or AI)**
→ **Dual evaluation**
   - human-objective fit
   - AI-environment operational reasonableness
→ **Human-governed decision**
   - adopt / revise / reject / defer / replace / reuse
→ **Operationalization**
→ **Behavioral observation**
→ **Evidence return**
→ **Dialogic reconstruction**
→ repeat as needed.

The phrase “dual evaluation” must not imply that an LLM can reliably determine its own hidden operational constraints. In empirical work, “AI-environment operational reasonableness” must be grounded in observable responses, documented constraints, tests, and explicit uncertainty—not model self-report alone.

## Safety/governance boundary

The methodology must explicitly reject an interpretation in which AI preference determines policy.

AI agreement is not sufficient evidence of:
- correctness;
- safety;
- human-value alignment;
- legitimacy;
- feasibility.

The human defines the problem/objective and retains adoption authority. AI proposals are candidate solutions evaluated against human-defined purposes and observable system behavior.

This is important because persuasive or fluent model output can cause human over-reliance. The method therefore needs an explicit anti-deference principle:

> **No proposal is adopted merely because the AI recommends or endorses it.**

## Revised research questions

### RQ1 — Method
Under what conditions can human-initiated natural-language dialogue function as a repeatable method for discovering, constructing, and revising AI rules or adaptive structures when the solution is not predetermined?

### RQ2 — Decision process
How can proposals originating from either the human or AI be evaluated and traced while preserving human-defined objectives and human-governed adoption?

### RQ3 — Recursive reconstruction
How do observations produced after operationalizing an adopted rule or structure influence subsequent dialogue, rejection, revision, replacement, or reuse?

### RQ4 — Reproducibility
Which parts of the construction trajectory must be recorded so that another researcher can distinguish the original problem, candidate proposals, decision rationale, operationalized structure, observed behavior, and later reconstruction?

## What should be recorded in a Construction Trajectory

For each meaningful design transition:

- `problem_definition`
- `human_objective`
- `constraints`
- `proposal`
- `proposal_origin` (human / AI / jointly synthesized)
- `alternatives_considered`
- `human_objective_fit_assessment`
- `operational_reasonableness_evidence`
- `decision` (adopt / revise / reject / defer / replace / reuse)
- `decision_rationale`
- `operationalized_rule_or_structure`
- `environment`
- `observed_result`
- `uncertainty_or_confounds`
- `next_problem_or_revision`

This schema converts historical conversational development into a form that can later support case-study analysis without pretending that unavailable historical metadata exists.

## Strong candidate case studies from the research program

These are candidates only; historical evidence must be checked before publication.

1. Safety meta-rule → Guardian proposal → Guardian agent → Guardian Layer.
2. Agent structuralization/interference problem → external observer and external board/storage alternatives.
3. Handoff coordination → shared-workspace coordination.
4. Broad LTA hypothesis → narrower CIS operational framework and Functional Convergence hypothesis.

These cases are useful precisely because they contain revisions, failures, replacements, and changes of realization rather than only successful final artifacts.

## Current novelty boundary

After this search, the safest current position is:

> The research does not claim novelty for human–AI dialogue, co-creation, mixed initiative, natural-language rules, iterative design, traceability, or feedback-driven refinement individually. It investigates whether their particular integration can be operationalized as a reproducible, human-governed methodology for discovering and reconstructing initially unknown AI rules and structures through natural-language interaction and behavioral feedback.

## Next step

The literature-boundary phase is now mature enough to stop endlessly broadening the search.

Next work should move from “Is anything remotely similar?” to **formalizing the method itself**:

1. define the minimum required stages;
2. define optional stages;
3. define decision authority;
4. define evidence requirements;
5. define failure conditions;
6. define a Construction Trajectory record format;
7. reconstruct one historical case using that format;
8. then test whether an independent person could follow the method on a new problem.

That transition is necessary if Paper 2 is to become a methodology paper rather than only a literature-positioning essay.
