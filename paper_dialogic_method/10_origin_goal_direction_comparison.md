# Origin–Goal–Direction Comparison of Adjacent Research

**Status:** Working literature-positioning note for Paper 2

## 1. Why Method Similarity Is Not Enough

Prior-art comparison for Dialogic Construction Methodology should not stop at whether another study uses similar techniques such as dialogue, iteration, human oversight, natural language, agents, or structured workflows.

Two studies can share methods while pursuing different research objects and different endpoints. Therefore, the relevant comparison should examine the full research direction:

**originating problem → research goal → role of dialogue/AI → intermediate artifact → final research object or endpoint**.

This note applies that comparison to several close neighboring areas found in the current literature search.

## 2. Current Direction of Dialogic Construction Methodology

The present research program originated from a practical problem: an AI working environment was experienced as repetitive, inefficient, and difficult to use effectively. The initial objective was therefore not to invent a new LLM, optimize model weights, or author a fixed policy language. The objective was to improve the usable AI environment.

Safety then became a foundational constraint: improvements to the environment should not create rules that conflict with established rules or create unintended consequences outside their intended scope.

This led to a research direction in which natural-language rules, dialogue, agents, layers, boundaries, memory, boards, shared workspaces, and other mechanisms are treated as possible construction materials or techniques rather than fixed endpoints.

The primary target is **structure**: an organized AI-facing environment in which rules, roles, boundaries, information stores, interaction pathways, and control functions can be assembled, evaluated, replaced, externalized, internalized, or recombined according to the human-defined purpose.

Accordingly:

> **The methods may vary; the research direction is toward constructing and reconstructing purpose-appropriate AI-facing structures.**

The intended methodology is also designed to be model- and implementation-agnostic: portability concerns the construction method rather than requiring one identical architecture across systems.

## 3. Comparison Axis

For each adjacent work, ask five questions:

1. **Origin:** What problem motivated the research?
2. **Goal:** What was the research trying to improve or produce?
3. **Method:** What role did human–AI interaction, natural language, iteration, or structure play?
4. **Artifact:** What was actually constructed or modified?
5. **Endpoint:** What counts as the successful outcome of the research?

A sixth question is especially important for this program:

6. **Is the AI-facing structure itself the primary evolving research object, or is structure mainly a means to another domain-specific outcome?**

## 4. Adjacent Direction A: Human–AI Co-Design

Recent Human–AI co-design literature studies collaborative design processes in which humans and AI jointly contribute to planning, synthesis, evaluation, ideation, or decision-making. Reviews describe non-linear collaboration, mixed initiative, varying decision authority, and adaptive interaction.

**Origin:** limitations of conventional design workflows and the growing availability of generative AI.

**Goal:** improve human design practice, creativity, decision quality, efficiency, controllability, or interaction.

**Method:** iterative Human–AI collaboration, mixed initiative, generation and evaluation.

**Artifact:** typically a domain design, candidate scheme, product concept, interface, building, lesson plan, or other target-domain artifact.

**Endpoint:** a better design outcome or better human–AI design process.

**Difference in direction:** although the interaction techniques overlap strongly, the AI collaboration environment itself is usually infrastructure for producing another artifact. Dialogic Construction Methodology instead investigates construction of the AI-facing organizational structure as a primary research object.

## 5. Adjacent Direction B: DesignerlyLoop and Reasoning Curation

DesignerlyLoop addresses mismatch between iterative human design intent and discrete LLM interaction. It externalizes design intent and LLM reasoning into inspectable structures that users can reorganize, correct, and regenerate.

**Origin:** human–LLM misalignment during design intent formation.

**Goal:** improve design-intent formulation, reflective control, and output quality.

**Method:** iterative co-reasoning and curation of externalized reasoning structures.

**Artifact:** design-intent and reasoning representations.

**Endpoint:** stronger formulation of design intent and better design outputs.

**Difference in direction:** this is extremely close at the interaction/process level, but its primary endpoint is design cognition and intent formulation. The current dialogic research program instead asks how dialogue can construct the rule/role/boundary/information/control organization of the AI-use environment itself.

## 6. Adjacent Direction C: AI-Assisted Requirements and Decision Frameworks

Frameworks such as GAGT organize requirement analysis, candidate generation, weighting, and human selection into a connected workflow. Requirements Engineering research similarly uses LLMs to elicit, reformulate, validate, prioritize, and trace requirements.

**Origin:** difficulty converting stakeholder needs into reliable design requirements and decisions.

**Goal:** improve requirements quality, candidate generation, prioritization, traceability, or decision support.

**Method:** structured Human–AI workflow with human confirmation and final judgment.

**Artifact:** requirement sets, weighted criteria, candidate solutions, specifications, or decisions.

**Endpoint:** a selected or improved domain solution/specification.

**Difference in direction:** requirements and decisions are usually inputs to or outputs from another engineering/design process. In Dialogic Construction Methodology, rules and requirements can instead become construction elements whose relationships form an evolving AI-facing structure.

## 7. Adjacent Direction D: Human-Governed Prompt/Tool Development

Human-in-the-loop chain-of-code prompting and related approaches iteratively refine prompts, modules, and generated code under expert control. Some explicitly describe the output as an evolving artifact and emphasize reproducibility, modularity, and transparent human control.

**Origin:** difficulty developing reliable deterministic tools with generative AI.

**Goal:** produce functional tools/code aligned with expert research requirements.

**Method:** repeated prompting, generation, expert validation, modular layering, feedback.

**Artifact:** code modules and tools.

**Endpoint:** reliable software/tool development.

