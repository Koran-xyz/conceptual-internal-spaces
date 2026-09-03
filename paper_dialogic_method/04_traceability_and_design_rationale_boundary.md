# Traceability, Design Rationale, and the Boundary of Dialogic Construction Methodology

**Status:** Working related-work analysis  
**Paper:** Dialogic Construction Methodology  
**Purpose:** Test whether the proposed idea of a reproducible "construction trajectory" is already covered by requirements traceability or design-rationale research.

## 1. Why This Comparison Matters

The proposed methodology treats the path from a human-defined problem to an adopted rule or structure as a research object. However, requirements engineering and design-rationale research have long studied why requirements and design decisions exist, how they change, what alternatives were considered, and how decisions can be traced.

Therefore, "we record why a decision was made" cannot by itself be claimed as a novel contribution.

## 2. Requirements Traceability

Requirements traceability links requirements to their sources, related artifacts, later implementation elements, and changes. Pre-requirements-specification traceability also addresses questions such as why a requirement exists, why it changed, and who was involved.

Natural-language processing has been extensively applied to requirements engineering, including the recovery and maintenance of trace links.

### Overlap with Dialogic Construction

Both approaches may preserve:

- the origin of a requirement or rule;
- relationships between an objective and later artifacts;
- changes over time;
- reasons for modification;
- information needed to reconstruct development history.

### Boundary

Requirements traceability primarily asks whether relevant engineering artifacts and their relationships can be followed across a development process.

The proposed Dialogic Construction Methodology instead asks whether a **human–AI dialogue process itself can be used as a repeatable construction method**, where the human defines the problem and objective, candidate rules or structures are generated and challenged through dialogue, and adoption remains human-governed.

This is a candidate distinction, not yet a demonstrated novelty claim.

## 3. Design Rationale and IBIS

Design-rationale research is an even closer neighbor.

IBIS and related approaches organize deliberation around issues, proposed positions or answers, arguments, and resolutions. Process-oriented design-rationale work has explicitly attempted to capture a trace of reasoning during ordinary design activity. Historical field studies recorded large numbers of requirements and design decisions and showed the value of preserving the reasons behind choices.

Therefore, the following ideas are **not novel by themselves**:

- recording alternatives;
- recording arguments for and against alternatives;
- recording why one option was selected;
- preserving decision history;
- making a design process transparent;
- revisiting or reversing a previous decision when its rationale changes.

## 4. Where the Proposed Method May Still Differ

After removing the overlap above, the remaining candidate contribution is narrower.

### 4.1 The AI is a participant in construction, not only a recording or analysis tool

The AI can generate candidate solutions, identify contradictions, suggest revisions, or evaluate whether a proposed rule is operationally coherent within the interaction environment.

However, AI participation alone is not sufficient novelty because human–AI co-design and mixed-initiative systems already study active AI contribution.

### 4.2 The human-defined problem remains the governing anchor

The method begins from a problem and intended objective defined by the human. AI proposals are evaluated relative to that objective rather than accepted because the AI prefers or endorses them.

This creates an explicit asymmetry:

**Human:** defines the problem/objective and governs adoption.  
**Human + AI:** generate, challenge, revise, and evaluate candidate solutions.  
**AI:** may contribute operational reasoning, but its agreement is not treated as proof of correctness.

Human control alone is also not novel; it must be considered part of the combined methodology.

### 4.3 The output can be an executable conversational rule structure

In this research program, the artifact produced by deliberation may itself be a natural-language rule or contextual structure that is then used directly in an AI interaction environment.

Thus the trajectory can connect:

**Problem → Objective → Dialogue → Candidate rule/structure → Challenge/revision → Human adoption → Deployment in dialogue → Observable behavior → New problem**

The final artifact is not necessarily a conventional software requirement or design document. It may be a natural-language behavioral rule, contextual boundary, role definition, coordination structure, or external/shared procedure.

This is a promising boundary, but adjacent work in end-user programming, natural-language programming, policy authoring, and agent configuration must still be checked before claiming novelty.

### 4.4 Construction is intentionally recursive

Observed behavior after deployment becomes input to the next construction cycle. A previously adopted structure may be modified, rejected, replaced, externalized, or reused.

Design-rationale research also tracks evolving decisions, so recursion alone is not novel. The candidate contribution is the combination of recursive human–AI deliberation with direct natural-language construction of the next operational rule or structure.

## 5. Construction Trajectory: Revised Definition

Because "traceability" and "rationale" already have established meanings, **Construction Trajectory** should not be presented merely as a new name for decision history.

For this paper, a construction trajectory is provisionally defined as:

