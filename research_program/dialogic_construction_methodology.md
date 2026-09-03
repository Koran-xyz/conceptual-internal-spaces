# Dialogic Construction Methodology and the Research Program

**Status:** Working research framework  
**Researcher:** Minoru Shimizu  
**Purpose:** To document the methodological trunk connecting the current natural-language rule research, Conceptual Internal Spaces (CIS), cross-platform functional convergence, and future work on common AI rules.

## 1. Starting Point

This research program did not begin with an attempt to discover or construct a hidden internal architecture inside an AI system. Its practical starting point was simpler: improving an AI working environment that felt inefficient and repetitive.

That practical problem led to a safety question. If a working environment is modified through natural-language rules, how can those rules avoid causing unintended behavior outside their intended context? This motivated an early principle that rules defined for a particular context should not override established rules outside that context.

From this point, the research question gradually became broader:

> Can natural language be used to construct common rule functions that remain meaningful across different AI environments?

The present research program develops from this question.

## 2. Dialogic Construction Methodology

The working term **Dialogic Construction Methodology** refers to a method in which a human and an AI construct and revise rules or structures through iterative natural-language dialogue.

A simplified cycle is:

**Problem discovery → Dialogue → Proposal → Mutual evaluation → Adoption or revision → Construction → Observation → Further dialogue**

Proposals are not assumed to originate only from the human. Either participant may identify a problem, suggest a possible solution, question an existing rule, or propose a modification. When neither participant has an adequate solution, the problem remains open for further joint exploration.

The methodology therefore does not prescribe one fixed architecture. It describes a process for constructing, evaluating, replacing, and reusing structures as research progresses.

## 3. Method Before Structure

An important historical distinction in this research is that the observed structures came after the construction method.

The research did not begin by assuming the existence of a Conceptual Internal Space. Natural-language rules were first developed for practical organization and safety. During continued construction and observation, context-sensitive boundaries, rule separation, role behavior, and other structural phenomena became research objects in their own right.

CIS was subsequently introduced as an operational framework for describing and testing some of these observable phenomena.

Accordingly:

> **The method preceded the structural interpretation.**

CIS should therefore not be treated as the origin or totality of the research program.

## 4. Research Genealogy

The current research line can be represented as:

**Dialogic Construction Methodology**  
↓  
**Natural-language rule construction**  
↓  
**Context, boundary, and rule-structure behavior**  
↓  
**Conceptual Internal Spaces (operational framework)**  
↓  
**Cross-platform comparison of rule-related functions**  
↓  
**Cross-Platform Functional Convergence Hypothesis**  
↓  
**Comparison of internal, external, and hybrid realizations**  
↓  
**Future research on common AI rules and coordination norms**

This genealogy is not intended to imply that every stage is already empirically established. Some stages are observed research developments, some are operational concepts, and some remain hypotheses or future research directions.

## 5. Stable Method, Changing Implementations

A recurring principle of the research program is that implementations are replaceable.

An agent, layer, shared board, memory store, internal construction, external construction, or hybrid arrangement should not be preserved merely because it was used previously. If another realization performs the required function more efficiently, safely, or reproducibly, the implementation may be replaced.

The core dialogic construction method, however, has remained comparatively stable across the present research program: identify a problem, discuss it, construct a candidate solution, observe the result, and revise when necessary.

This distinction can be summarized as:

> **Structures may change; the construction methodology provides continuity.**

This is a description of the current research history, not a claim that the methodology can never itself be revised.

## 6. Internal, External, and Hybrid Realizations

The research has also raised a placement question: must a useful rule or coordination function be realized inside a constructed AI context?

Exploratory work suggests three design categories worth comparing:

- **Internal realization:** rule or coordination functions are constructed within the active AI context.
- **External realization:** functions are placed in an external shared structure, such as a board or store.
- **Hybrid realization:** local/internal functions and shared/external functions are combined according to purpose.

The important research target is therefore not structural identity across platforms. Different AI environments may realize comparable functions through different structures or placements.

This motivates the broader functional question underlying the current working paper: under what conditions do comparable rule-related functions emerge even when their structural realizations differ?

## 7. Relationship to the Current Working Paper

The current Working Paper v0.2, **Natural-Language Rule Construction Across LLM Environments: An Exploratory Study of Conceptual Internal Spaces and Cross-Platform Functional Convergence**, examines one experimentally tractable part of this larger program.

It does not attempt to validate the entire Dialogic Construction Methodology. Instead, it narrows the investigation to observable natural-language rule behavior, scope conditions, CIS as an operational framework, and possible functional convergence across heterogeneous LLM environments.

The broader methodology provides the research genealogy; the working paper provides a bounded empirical target.

## 8. Long-Term Direction

The long-term objective is not to impose one universal architecture on all AI systems. The research instead asks whether people and AI systems can collaboratively develop understandable rule functions and coordination norms that remain useful across heterogeneous environments.

A useful analogy is that technical safety mechanisms can protect individual systems, while shared environments may additionally require understandable behavioral rules for interaction and coordination.

The eventual content of such common rules is intentionally left open. Determining what should be shared, what should remain platform-specific, how rules should be evaluated, and how disagreement should be handled are themselves research questions.

For that reason, the project is intended to remain open to replication, criticism, alternative implementations, negative results, and contributions from other researchers.

## 9. Current Status

This document is a research-program map rather than an empirical result. It records the methodological continuity connecting multiple experiments and constructions while keeping established observations separate from hypotheses and future directions.

Experimental validation should proceed independently through bounded protocols. Research development does not need to stop while individual experiments are waiting for suitable technical conditions.