**Difference in direction:** the final object is executable software. Dialogic Construction Methodology does not require generated code and is intended to remain usable even where source code, model weights, or programmatic modification are unavailable. Its target is the functional organization of the AI-use environment, potentially realized through natural-language-defined rules and structures alone or in combination with external artifacts.

## 8. Adjacent Direction E: Compound AI System Architecture

Pocketflow/Flow State is a particularly close structural comparator. It explicitly argues for structural clarity and explicit control in compound AI systems, offers modular nodes and flows, supports Human–AI co-design, and describes itself as vendor-agnostic.

**Origin:** complexity, ambiguity, and maintenance problems in compound AI system development.

**Goal:** provide a minimal programming framework for prototyping, refining, and deploying compound AI systems.

**Method:** Human–AI co-design using explicit software abstractions and a Python framework.

**Artifact:** programmed compound AI workflows/systems.

**Endpoint:** maintainable, adaptable, scalable deployed AI systems.

**Similarity:** structural organization, iterative Human–AI design, vendor independence, and adaptability are all close.

**Key directional distinction to test:** Pocketflow begins from software architecture for compound AI systems and provides fixed core programming abstractions. Dialogic Construction Methodology begins from human–AI dialogue as the construction method and deliberately does not prescribe a single architecture or require a programming framework. Structures may differ by environment and may be internal/contextual, external, or hybrid.

This is one of the strongest prior-art comparators and should be treated seriously rather than dismissed as merely similar.

## 9. Adjacent Direction F: Domain-Specific Structural Design

Architectural and structural-design research increasingly uses conversational and multimodal AI to help humans iteratively create evolving physical structures. Some work explicitly supports incomplete specifications, emergent constraints, negotiation, and iterative structural modification.

**Origin:** generative AI systems tend to produce final answers, while professional structural/architectural design requires exploration under evolving constraints.

**Goal:** support creative and technically constrained design of physical structures.

**Method:** conversational Human–AI co-creation and iterative constraint negotiation.

**Artifact:** buildings, layouts, structural models, or other physical-design representations.

**Endpoint:** improved architectural/structural design.

**Difference in direction:** the word “structure” is shared, but the research object is a physical/domain structure. Dialogic Construction Methodology concerns organizational structures governing or supporting AI use itself.

## 10. A Newly Important Comparator: Human–AI Collaboration Architecture

The search also identified experimental frameworks explicitly described as collaboration architectures for sustained Human–AI work, including systems that separate governance, research, knowledge, runtime, memory, or other responsibilities.

These are directionally closer than ordinary co-creation studies because the collaboration environment itself becomes a designed object.

This means the novelty boundary cannot simply be:

> “We construct an AI collaboration environment.”

That territory is already occupied.

The remaining question is narrower:

> **Does prior work begin from the same research stance: treating natural-language dialogue as a portable construction method through which the human and AI discover, select, assemble, observe, and reconstruct the AI-facing structure itself without prescribing a fixed architecture or requiring model/source-code access?**

This is now the critical comparison question.

## 11. Current Assessment

The literature reviewed so far shows substantial overlap in individual techniques and even in some high-level goals:

- Human–AI co-design exists.
- Iterative construction exists.
- Human-governed decision making exists.
- Externalized reasoning structures exist.
- Requirements traceability exists.
- Natural-language programming and policy authoring exist.
- Vendor-agnostic compound-AI frameworks exist.
- Human–AI collaboration architectures exist.
- Iterative structural design under incomplete specification exists.

Therefore none of these should be claimed individually as novel.

However, the **research stance and endpoint** of Dialogic Construction Methodology remain potentially distinguishable. Its current direction can be summarized as:

> **Start from a human-defined problem in AI use; use dialogue to discover rather than presuppose the required rules and organizational elements; treat those elements as replaceable construction materials; construct a purpose-appropriate AI-facing structure; observe its behavior; reconstruct it when necessary; and seek portability of the construction methodology rather than identity of architecture.**

This is a positioning hypothesis, not yet a confirmed novelty claim.

## 12. Revised Novelty Test

Future prior-art searches should no longer ask only:

> “Does another study use a similar method?”

They should ask:

> **“Did another study begin from substantially the same problem, adopt substantially the same research stance, and aim at substantially the same final research object?”**

A close match should satisfy most of the following:

1. The motivating problem concerns the organization or usability of an AI-use environment itself.
2. The human defines the governing problem/objective.
3. The final rule/structure is not fully predetermined.
4. Natural-language Human–AI dialogue is a primary construction mechanism rather than only an interface.
5. Rules, roles, boundaries, memory, control, or interaction pathways can be construction elements.
6. The resulting AI-facing structure is itself a primary research artifact.
7. Structures may be replaced or reorganized after observed consequences.
8. The method does not require one fixed architecture.
9. Portability is sought at the methodology/function level across heterogeneous AI systems.
10. Model weights/source-code access is not a prerequisite.

If an existing methodology satisfies most of these points, Paper 2 should be positioned as an extension, application, or comparison rather than as a distinct methodology.

If systematic searching finds no such close match, the paper may cautiously state that **within the reviewed literature, no work was identified that combines this originating stance, construction target, and portability objective in the same methodological framework**.

## 13. Next Search Target

The next search should concentrate specifically on:

- end-user construction of AI environments,
- natural-language construction of agent architectures,
- conversational configuration of multi-agent systems,
- adaptive Human–AI collaboration architectures,
- meta-design of AI systems,
- end-user AI orchestration,
- conversational programming of agent workflows,
- model-agnostic AI environment construction.

The purpose is no longer to collect broadly similar Human–AI dialogue research. It is to find—or fail to find—a study with the **same starting stance and the same structural endpoint**.