> A recorded sequence linking a human-defined problem and objective to candidate natural-language rules or structures, the human–AI dialogue through which those candidates are proposed and revised, the human-governed adoption decision, the deployed artifact, and the subsequent observable result that may initiate another construction cycle.

A minimal trajectory record should include:

1. **Problem** — what the human is trying to solve.
2. **Objective** — what successful resolution should achieve.
3. **Constraints** — safety, platform, task, or other boundaries.
4. **Candidate** — proposed rule, structure, or procedure.
5. **Proposer** — human, AI, or jointly developed.
6. **Reasoning record** — relevant objections, trade-offs, contradictions, and revisions.
7. **Human decision** — adopt, revise, reject, defer, replace, or reuse.
8. **Artifact** — the actual adopted natural-language rule or structure.
9. **Deployment context** — where and how it was used.
10. **Observed result** — what happened after deployment.
11. **Next problem** — whether the observation initiated another cycle.

This schema deliberately incorporates lessons from traceability and design-rationale research instead of pretending those traditions do not exist.

## 6. A More Defensible Novelty Candidate

At this stage, the paper should **not** claim novelty for dialogue, co-creation, mixed initiative, traceability, rationale capture, human final authority, or iterative revision individually.

The narrower candidate is:

> A human-initiated, human-governed methodology in which natural-language dialogue with an AI is used not only to discuss a design problem but to construct and recursively revise operational natural-language rules or structures, while preserving a trajectory from the human-defined objective through deliberation, adoption, deployment, observation, and subsequent reconstruction.

Even this formulation remains a **novelty candidate** until additional adjacent fields are reviewed.

## 7. Critical Difference Between "AI-Compatible" and "AI-Preferred"

The method must not define a good rule as one that the AI simply accepts, prefers, or finds convenient.

A candidate rule should instead be examined along at least two separate dimensions:

### Human-objective adequacy
Does the candidate preserve the human-defined purpose, constraints, values, and safety requirements?

### Operational coherence
Can the candidate be represented and followed coherently in the relevant AI interaction environment without obvious contradiction or failure?

Neither dimension substitutes for the other.

AI agreement is not evidence of human-objective adequacy. Human desire is not evidence that a proposed construction will function coherently in the AI environment.

## 8. Failure Conditions

The methodology should explicitly count the following as possible failures:

- the AI endorses a candidate that conflicts with the human-defined objective;
- the human accepts an AI proposal without evaluating it;
- the human forces a rule that does not function coherently in the target environment;
- rationale is recorded but the adopted artifact cannot be reconstructed;
- the final artifact changes but the trajectory does not record why;
- dialogue produces agreement but deployment does not produce the intended behavior;
- later behavior contradicts the assumptions used when the rule was adopted.

These failures are scientifically useful because they make the method falsifiable and evaluable rather than merely descriptive.

## 9. Relationship to the Existing CIS Working Paper

The CIS / Functional Convergence paper tests properties of deployed natural-language rules and contextual structures.

The Dialogic Construction Methodology paper asks a different question:

**How did the candidate rule or structure come to be selected and revised in the first place?**

The two papers can therefore connect without collapsing into one another:

**Dialogic Construction Methodology → produces candidate operational structures → CIS / functional experiments test selected observable properties → results return to the next construction cycle.**

## 10. Current Conclusion

The comparison weakens any broad novelty claim based on "traceable dialogue" or "recording why decisions were made." Those ideas have deep precedents in requirements traceability and design rationale.

However, a narrower research target remains plausible: a human-governed construction cycle in which dialogue with an AI produces directly deployable natural-language rules or structures, and observed behavior recursively feeds the next construction decision.

The next literature boundary should test this remaining claim against **end-user programming, natural-language programming, policy/rule authoring, and conversational agent configuration** before the paper states a formal novelty contribution.

## References checked in this boundary review

- Zhao, L., et al. (2021). *Natural Language Processing for Requirements Engineering: A Systematic Mapping Study*. ACM Computing Surveys, 54(3), Article 55. DOI: 10.1145/3444689.
- Guo, J. L. C., Steghöfer, J.-P., Vogelsang, A., & Cleland-Huang, J. (2024). *Natural Language Processing for Requirements Traceability*. arXiv:2405.10845.
- Conklin, E. J., & Yakemovic, K. C. B. (1991). *A Process-Oriented Approach to Design Rationale*. Human–Computer Interaction, 6(3–4), 357–391.
- Tang, A., et al. (2007). *A rationale-based architecture model for design traceability and reasoning*. Journal of Systems and Software.

**Evidence note:** This document is a related-work boundary analysis. It does not establish that the proposed methodology is novel.