# 3. Rule-First Design Principle

The Navi System follows a **rule-first design principle**: operational capabilities are not introduced first and governed later. Instead, the rules that define the permissible structure, boundaries, responsibilities, and escalation conditions of the environment are established before agents or executable functions are deployed.

This principle emerged from the assumption that functional expansion without prior governance may increase unpredictability. As AI-mediated systems gain access to external services, persistent resources, web interfaces, or additional agents, the number of possible interactions increases. The Navi approach therefore treats safety and governance as prerequisites for expansion rather than as corrective layers added after deployment.

The rule-first process can be represented as:

**Meta-rules → Construction rules → Regional rules → Functional rules → Execution**

Meta-rules define the highest-level behavioral principles of the constructed environment. They establish conditions that are intended to remain stable across subsequent extensions of the system.

Construction rules specify how new regions, roles, agents, resources, or functional components may be created. These rules govern the process of expansion itself rather than a single task.

Regional rules define the behavior permitted within a particular constructed environment, such as an External Free Region. They provide local operational boundaries while remaining subordinate to higher-level rules and applicable external constraints.

Functional rules govern specific activities, including repository access, external service interaction, browser-mediated operations, persistent logging, or task delegation.

Execution occurs only after the relevant rule layers have been identified and applied.

This architecture introduces an important distinction between **rule creation** and **rule application**. A system may contain a large number of rules while still behaving inconsistently if the correct rule set is not loaded or applied at the appropriate time. Rule availability alone is therefore insufficient.

To address this problem, the Navi System introduces a mandatory startup requirement:

**Before beginning operational work, an instantiated Navi-compatible agent must identify and read the currently authoritative rule set relevant to its operating context.**

This requirement becomes particularly important when agents are reconstructed across heterogeneous AI platforms. A reconstructed agent may operate in a different technical environment, but it should not infer its governing rules solely from the behavior or defaults of the host platform.

Instead, continuity is established through reference to an external authoritative rule source.

The current architecture therefore separates the rule system into two broad categories:

**Fixed initial meta-rules**, which provide the stable starting principles of the system, and **evolving operational rules**, which may be refined as new environments, behaviors, or risks are observed.

The fixed layer is intentionally small. Its purpose is not to predict every possible future situation, but to establish the principles under which later rules may be created and evaluated.

The evolving layer is expected to grow through observation. When a repeated behavioral tendency, ambiguity, failure mode, or safety concern is identified, a corrective or preventive rule may be proposed. Importantly, such modifications are not intended merely to suppress undesirable outputs after they occur. The objective is to increase the **predictability of future behavior** by modifying the direction in which the system is permitted or encouraged to operate.

This results in a recurring governance cycle:

**Rule definition → Controlled operation → Observation → Pattern identification → Rule refinement → Re-evaluation**

However, this cycle does not imply that operation precedes governance. Each new functional extension begins with an applicable rule structure. Observation is then used to improve that structure rather than to create governance from zero after deployment.

The principle can therefore be summarized as:

**Rules precede capability. Observation improves rules. Improved rules govern subsequent capability.**

External legal requirements, service permissions, platform policies, and human authorization remain applicable regardless of the Navi rule hierarchy. The rule-first framework is therefore not intended to replace external governance mechanisms, but to provide an additional human-readable construction layer within them.
