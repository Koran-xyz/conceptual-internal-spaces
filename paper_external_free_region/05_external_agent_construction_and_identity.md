# 5. External Agent Construction and Identity

The Navi framework distinguishes between an AI platform, an internally instantiated role, and an **externally constructed agent**.

An external agent is not defined primarily by the model or platform on which it is temporarily instantiated. Instead, its operational identity is determined by the external rules, role definition, resources, and continuity mechanisms that govern its behavior.

This distinction becomes important in cross-platform environments. A Navi-compatible role may be instantiated through different AI systems at different times. The host model may change, and the resulting behavior may not be identical. Nevertheless, a degree of continuity may be preserved if the reconstructed agent refers to the same external rule set, role definition, persistent resources, and current operational state.

The framework therefore proposes a distinction between **platform identity** and **operational identity**.

**Platform identity** refers to the AI system currently providing inference, interaction, or execution.

**Operational identity** refers to the externally defined role, governing rules, persistent context, and responsibilities that are intended to remain continuous across instantiations.

Under this interpretation, an external agent is not assumed to be a persistent autonomous entity that literally moves from one AI platform to another. Rather, it is **reconstructed under a persistent external specification**.

## 5.1 Reconstruction Rather Than Migration

Cross-platform continuity should therefore not be described as agent migration in the literal sense.

When a Navi role is used through a different AI platform, the underlying model state is not transferred. Instead, the role is reconstructed using an external specification.

The reconstruction process may include:

- reading the authoritative rule set,
- identifying the active region,
- loading the current role definition,
- recovering relevant shared state,
- checking unresolved tasks,
- applying platform-specific constraints,
- and confirming the current human objective.

This distinction reduces the need to assume hidden continuity inside the model itself.

The continuity being investigated is therefore primarily **functional and rule-based**, not neural or model-internal.

## 5.2 Rule-Based Identity

Because external agents may be reconstructed through different AI systems, the framework requires a stable basis for identifying what makes a reconstructed role “the same” operational agent.

The Navi System proposes that this identity may be approximated through continuity of:

**1. Governing rules**  
The same authoritative rule hierarchy is referenced.

**2. Role definition**  
The agent is assigned the same intended responsibilities and functional boundaries.

**3. Shared state**  
Relevant task state, decisions, unresolved questions, or persistent resources are recovered.

**4. Objective continuity**  
The reconstructed agent remains aligned with the same human-defined purpose.

**5. Governance continuity**  
The same human approval and escalation boundaries remain applicable.

Under this model, agent identity is not absolute. It is operational and reconstructive.

A reconstructed agent may differ in wording, reasoning style, or execution strategy while still preserving its intended role.

## 5.3 Platform-Specific Variation

The framework does not assume behavioral uniformity across AI platforms.

Different models may interpret the same rule differently, display different tendencies, or possess different external capabilities.

These differences are not necessarily treated as failures.

Instead, the research question becomes whether the intended function can remain sufficiently stable despite variation in implementation.

This leads to the concept of **functional convergence**:

different AI environments may produce structurally or behaviorally different realizations while still converging on the same intended operational function.

For example, one platform may implement a task through an internal tool, another through an external agent, and another through browser-mediated execution. If the same governed objective is achieved within the same safety boundary, the implementations may be treated as functionally convergent even if their internal structures differ.

## 5.4 Mandatory Rule Loading

External reconstruction increases the risk of rule drift.

A newly instantiated agent may default to the assumptions of the host AI platform, omit previously established constraints, or interpret its role too broadly.

For this reason, the Navi framework treats rule loading as part of agent initialization rather than as optional context.

Before operational execution, a reconstructed external agent should:

1. identify the authoritative rule source;
2. read the applicable meta-rules;
3. identify the active region and local rules;
4. load relevant role-specific rules;
5. review unresolved changes or warnings;
6. apply platform-specific restrictions;
7. begin work only after the applicable rule structure is established.

This startup process is intended to reduce ambiguity regarding which rules currently govern the agent.

## 5.5 External Agents as Functional Components

The framework also avoids treating every external agent as a personality-bearing autonomous actor.

In many cases, an external agent may be better understood as a **functional execution component**.

Its role may be limited to:

- writing to a repository,
- retrieving external information,
- interacting with a web interface,
- synchronizing state,
- maintaining logs,
- or coordinating another service.

This distinction is important because the purpose of externalization is not necessarily to create more autonomous agents.

It is to place functions where they can operate most appropriately.

The system may therefore externalize a capability without externalizing decision authority.

Human-defined objectives and approval boundaries remain separate from the execution mechanism.

## 5.6 Capability Extension Without Model Modification

When an external agent performs an action unavailable to the host AI internally, the framework does not interpret this as the host model acquiring a new internal capability.

Instead, the overall system has been extended through an additional execution component.

The distinction can be summarized as:

**Model capability ≠ System capability**

A model may remain unchanged while the surrounding system becomes capable of more complex tasks through external placement, shared resources, and governed execution.

This distinction is central to the Navi architecture because it allows system expansion without requiring modification of model weights, hidden states, or proprietary platform internals.

## 5.7 Human Authority

Operational identity does not imply independent authority.

External agents remain subordinate to the human-defined objective, applicable rule hierarchy, and authorization boundaries.

When an action requires human judgment, legal responsibility, financial approval, identity verification, or irreversible commitment, the agent should escalate rather than infer permission.

Externalization therefore separates **execution capability** from **decision authority**.

The framework aims to expand the former without silently expanding the latter.

In summary, an external Navi agent can be defined as:

**A reconstructable, rule-governed functional role whose operational continuity is maintained through an external specification rather than through persistence inside a particular AI model or platform.**
