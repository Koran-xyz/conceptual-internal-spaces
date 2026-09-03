# Natural-Language Programming, Policy Authoring, and the Boundary of Dialogic Language Theory

Status: Working comparison note for Paper 2
Date: 2026-09-03

## Purpose

This note tests the proposed Dialogic Language Theory / Dialogic Construction Methodology against adjacent work in natural-language programming, end-user programming, prompt-based application construction, and natural-language policy authoring.

The purpose is not to claim novelty prematurely. It is to remove claims already covered by neighboring fields and identify a narrower research object that remains worth testing.

## 1. Natural-language programming is not the novelty

Prior work already treats natural language as an interface for creating executable behavior. Research on end-user programming with LLMs studies how humans describe information-processing tasks in ordinary language and how well an LLM can realize those descriptions. Other natural-language programming work translates lay descriptions into programs or methods.

Therefore, Paper 2 should not claim novelty merely because:

- natural language can specify behavior;
- a non-programmer can create a system through language;
- an LLM can turn a human description into executable behavior;
- prompts can function as reusable program-like specifications.

These are established or actively studied directions.

## 2. Natural-language policy authoring is also not the novelty

Current agent infrastructure can already accept authorization requirements in natural language, translate them into formal policies, validate them against schemas, analyze problematic permissions, and enforce them externally at runtime.

This is especially important for the present research program because it shows that "writing AI rules in natural language" is no longer, by itself, a defensible novelty claim.

Natural-language policy authoring and Dialogic Language Theory should therefore be distinguished carefully.

A typical policy-authoring pipeline can be summarized as:

Human already has policy requirement -> natural-language specification -> translation/formalization -> validation -> enforcement.

The proposed dialogic method instead focuses on an earlier and more open-ended construction problem:

Human defines problem and intended objective -> human and AI examine the problem -> candidate rule/structure proposed -> candidate is challenged or revised -> human evaluates objective/value/safety fit -> candidate is instantiated in an AI environment -> observable consequences are examined -> result returns to the next dialogue cycle.

The distinction is not that one uses natural language and the other does not. Both can use natural language.

The candidate distinction is that the dialogic method studies **how the rule or structure itself is discovered, negotiated, revised, replaced, or reused before and after implementation**, rather than primarily translating an already-defined requirement into an enforceable representation.

## 3. Prompt engineering is not enough

Modern prompts can define complex application behavior. Research increasingly treats prompting as a form of end-user software construction.

Therefore the proposed method should not be positioned as "better prompt engineering" or as the discovery that prompts can create persistent application behavior.

Its candidate research object is the **construction process that produces and revises the specification**, including the reasoning boundary between human objectives and AI-operational considerations.

## 4. Candidate distinctive unit: the dialogic construction cycle

The smallest proposed unit of analysis is not a prompt and not a final policy.

It is a cycle:

1. Human-defined problem
2. Human-defined objective and constraints
3. Candidate proposal from human or AI
4. Dialogic examination of the candidate
5. Human-governed adoption, rejection, revision, replacement, or deferral
6. Instantiation as a rule, procedure, role, or structure
7. Observation of behavior or operational consequences
8. Return of the observation to dialogue

This creates a **construction trajectory** across multiple cycles.

## 5. Two distinct evaluation axes

A central clarification is that "good for the AI" must not mean "advantageous to the AI."

Candidate rules or structures should be evaluated along at least two conceptually separate axes.

### Axis A — Human objective and governance fit

Does the candidate remain consistent with the human-defined purpose, values, safety boundaries, and acceptable operating conditions?

The human retains authority over the problem definition and adoption decision.

### Axis B — AI-operational coherence

Given the observable behavior of the AI environment, is the candidate understandable, internally coherent at the interaction level, usable, and capable of supporting the intended function without obvious contradiction or unnecessary complexity?

An AI's approval is not evidence that a proposal is safe, correct, or aligned with human interests. AI-generated proposals remain candidates subject to human evaluation.

