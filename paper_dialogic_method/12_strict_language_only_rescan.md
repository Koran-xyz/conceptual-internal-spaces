# Strict Language-Only Rescan

**Status:** Targeted prior-work rescan for Paper 2

## Search Question

This pass applies a stricter criterion than ordinary “no-code” research.

The target is prior work in which:

1. the research target is an AI-facing environment or operational structure;
2. natural language itself participates in constituting that structure;
3. the structure is not merely translated into Python, executable code, formal policy, API calls, or workflow-engine representations;
4. human–AI dialogue can participate in construction or revision;
5. the final structure is not fully predetermined before dialogue;
6. the method is not intrinsically tied to one open-source model or one model implementation.

Systems that expose a natural-language UI while relying on code as the actual structural substrate are treated as adjacent work, not strict matches.

## Results

### 1. Natural Language as Architecture — autonomous-agent implementation

A recent implementation explicitly describes natural-language prompt files as architectural components. Thirteen Markdown prompt files and four natural-language axioms determine much of an agent's behavior.

However, the author also explicitly states that Python provides the execution skeleton and enforcement layer. The implementation depends on Python and an external request library. Under the present criterion, this is therefore an **adjacent but excluded** case.

Why it matters: it is strong evidence that the phrase “natural language as architecture” is already in active use. Paper 2 must therefore not claim novelty merely from treating prompts or Markdown rules as architectural material.

### 2. POMASA — prompt-defined multi-agent system

POMASA is particularly close at the declarative layer. It describes agents through structured natural-language “blueprints” containing role definitions, input specifications, tasks, output specifications, and quality standards. The paper explicitly contrasts this with writing substantial behavioral code and emphasizes that domain experts can modify agent behavior through text.

This is a **close comparator**, because natural language defines roles and behavioral structure rather than merely serving as a one-shot interface.

However, from the accessible description, POMASA is still presented as an implemented multi-agent system architecture. The natural-language blueprints define agent behavior within a surrounding system rather than establishing that the complete operational environment exists solely as language without software/runtime scaffolding.

Therefore it should not yet be classified as a strict match. It requires full-paper inspection before final exclusion or inclusion.

### 3. Natural Language Architecture (NLA) templates

NLA explicitly uses structured natural language to define systems, OS-level structures, layers, flows, and feedback loops, and describes itself as tool-agnostic and model-agnostic.

This is conceptually very close to the “language-first architecture” direction.

But NLA explicitly describes these natural-language architectures as designs that may later be implemented in code, no-code, or hybrid stacks. Natural language is primarily the architecture/design medium rather than necessarily the complete operational substrate.

Classification: **close conceptual comparator, but not a strict operational match**.

### 4. Intent Architecture

Intent Architecture begins with natural language but explicitly argues that language must be converted into enforceable artifacts such as schemas, policy checks, tool parameters, and execution boundaries.

Classification: **excluded** under the strict criterion because the operational structure is produced through formal/executable artifacts rather than language remaining the structural medium.

### 5. Natural-language no-code AI workflow systems

Recent no-code AI workflow approaches allow users to specify component behavior conversationally, but at least some explicitly translate those instructions into machine-executable code-based instructions.

Classification: **excluded**. A no-code user experience is not equivalent to a language-only architecture.

### 6. LLM OS / intent-driven operating-system concepts

Recent LLM-OS concepts make conversation the universal interface and let an LLM dynamically orchestrate tools and capabilities. These are relevant to the broad goal of reorganizing the AI/computing environment around language.

However, their underlying architecture remains a software system composed of tools, files, APIs, SDKs, generated software, or other executable components.

Classification: **adjacent, but excluded from strict language-only comparison**.

### 7. Language-mediated Active Inference safety architecture

A 2025 paper proposes an AGI safety architecture in which beliefs and preferences are represented in natural language, with modular multi-agent structures and hierarchical safety constraints.

This is relevant because natural language is used for transparent system-level representations rather than merely as an interface.

However, the framework is grounded in Active Inference and a specific computational architecture. It is not presented as a model-independent, language-only dialogic method for constructing arbitrary AI-facing structures.

Classification: **adjacent theoretical comparator, not a strict match**.

### 8. EpisodeSim / natural-language control state

A September 2026 paper represents classic-AI control structures as natural-language state interpreted by LLM calls. It uses natural-language control state for roles, scripts, obligations, commitments, timing, and closure conditions.

This is highly relevant to the proposition that persistent structure can be represented in language.

But it is explicitly a hybrid architecture: natural-language state is embedded in an engineered simulation system with designated components such as a World Master.

Classification: **close structural comparator, but excluded from strict language-only criterion**.

## Important Finding

The strict filter changes the literature landscape substantially.

Many projects that appear at first to be “natural-language architectures” fall into one of four categories:

1. **Natural language as interface** → translated into executable actions/code.
2. **Natural language as configuration** → prompts/blueprints configure a software framework.
3. **Natural language as design specification** → language describes architecture later implemented elsewhere.
4. **Natural language as one structural representation inside a hybrid architecture** → language carries some state/rules while code provides the surrounding system.

The current research target is narrower:

> **Natural language is investigated as a directly operative structural medium for constructing and revising an AI-facing environment through dialogue, rather than merely as an interface, configuration layer, design document, or precursor to executable code.**

This distinction should become explicit in Paper 2.

## Caution

This rescan does **not** establish that no prior work satisfies all criteria. Search terminology is unstable: relevant work may use terms such as prompt architecture, declarative agents, language-mediated control, textual scaffolding, constitutions, manifests, context engineering, or conversational programming without using “natural-language architecture.”

The correct scholarly claim remains:

> Within the literature and systems reviewed so far, we identified several close approaches in which natural language specifies, configures, or represents AI-system structure, but we have not yet identified a clear prior framework matching the full combination of language-as-operative-structure, dialogic construction and revision, non-predetermined structural outcomes, and deliberate model/implementation portability without code or formal translation as the structural substrate.

## Revised Comparison Test

For each future candidate, record five layers separately:

- **User-facing medium:** What does the human type or manipulate?
- **Construction medium:** What actually defines the structure?
- **Execution substrate:** What makes the structure operational?
- **Research objective:** Is the goal rules, workflow, software, task output, or AI-environment structure?
- **Portability assumption:** Does the method require a particular model, framework, source-code access, or executable runtime?

This prevents “no-code UI” from being incorrectly treated as “language-only structure.”

## Next Priority

The strongest unresolved comparator from this pass is POMASA. The next audit should inspect its full architecture and implementation details to determine whether its natural-language blueprints are merely declarative configuration over a coded runtime or whether the authors make a stronger claim about language constituting the multi-agent structure itself.
