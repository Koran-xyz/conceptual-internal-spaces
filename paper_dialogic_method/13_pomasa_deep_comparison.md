# POMASA Deep Comparison: Is Natural Language the Operative Structure?

**Status:** Prior-art comparison note for Paper 2

## Question

POMASA is a particularly close comparator because it explicitly replaces conventional code-defined agent behavior with natural-language blueprints. This note asks whether POMASA satisfies the stricter criterion currently being investigated for Dialogic Construction Methodology: **natural language itself as the operative structural medium, without Python or equivalent orchestration code being required to define the multi-agent structure.**

## Finding 1: POMASA is genuinely declarative and natural-language-defined

The peer-reviewed POMASA description states that traditional multi-agent development normally requires code for behavior, state, and communication, whereas POMASA defines each agent through a structured natural-language blueprint. The blueprint specifies role, expected inputs, task, outputs, and quality standards.

This means POMASA should not be dismissed merely as a graphical or conversational front end that secretly asks the user to write Python agent definitions.

## Finding 2: Its deployed systems can avoid Python orchestration code

Associated POMASA documentation reports a production research system containing hundreds of declarative agents and explicitly describes it as having no Python orchestration code, with agents represented as Markdown files.

Therefore, the earlier working assumption that POMASA could probably be excluded because a conventional Python orchestration layer sat underneath the blueprints is not supported. POMASA passes a substantially stricter language-defined-system test than many natural-language workflow systems.

## Finding 3: POMASA still requires an intelligent runtime

POMASA nevertheless does not claim that Markdown text executes independently. One of its required core patterns is **COR-02 Intelligent Runtime**. The runtime must be able to interpret the blueprints, instantiate agents, schedule resources, and execute tasks. Examples given by POMASA include agent-capable runtimes such as Claude Code, Cursor, and Cline.

This distinction is important:

- POMASA does not require Python orchestration code to define its agent architecture.
- But it does require a capable runtime that interprets the natural-language architecture.

This is not necessarily a meaningful difference from Dialogic Construction Methodology, because any natural-language structure ultimately requires an AI system capable of interpreting language. The relevant comparison cannot therefore be reduced to whether *any* software exists underneath.

## Finding 4: POMASA's research object and design goal differ

POMASA is presented as a **pattern-oriented multi-agent system architecture** for building declarative multi-agent research systems. Its pattern catalogue prescribes architectural patterns covering agents, structure, behavior, and quality. Its practical goal is to make robust multi-agent research systems constructible and maintainable without conventional programming expertise.

Dialogic Construction Methodology is currently being framed more broadly and differently. Its proposed primary research object is not a predefined multi-agent architecture or pattern catalogue. It investigates a process in which:

1. a human identifies and defines a problem and objective;
2. the final rule or structure is not necessarily known in advance;
3. human and AI use natural-language dialogue to generate and criticize candidate solutions;
4. rules, roles, boundaries, layers, agents, external stores, or other elements may be selected as provisional building materials;
5. the human governs adoption;
6. the resulting structure is used and observed;
7. observed consequences are returned to dialogue;
8. the structure may then be revised, replaced, externalized, internalized, or otherwise reconstructed.

Accordingly, POMASA is a close comparator for **language-defined architecture**, but it does not by itself establish equivalence with a **dialogic structure-discovery methodology** whose structural form is intentionally left open.

## Finding 5: Fixed pattern language versus open-ended structural discovery

POMASA has a catalogue of required, recommended, and optional architectural patterns. A generator can collect requirements, select an appropriate combination of those patterns, and generate the corresponding system files.

This is powerful, but conceptually it begins with an established architectural vocabulary and asks which patterns should be instantiated.

The current Dialogic Construction Methodology hypothesis begins one level earlier: the human may know the problem and desired objective while not yet knowing whether the appropriate solution should be a rule, agent, layer, internal contextual structure, external board, shared store, hybrid arrangement, or another structure. Dialogue is intended to participate in discovering that structural response rather than only configuring a pre-existing pattern catalogue.

This distinction must be tested carefully in later literature review and empirical work; it should not yet be presented as a confirmed novelty claim.

## Revised Exclusion Criterion

The previous criterion, “exclude any system that uses code somewhere,” is too broad. All practical LLM systems ultimately run on software.

A more defensible distinction is:

### Exclude from the strictest comparison
Systems in which the user-facing natural language is translated into a separately authored executable architecture (for example Python orchestration, API workflow code, or another formal executable representation) that becomes the actual structural specification.

### Keep as close comparators
Systems in which natural-language artifacts remain the primary editable specification interpreted directly by an intelligent runtime.

Under this corrected criterion, **POMASA remains a close comparator and should not be excluded.**

## Current Differentiation Hypothesis

The strongest remaining distinction is therefore not simply “language instead of code.” It is potentially:

> **Natural-language-mediated, human-governed discovery and reconstruction of the AI-facing structure itself, where the final structural form is not predetermined and where observations from the deployed structure feed back into subsequent dialogic reconstruction.**

POMASA demonstrates that declarative, natural-language-defined multi-agent architecture without Python orchestration is already real prior art. This narrows the candidate contribution of Dialogic Construction Methodology and strengthens the need to focus on **open-ended structure discovery, reconstruction, and construction trajectory**, rather than claiming natural-language architecture itself as novel.

## Sources Reviewed

- Xiong (2026), *Innovative Artificial Intelligence-Assisted Systems for Social Science Research: Architecture Design and Applied Practice*, AI & Innovation, DOI 10.1002/aiv2.70003.
- POMASA public documentation and pattern catalogue descriptions.
- Tricontinental Institute documentation describing declarative multi-agent systems and production deployment using POMASA.

## Evidence Boundary

This note compares published/documented system descriptions. It does not establish that POMASA and Dialogic Construction Methodology are empirically different in all implementations. A future direct comparison should apply the same construction task to both approaches and record what aspects of structural discovery are constrained, predetermined, generated, revised, and retained as natural-language artifacts.