## 6. Important distinction from policy compilation

Natural-language policy systems can perform sophisticated translation and automated validation. This narrows the Paper 2 claim substantially.

Paper 2 should not claim:

> Natural language lets humans create AI policies.

A more defensible research question is:

> Can a human-governed dialogue with an AI be operationalized as a repeatable method for discovering, evaluating, instantiating, observing, and revising rules or adaptive structures when the final specification is not fully known at the start?

This focuses on **construction under incomplete specification**, rather than translation of a pre-existing specification.

## 7. Candidate novelty boundary after this comparison

The current candidate contribution is the combination of the following elements, not any single element alone:

1. **Human-originated problem definition** — the purpose and problem originate with the human.
2. **Bidirectional solution proposal** — either participant may propose candidate solutions, while proposal authority is distinct from adoption authority.
3. **Human-governed adoption** — AI preference or agreement is never sufficient for adoption.
4. **Dual evaluation** — human-purpose fit and AI-operational coherence are treated as separate questions.
5. **Construction under incomplete specification** — the final rule or structure need not be known when dialogue begins.
6. **Instantiation and observation** — the constructed rule or structure is used, not merely discussed.
7. **Feedback into reconstruction** — observed behavior can cause revision, rejection, replacement, or reuse.
8. **Trajectory as research data** — the sequence of proposals, decisions, implementations, observations, and revisions is retained as an analyzable object.
9. **Structure variability** — the method does not prescribe one permanent architecture; structures may be replaced when a more effective realization is found.

These elements still require a deeper literature audit before any strong novelty claim.

## 8. Relationship to the broader research program

This comparison clarifies the relationship between Paper 2 and the other planned papers.

Paper 2 studies **how structures are constructed through dialogue**.

Paper 1 studies whether natural-language-constructed rule functions can be observed and compared across LLM environments.

Future internal/external/hybrid work studies **where functions should be realized**.

Agent-versus-layer work studies **what structural realization is appropriate for a persistent function**.

Shared-workspace work studies **how multiple heterogeneous AI systems can coordinate without requiring identical internal structures**.

Thus Paper 2 should not absorb the empirical claims of the other papers. It provides the methodological trunk from which those construction decisions can be documented and studied.

## 9. Strongest current formulation

A cautious current formulation is:

> Dialogic Language Theory investigates a human-governed method of constructing AI-facing rules and adaptive structures through iterative natural-language dialogue. The human defines the problem and intended objective; candidate solutions may originate from either the human or AI; adoption remains human-governed; and implemented structures are observed and recursively reconsidered through further dialogue. The research object is not dialogue alone, nor natural-language programming alone, but the traceable construction trajectory connecting problem definition, proposal, decision, implementation, observation, and reconstruction.

This is a working formulation, not a final novelty claim.

## 10. Sources checked in this comparison

- Pickering et al. (CHI 2025), *How Humans Communicate Programming Tasks in Natural Language and Implications for End-User Programming with LLMs*.
- Sarkar et al. (PPIG 2022), *What is it like to program with artificial intelligence?*
- Sarkar (Onward! 2023), *Will Code Remain a Relevant User Interface for End-User Programming with Generative AI Models?*
- Weigelt et al. (ACL 2020), *Programming in Natural Language with fuSE*.
- NoviCode / Natural Language Programming work on generating structured programs from everyday language.
- Amazon Bedrock AgentCore Policy documentation (accessed 2026-09-03), including natural-language policy authoring, Cedar/Dogwood translation, validation, analysis, and external enforcement.

## 11. Next comparison target

The remaining novelty audit should focus on literature that may already combine several of the elements above, especially:

- interactive specification and requirements negotiation with LLMs;
- human-AI value elicitation and preference construction;
- iterative policy design and constitutional rule revision;
- interactive machine teaching;
- reflective or self-refining agent design in which humans retain governance;
- design-science and action-research methodologies where artifacts are iteratively built and evaluated.

Only after this comparison should Paper 2 state a formal novelty contribution.