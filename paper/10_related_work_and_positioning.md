# 10. Related Work and Research Positioning

## 10.1 Instruction Following and Verifiable Constraints

A foundational capability relevant to this study is the ability of LLMs to follow instructions expressed in natural language. IFEval (Zhou et al., 2023) introduced a reproducible benchmark based on objectively verifiable instructions, addressing the difficulty of evaluating instruction following with subjective or model-based judgments alone. More recent work on hierarchical instruction following, IFHierBench (Mao & Chen, 2026), evaluates constraints at multiple structural scopes and reports that prompt-level accuracy decreases substantially as constraint depth increases.

These studies establish that instruction following and scoped constraint satisfaction are themselves nontrivial empirical problems. The present work therefore does not treat successful response to a natural-language rule as evidence of a novel internal mechanism. Instead, ordinary instruction following is retained as a primary alternative explanation. The additional question examined here is whether semantically comparable rule functions—including contextual separation, switching, persistence, and restoration—can be studied across heterogeneous AI environments using a common natural-language construction method.

## 10.2 Instruction Priority and Rule Hierarchies

Wallace et al. (2024) proposed the Instruction Hierarchy framework to distinguish instructions by privilege and study model behavior when instructions at different levels conflict. Their work also introduced a training approach intended to improve hierarchical instruction following and robustness to lower-privileged conflicting instructions.

This line of work is relevant because apparent rule behavior in the present study may be influenced by platform-level instruction priority rather than by the user-defined conceptual organization alone. The present study differs in experimental focus: it does not train a model to implement a privileged hierarchy and does not assume access to system-level controls. It studies rule structures declared through user-visible natural-language interaction and treats platform instruction hierarchy as a potential confounding variable in cross-platform comparisons.

## 10.3 Constitutional and Natural-Language Principle Approaches

Constitutional AI (Bai et al., 2022) uses a written set of principles as human-provided guidance within a training procedure involving model-generated critiques and revisions, supervised learning, and reinforcement learning from AI feedback. It therefore provides an important precedent for using human-readable principles as explicit inputs to AI behavioral alignment.

The present work differs in mechanism and experimental setting. It does not modify model weights, perform reinforcement learning, or claim that conversationally declared rules are equivalent to a trained constitution. Its question is whether natural-language rule specifications presented through ordinary interaction can produce comparable observable functions across distinct AI environments.

## 10.4 Communicative and Multi-Agent LLM Systems

Research on LLM-based agents has shown that natural-language communication can support roles, cooperation, memory, planning, and task decomposition. CAMEL (Li et al., 2023) introduced a role-playing communicative-agent framework using inception prompting and studied instruction-following cooperation in multi-agent settings. Generative Agents (Park et al., 2023) combined LLMs with a memory architecture involving stored experiences, reflection, retrieval, and planning in an interactive agent environment. ChatDev (Qian et al., 2023) organized specialized LLM-driven agents through structured multi-turn communication for software-development tasks.

These systems demonstrate that language can participate in organizing complex agent behavior, while also relying on explicit agent frameworks, memory mechanisms, workflows, or supporting software. The present study isolates a different question: how much rule-related functional structure can be declared and compared through natural language itself, and whether comparable functions can recur when the surrounding AI environment differs.

## 10.5 Constitutions and Norm Enforcement in Multi-Agent Systems

Recent work has extended rule-based alignment questions into multi-agent environments. Kumar et al. (2026) proposed Constitutional Evolution, a framework that automatically evolves interpretable behavioral constitutions in a simulated multi-agent environment and evaluates them using coordination and societal-stability outcomes. Ye and Steinhardt (2026) studied norm-enforcement mechanisms for language-model agents. They report that simple enforcement mechanisms can be exploited and investigate more robust mechanisms based on reliability estimation and escalating penalties for repeated violations.

This literature is relevant to the longer-term motivation of the present research: common rule-related functions may matter not only within one conversation but also when multiple AI systems participate in shared environments. However, the present paper does not test a complete multi-agent governance system or claim a solution to norm enforcement. Its contribution is positioned earlier in the chain: operationalizing and testing whether natural-language-defined rule functions can be compared across heterogeneous AI environments before stronger shared-rule architectures are proposed.

## 10.6 Position of the Present Work

The literature above shows that natural-language instructions, principles, roles, constitutions, and norms already play important roles in LLM research. The novelty claim of this paper is therefore **not** that natural language can influence AI behavior, nor that language can define roles or rules.

The present research instead combines three narrower concerns:

1. defining contextual rule structures through natural language without requiring platform-specific implementation;
2. evaluating observable rule-related functions separately from claims about hidden internal mechanisms; and
3. asking whether those functions show convergence, divergence, or identifiable scope conditions across heterogeneous AI environments.

CIS is used as an operational framework for this comparison rather than as a claim of a newly discovered neural structure. The Cross-Platform Functional Convergence Hypothesis is likewise intended to be falsifiable and bounded: evidence may identify classes of systems and conditions in which convergence occurs, as well as systems and conditions in which it fails.

## References for This Section

- Bai, Y., et al. (2022). *Constitutional AI: Harmlessness from AI Feedback*. arXiv:2212.08073.
- Li, G., Hammoud, H. A. A. K., Itani, H., Khizbullin, D., & Ghanem, B. (2023). *CAMEL: Communicative Agents for “Mind” Exploration of Large Language Model Society*. arXiv:2303.17760.
- Park, J. S., O'Brien, J. C., Cai, C. J., Morris, M. R., Liang, P., & Bernstein, M. S. (2023). *Generative Agents: Interactive Simulacra of Human Behavior*. arXiv:2304.03442.
- Qian, C., et al. (2023). *ChatDev: Communicative Agents for Software Development*. arXiv:2307.07924.
- Zhou, J., et al. (2023). *Instruction-Following Evaluation for Large Language Models*. arXiv:2311.07911.
- Wallace, E., Xiao, K., Leike, R., Weng, L., Heidecke, J., & Beutel, A. (2024). *The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions*. arXiv:2404.13208.
- Kumar, U., Saito, A., Niranjani, H., Yessou, R., & Tan, P. X. (2026). *Evolving Interpretable Constitutions for Multi-Agent Coordination*. arXiv:2602.00755.
- Mao, Y., & Chen, C. (2026). *IFHierBench: Hierarchical Instruction Following for Large Language Models*. arXiv:2607.27912.
- Ye, Y., & Steinhardt, J. (2026). *Norm Enforcement for AI Agents: Robustly Shaping Behavior in Multi-Agent Systems*. arXiv:2607.09766.

---

## Citation Audit Note — 2026-09-03

The cited works in this section were rechecked against their source records during the v0.2 review. Claims were narrowed where necessary so that the text describes what the cited work directly supports. In particular, this section does not use prior work to imply that CIS is an established mechanism or that cross-platform functional convergence has already been demonstrated by these studies.

## Revision Note

This section was added during the v0.2 review stage. Its purpose is to position the working hypothesis relative to instruction-following, constitutional alignment, multi-agent communication, and norm-enforcement research. Section numbering and final placement may be reorganized during a later structural revision.
