# Dialogic Construction Methodology — Scope and Research Questions

**Status:** Paper 2 — Working draft v0.1  
**Researcher:** Minoru Shimizu

## Provisional Title

**Dialogic Construction Methodology: Human–AI Co-Construction of Rules and Adaptive Structures Through Natural-Language Interaction**

## 1. Research Object

This paper treats the **process of human–AI dialogue itself as a construction method**.

The research object is not a particular agent architecture, prompt template, internal space, board, or software platform. Those are possible artifacts produced or revised through the method.

The proposed methodological cycle is:

**Problem discovery → Dialogue → Proposal → Mutual evaluation → Adoption or revision → Construction → Observation → Further dialogue**

Either the human or the AI may identify a problem or propose a candidate solution. The resulting structure is not assumed to be permanent. It may be revised, replaced, removed, externalized, recombined, or reused when conditions change.

## 2. Core Research Question

> **RQ1: Under what conditions can iterative natural-language dialogue between a human and an AI function as a reproducible method for constructing and revising rules or adaptive structures?**

This formulation deliberately asks about conditions and reproducibility rather than claiming that dialogue always produces effective structures.

## 3. Secondary Research Questions

> **RQ2: How does construction differ when initiative can originate from either the human or the AI, rather than from the human alone?**

> **RQ3: What observable decision process transforms a conversational proposal into an adopted, revised, rejected, replaced, or reused rule or structure?**

> **RQ4: Which parts of the method remain stable when the resulting implementation changes across tasks, AI environments, or stages of the research process?**

> **RQ5: How can the method preserve traceability so that later researchers can distinguish human proposals, AI proposals, negotiated decisions, observations, interpretations, and subsequent revisions?**

## 4. Central Claim Boundary

The paper does **not** initially claim that:

- AI and humans possess identical agency or responsibility;
- every dialogue is genuinely collaborative;
- the method is universally effective across all AI systems;
- an AI proposal reveals an autonomous hidden intention;
- one fixed architecture should result from the method;
- existing human–AI co-creation research has not already studied iterative or mixed-initiative collaboration.

The narrower candidate contribution is that **natural-language dialogue can be studied as a repeatable construction process in which rules and system structures themselves become revisable artifacts**.

## 5. Provisional Novelty Target

Existing human–AI co-creation and mixed-initiative research already studies iterative interaction, shared initiative, design artifacts, and collaborative workflows. Therefore, novelty cannot rest merely on the statement that humans and AI can create things together.

The present paper will investigate a narrower combination:

1. **Rules and system structures are the construction artifacts**, not only text, images, designs, or task outputs.
2. **Initiative is bidirectional at the proposal level**: either participant may surface a problem or candidate modification.
3. **Acceptance is explicit and traceable**: proposals may be adopted, revised, rejected, replaced, or deferred.
4. **Implementations are intentionally non-fixed**: continuity is sought in the construction method rather than architectural identity.
5. **Failures and replacements are part of the method**, rather than being removed from the research history.
6. **The method can generate later testable branches**, such as CIS, agent-versus-layer design, internal/external/hybrid realization, and shared-workspace coordination.

These points are provisional positioning claims and require a full literature review before any novelty claim is finalized.

## 6. Relationship to Existing Research Areas

The literature review should explicitly compare the proposed methodology with at least the following areas:

- Human–AI co-creation and co-design.
- Mixed-initiative interaction and mixed-initiative co-creativity.
- Iterative design and reflective design processes.
- Human–AI collaborative problem solving.
- LLM-based agent and role design.
- Interactive context construction and management.
- Design-science approaches in which a process or artifact is iteratively constructed and evaluated.

Recent work already treats human–AI co-creation as iterative and, in some cases, mixed-initiative. This overlap should be treated as a foundation and comparison point, not ignored.

## 7. Candidate Unit of Analysis

A future case-study or protocol-based evaluation can use a **construction episode** as the unit of analysis.

A construction episode begins when a concrete problem or limitation is identified and ends when a candidate response reaches one recorded state:

- adopted;
- adopted with revision;
- rejected;
- deferred;
- replaced by another structure;
- removed after observation;
- reused in a later context.

For each episode, the research record should preserve:

- triggering problem;
- proposer of each candidate idea (human / AI / jointly developed / unclear);
- exact or summarized proposal;
- objections or identified risks;
- decision and rationale;
- resulting implementation;
- subsequent observation;
- later revision or replacement, if any;
- evidence status and missing historical metadata.

## 8. First Testable Proposition

A conservative first proposition is:

> **P1: A dialogic construction process can be made more reproducible when its construction episodes explicitly record the triggering problem, proposal origin, evaluation, decision, implementation, and subsequent observation.**

This proposition concerns traceability of the method. It does not require a claim about hidden AI cognition.

## 9. Historical Case Material

The existing research program contains candidate historical construction episodes that may later be reconstructed as case studies, including:

- development of natural-language safety rules;
- emergence and revision of Guardian-like functions;
- movement from agent-style safety roles toward structural-layer concepts;
- failures caused by excessive structuralization of agent roles;
- development of external observation and board-based structures;
- comparison of internal, external, and hybrid realizations;
- movement from sequential handoff concepts toward shared-workspace coordination.

These are currently **candidate historical cases**, not controlled experimental evidence. Missing records must be marked unavailable rather than reconstructed as fact from memory.

## 10. Immediate Paper-Building Plan

The next stages are:

1. Conduct a focused related-work review and build a comparison matrix.
2. Define the methodology formally enough that another researcher can identify a construction episode in a dialogue log.
3. Select a small number of historical cases with the strongest surviving records.
4. Separate documented dialogue evidence from retrospective interpretation.
5. Develop a prospective logging protocol for future construction episodes.
6. Only after those steps, decide whether the first version should be framed as a methodology paper, design-science paper, case-study paper, or combined exploratory paper.

The purpose of v0.1 is to establish a bounded research object before expanding the theory.