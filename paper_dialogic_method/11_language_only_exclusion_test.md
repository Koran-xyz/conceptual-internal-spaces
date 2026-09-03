# Language-Only Exclusion Test for Adjacent AI-Environment Construction Research

**Status:** Working literature-screening note for Paper 2

## 1. New Screening Criterion

The comparison is narrowed from "Does prior work structure an AI environment?" to a stricter question:

> **Is the resulting AI environment constructed and maintained through natural language itself, without Python, source-code modification, model-weight modification, formal workflow code, API orchestration code, or another executable implementation layer being required as part of the construction method?**

This criterion matters because Dialogic Construction Methodology is intended to investigate language itself as the construction medium, rather than merely using natural language as a front end that is translated into code.

For this screening step, systems that accept natural-language input but generate, invoke, or depend on executable code underneath are treated as adjacent but excluded from the closest-comparator set.

This is a methodological exclusion criterion for the present comparison. It is not a claim that code-based or hybrid approaches are inferior.

## 2. Three Categories

### Category A — Language-only construction candidate
The research must aim to construct the relevant AI-facing rule/role/boundary/coordination structure through natural-language artifacts and dialogue, with no required executable construction layer supplied by the method.

### Category B — Natural-language front end over coded infrastructure
The user may interact without writing code, but the method internally generates code, calls APIs, compiles formal policies, constructs executable workflow graphs, or depends on a coded orchestration framework. These systems are **not language-only** under the present definition.

### Category C — Code/hybrid architecture
The architecture itself is implemented using programming frameworks, workflow languages, graph specifications, APIs, or other executable infrastructure. These are excluded from the closest-comparator set even when natural-language instructions appear inside the architecture.

## 3. Initial Re-screening of Close Comparators

### AutoAgent — Excluded from closest-comparator set
AutoAgent explicitly presents itself as a zero-code framework for end users and allows users to create tools, agents, and workflows through natural language. This is a very important adjacent system because its user-facing construction process is unusually close to language-only interaction.

However, it remains a software framework / Agent Operating System whose implementation creates and manages executable agents, tools, files, and workflows. "Zero-code" describes the user's interaction requirement, not the absence of an underlying executable construction layer.

**Classification:** Category B.

**Reason for exclusion:** natural language is a construction interface to an implemented agent framework rather than the sole persistent construction substrate.

### AIAP — Excluded from closest-comparator set
AIAP is a no-code workflow builder that translates ambiguous natural-language requests into functional AI workflows using multi-agent collaboration. It also maps user intent to services/actions and establishes API connections.

**Classification:** Category B.

**Reason for exclusion:** the output is an operational workflow integrating tools/services/APIs; natural language hides implementation complexity rather than replacing the implementation layer.

### Text2BIM — Excluded
Text2BIM accepts natural-language design instructions but transforms them into imperative code that invokes BIM software APIs.

**Classification:** Category B/C.

**Reason for exclusion:** natural language is explicitly translated into code.

### Multi-agent code generation systems — Excluded
Systems that convert plain-language requests into tested code through LangGraph, Docker, Python, or similar infrastructure are not language-only construction methods.

**Classification:** Category B/C.

### Infrastructure-as-Code multi-agent systems — Excluded
Systems that use LLM agents to produce Terraform or other infrastructure code are structurally oriented but their target artifact is executable code.

**Classification:** Category C.

### Enterprise / reference agent architectures — Excluded from closest set
Reference architectures such as enterprise agentic architectures and multi-agent reference architectures may include natural-language interfaces, but orchestration, plugins, memory, routing, APIs, and control mechanisms are implemented as software architecture.

**Classification:** Category C.

## 4. A Particularly Important Near Match: Natural Language Architecture (NLA)

A public project titled **Natural Language Architecture Templates** describes natural language as the primary architecture medium for system and OS-level structures. It is explicitly tool-agnostic and model-agnostic and distinguishes itself from ordinary prompts and agents. It focuses on layers, flows, feedback loops, governance, and system-level structure.

This is conceptually much closer to the present research direction than many coded agent frameworks.

However, its own description says the language-native architecture can later be implemented in **code, no-code, or hybrid stacks**. Its stated purpose is primarily to capture architectural intent and prepare designs that other teams/tools can implement. It therefore appears to use natural language primarily as an **architecture/design representation**, rather than demonstrating that the natural-language structure itself functions as the operative AI environment without a subsequent implementation layer.

It is also currently a public GitHub methodology/template project rather than, on the evidence reviewed here, an established peer-reviewed research program demonstrating the same human–AI dialogic construction cycle.

**Classification:** potential Category A-adjacent comparator; requires continued monitoring and careful citation/status labeling.

**Key distinction to test:**

> Is natural language merely the specification of an architecture, or is the natural-language artifact itself the operative structure that organizes AI behavior?

This distinction may be central to Paper 2.

## 5. Revised Core Distinction

A much sharper distinction is now available:

### Natural-language interface
Human describes a system in language; software/code/formal policy/workflow machinery realizes it.

versus

### Natural-language construction substrate
The language-defined rules, roles, boundaries, relationships, and coordination structures themselves remain the operative construction used by the AI environment.

Dialogic Construction Methodology is intended to investigate the second case.

This means that "no-code for the user" is **not sufficient** for inclusion. The question is whether code is merely hidden from the user or whether code is unnecessary to the structure being studied.

## 6. Stronger Working Definition

For the present research program, a **language-only AI-environment construction** is provisionally defined as:

> A construction in which the operative organization of rules, roles, boundaries, relationships, memory conventions, or coordination functions is expressed and maintained through natural-language artifacts and interaction, without requiring those artifacts to be translated into executable code, formal policy languages, model-weight changes, or a platform-specific orchestration program in order to constitute the studied structure.

External storage of language artifacts does not automatically violate this definition. For example, storing a rule document in a board or document service is different from requiring Python code to interpret and execute the architecture. This boundary must be stated explicitly in future experiments.

## 7. Important Consequence for Platform Independence

This criterion strengthens the earlier **Portable Methodology, not Portable Architecture** position.

If the operative construction is language-based rather than code-based, then portability can be tested without requiring the same programming framework on every platform.

The hypothesis becomes more specific:

> **Can natural-language-defined structures preserve intended functions across heterogeneous AI environments without requiring a shared executable implementation layer?**

This is substantially narrower than generic model-agnostic or no-code claims.

## 8. What Must Still Be Searched

The next search should prioritize work that satisfies all of the following simultaneously:

1. The target is an AI environment or AI-facing organizational structure, not merely a task answer or physical artifact.
2. The operative structure is made from natural-language rules/roles/relationships/boundaries.
3. The structure itself functions without translation into Python, workflow code, formal policy code, or a platform-specific executable architecture.
4. Human–AI dialogue participates in discovering or revising the structure.
5. The final structure is not predetermined.
6. The approach is intended to transfer across heterogeneous AI systems or does not depend on one open-source model.

The literature reviewed so far contains many systems matching several of these criteria, but this stricter language-only filter removes many of the previously close comparators.

## 9. Caution

No novelty claim follows automatically from this exclusion test. In particular, "no code" must not be confused with "no hidden software infrastructure": every hosted LLM service necessarily runs on software. The relevant distinction is whether the **researcher's construction method and operative structure require an additional executable architecture beyond the natural-language artifacts being studied**.

This distinction should be operationalized before formal empirical claims are made.
