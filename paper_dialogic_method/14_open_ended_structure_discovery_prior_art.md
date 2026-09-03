# Open-Ended Structure Discovery Prior-Art Search

Status: working literature note
Date: 2026-09-03

## Question

Do prior studies begin from a human problem or objective without a predetermined final architecture, use natural-language interaction, and allow the agent/system organization itself to emerge, be constructed, or be revised?

The comparison is not merely whether the same techniques appear. The key test is whether the research begins from the same stance and aims at the same endpoint.

## Screening dimensions

1. Initial problem / research stance
2. Primary endpoint
3. Is the final structure predetermined?
4. Is natural language the operative construction medium?
5. Is human–AI dialogue used to discover/revise the structure?
6. Does the approach depend on programmatic scaffolding or a fixed runtime architecture?
7. Can the resulting structure itself be replaced or reconstructed after observation?

## Closest studies found

### S-Agents: Self-Organizing Agents in Open-Ended Environments (2024)

The work explicitly criticizes fixed task-oriented workflows and studies agent-centric organizational structures in open-ended environments. Agents are not assigned specific roles in advance; instead, they coordinate and allocate tasks dynamically.

This is an important overlap because the resulting organization is not fully predefined.

However, the starting stance differs. The research asks how autonomous LLM agents can self-organize efficiently in open-ended tasks. It provides a designed agent graph, tree organization, hourglass architecture, and collaboration mechanism. Human–AI dialogue is not the method by which a human-defined problem is transformed into an AI-facing structure. The organization emerges among agents inside a pre-engineered system.

Classification: close on emergent organization, different on construction stance and human-dialogic method.

### Drop the Hierarchy and Roles: How Self-Organizing LLM Agents Outperform Designed Structures (2026)

This study tests coordination protocols from imposed hierarchy to emergent self-organization. Under minimal scaffolding, agents invent roles and shallow hierarchies without pre-assigned roles.

This is strong evidence that structure discovery itself is an active research topic.

However, the primary goal is to measure autonomous coordination and performance under different protocols. A human does not begin with a practical problem and iteratively co-construct the resulting system structure through natural-language dialogue. The structure is emergent agent behavior within experimentally supplied protocols.

Classification: very close on non-predetermined roles; different research direction.

### AgentRAN: Agentic AI Architecture for Autonomous Control of Open 6G Networks (2025)

AgentRAN begins with natural-language operator intents. Agents interpret the intents, negotiate strategies, decompose tasks, and instantiate a self-organizing hierarchy. An AI-RAN Factory can observe interactions and generate new agents.

This is a particularly close comparator because high-level human intent can lead to changing agent organization rather than a fixed workflow.

Differences remain substantial. The endpoint is autonomous control of a 6G/Open-RAN network; the system is a predefined engineering framework and automated synthesis pipeline. Natural language expresses network-control intents, while the architecture that interprets and realizes those intents is programmatically engineered. The method is not a general human–AI dialogic methodology for discovering what kind of AI-facing structure should exist.

Classification: closest technical analogue found in this pass, but different domain goal and fixed framework substrate.

### Agentic AI Factories: Constructing Intelligent Workflows for Data-Driven Decision Making (2026)

The Factory Interface is a bidirectional chatbot that gathers and refines user requirements and proposes dynamic iterative workflow designs. It asks clarifying questions about goals, constraints, data, and desired outcomes.

This overlaps strongly with incomplete specification plus dialogue-driven construction.

However, its target is a workflow for data-driven decision making and the methodology is explicitly low-code. The dialogue is a requirements/design interface around a workflow-building system rather than natural language itself serving as the complete operative structural medium.

Classification: close on human-dialogic requirements discovery, different on endpoint and implementation substrate.

### POMASA (2026)

POMASA remains a close comparator because agents are declaratively defined by natural-language blueprints and can be changed by editing text rather than traditional agent code.

Its principal difference for the current question is that the blueprint vocabulary and agent-pattern methodology provide a predefined way to declare agent organization. The human primarily specifies/configures agents through this declarative system; the research does not appear to center an open-ended human–AI dialogue in which the kind of structure itself is initially unknown and is discovered, observed, replaced, and reconstructed.

Classification: close on language-defined structure, different on open-ended dialogic discovery.

## Important result

The prior-art search shows that several individual pieces already exist:

- structures can emerge without predefined roles;
- natural-language intent can drive dynamic agent organization;
- dialogue can refine incomplete workflow requirements;
- natural-language blueprints can declaratively define agents;
- systems can observe interactions and generate new agents.

Therefore none of these elements alone should be claimed as novel.

## Remaining candidate research stance

The narrower candidate distinction is the combination of the following starting stance and endpoint:

**Human-defined practical problem and objective → open-ended natural-language dialogue → candidate rules/roles/boundaries/components → human-governed evaluation and adoption → AI-facing structural configuration → use/observation → dialogic replacement or reconstruction of the structure itself.**

In this framing, neither the agent organization nor a workflow pattern is necessarily the starting assumption. Rules, agents, layers, memory stores, internal placement, external placement, or hybrid arrangements can be selected as replaceable construction techniques.

The primary endpoint is not task completion, policy translation, workflow generation, autonomous self-organization, or a domain artifact. It is the construction and reconstruction of an AI-facing structure appropriate to the human-defined purpose.

## Cautious conclusion

This search did not identify an exact prior framework with the same full starting stance, construction process, and endpoint. However, several nearby studies cover substantial parts of it. No uniqueness claim is justified yet.

The strongest next test is to search specifically for systems where a human and an LLM jointly decide *what architectural primitives should exist*—not merely their values, roles, or workflow instances—and where those primitives can be replaced after observing the deployed system.

## Sources reviewed

- Chen et al., S-Agents: Self-Organizing Agents in Open-Ended Environments, ICLR Workshop 2024.
- Dochkina, Drop the Hierarchy and Roles: How Self-Organizing LLM Agents Outperform Designed Structures, 2026 preprint.
- Elkael et al., AgentRAN: An Agentic AI Architecture for Autonomous Control of Open 6G Networks, 2025 preprint.
- Agentic AI Factories: Constructing Intelligent Workflows for Data-Driven Decision Making, Springer, 2026.
- Xiong, Innovative Artificial Intelligence-Assisted Systems for Social Science Research: Architecture Design and Applied Practice (POMASA), AI & Innovation, 2026.
