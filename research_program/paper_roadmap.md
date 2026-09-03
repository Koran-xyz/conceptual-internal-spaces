# Paper Roadmap for the Research Program

**Status:** Working roadmap  
**Researcher:** Minoru Shimizu  
**Purpose:** Convert the branches of the research genealogy into bounded paper candidates without treating unverified ideas as established results.

## Guiding Principle

The research program should not be forced into one oversized paper. Each branch should become a paper when it has a sufficiently clear research question, evidence boundary, and reproducible evaluation plan.

A paper may begin as a hypothesis-forming or conceptual working paper. Experimental claims should be added only when the required evidence exists.

---

## Paper 1 — Natural-Language Rule Construction, CIS, and Functional Convergence

**Current status:** Active Working Paper v0.2 / baseline frozen for further research.

**Working title:**
*Natural-Language Rule Construction Across LLM Environments: An Exploratory Study of Conceptual Internal Spaces and Cross-Platform Functional Convergence*

**Core question:**
Under what conditions can natural-language-constructed rules produce comparable rule-related functions across different LLM environments?

**Current evidence:**
- Recorded small manual pilot experiments within ChatGPT.
- Historical exploratory observations from other AI environments.
- Related-work review and reproducibility protocol.

**Evidence still needed:**
- Stronger scope-sensitive tests.
- Standardized cross-platform replication.
- Better control conditions.

**Priority:** 1 — already established as the first bounded paper.

---

## Paper 2 — Dialogic Construction Methodology

**Provisional title:**
*Dialogic Construction Methodology: Human–AI Co-Construction of Rules and Adaptive Structures Through Natural-Language Interaction*

**Core question:**
Can iterative human–AI dialogue be described as a reproducible methodology for constructing, evaluating, revising, replacing, and reusing rules and structures?

**Main contribution candidate:**
Formalize the process:

**Problem discovery → Dialogue → Proposal → Mutual evaluation → Adoption/revision → Construction → Observation → Further dialogue**

**Important distinction:**
This paper should describe a methodology rather than claim that one fixed architecture results from the method.

**Evidence needed later:**
- Historical construction cases organized as traceable case studies.
- Examples where proposals originated from the human, AI, or both.
- Examples of rejected/revised structures, not only successful constructions.
- Comparison with related human–AI co-design, interactive design, and agent-design literature.

**Can progress without immediate experiments:** Yes.

**Priority:** 2 — strongest next paper for conceptual development while experiments are temporarily difficult.

---

## Paper 3 — Safety Functions: From Agent Roles to Structural Layers

**Provisional title:**
*From Safety Agent to Safety Layer: Comparing Agent-Based and Structural Realizations of Persistent Rule Functions in LLM Environments*

**Core question:**
Which safety-related functions are better represented as autonomous agent roles, and which are better represented as persistent structural or environmental functions?

**Origin:**
Exploratory development in which Guardian-like safety functions evolved from an agent-style role toward a structural layer concept.

**Hypothesis candidate:**
Some persistent safety functions may become more stable or less dependent on agent personality when represented structurally, while structuralizing all roles may destroy useful agent independence and diversity.

**Evidence status:** Historical exploratory observation / design hypothesis.

**Evidence needed:**
- Operational definitions of stability, persistence, interference, and role independence.
- Agent vs layer matched comparison.
- Failure cases where structuralization reduces useful multi-agent behavior.

**Priority:** 4 — valuable but should wait for clearer experimental conditions.

---

## Paper 4 — Internal, External, and Hybrid Rule Realization

**Provisional title:**
*Where Should AI Rule Functions Live? Internal, External, and Hybrid Realizations of Natural-Language Coordination Structures*

**Core question:**
Which rule, memory, safety, and coordination functions require internal contextual construction, and which can be externalized without losing their intended function?

**Design conditions:**
- Internal realization.
- External board/store realization.
- Hybrid realization.

**Main conceptual contribution candidate:**
Platform independence need not require identical architecture. Comparable functions may be realized through different placements depending on platform constraints and task requirements.

**Evidence needed:**
- Matched tasks across the three placement conditions.
- Measures of functional success, interference, persistence, coordination cost, and reproducibility.
- Multiple AI environments.

**Can progress without immediate experiments:** Partly; taxonomy and protocol can be developed now.

**Priority:** 3 — directly extends Paper 1 and the functional-convergence idea.

---

## Paper 5 — Shared Workspace Coordination Across Heterogeneous AI Systems

**Provisional title:**
*From Agent Handoff to Shared Workspaces: Functional Coordination Across Heterogeneous AI Systems*

**Core question:**
Can multiple AI systems preserve distinct platform-specific behavior while coordinating through a common external dialogue or work space?

**Key distinction:**
The target is not literal migration of one identical agent between platforms. The target is reconstruction of useful roles/functions and coordination through shared context.

**Evidence status:** Historical exploratory observations and existing design work; controlled replication still required.

**Evidence needed:**
- Defined shared-work protocol.
- Multiple AI participants.
- Task completion and consistency measures.
- Role reconstruction tests.
- Comparison with sequential handoff.

**Priority:** 5 — important applied branch, but technically heavier.

---

## Paper 6 — Common Natural-Language Rules for Multi-AI Environments

**Provisional title:**
*Toward Common Natural-Language Rules for Heterogeneous AI Environments: A Research Agenda for Shared Behavioral Norms*

**Core question:**
Which understandable behavioral rules, if any, can be shared across heterogeneous AI systems while respecting platform-specific constraints and existing safety requirements?

**Role in the program:**
This is the long-term synthesis branch. It returns to the original practical safety problem and the analogy of shared "traffic rules" for environments containing multiple AI actors.

**Important limitation:**
The content of common rules is not assumed in advance, and universal applicability should not be claimed.

**Likely paper type initially:** Research agenda / position paper, later supported by results from Papers 1–5.

**Priority:** 6 — synthesis target rather than immediate empirical paper.

---

## Recommended Order

The current working order is:

**Paper 1 — CIS / Functional Convergence**  
→ **Paper 2 — Dialogic Construction Methodology**  
→ **Paper 4 — Internal / External / Hybrid**  
→ **Paper 3 — Agent vs Layer Safety Functions**  
→ **Paper 5 — Shared Workspace Coordination**  
→ **Paper 6 — Common AI Rules**

This order is not permanent. It should change if new evidence makes another branch more mature.

## Why Paper 2 Comes Next

Paper 2 can be developed while stronger experimental infrastructure is unavailable. Much of its first-stage work consists of reconstructing the research history, defining the methodology precisely, identifying decision points, separating observation from interpretation, and comparing the method with existing literature.

It also explains why Papers 1, 3, 4, 5, and 6 belong to one research program.

## Validation Queue

Experimental work is not abandoned. Tasks requiring stronger technical conditions remain queued, including:

- Nested scope / local rule shadowing / scope restoration.
- Independent repetitions in fresh conversations.
- Cross-platform standardized replication.
- Agent vs structural-layer comparison.
- Internal vs external vs hybrid comparison.
- Shared-workspace multi-AI trials.

Conceptual development, literature review, protocol design, and research documentation can continue while these tests wait.

## Publication Discipline

For every future paper:

1. Separate recorded evidence from historical observations.
2. Separate operational concepts from claims about hidden mechanisms.
3. Label hypotheses as hypotheses.
4. Preserve negative and failed results.
5. State scope conditions rather than claiming universality.
6. Publish reproducibility material whenever practical.
7. Revise the research genealogy when a result changes the direction of a branch.

The purpose of the roadmap is not to predetermine conclusions. It is to make each research question small enough that another researcher can understand, criticize, reproduce, or extend it.