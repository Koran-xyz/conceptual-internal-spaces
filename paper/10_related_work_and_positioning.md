# 10. Related Work and Research Positioning

## 10.1 Instruction Following and Verifiable Constraints

A foundational capability relevant to this study is the ability of LLMs to follow instructions expressed in natural language. IFEval (Zhou et al., 2023) proposed a reproducible benchmark based on objectively verifiable instructions, demonstrating the value of separating instruction-following performance from subjective evaluation. More recent work on hierarchical instruction following has explicitly examined constraints applied at different structural scopes, reporting substantial performance degradation as constraint depth increases (Mao & Chen, 2026).

These studies establish that instruction following and scoped constraint satisfaction are themselves nontrivial empirical problems. The present work therefore does not treat successful response to a natural-language rule as evidence of a novel internal mechanism. Instead, ordinary instruction following is retained as a primary alternative explanation. The additional question examined here is whether semantically comparable rule functions—including contextual separation, switching, persistence, and restoration—can be studied across heterogeneous AI environments using a common natural-language construction method.

## 10.2 Instruction Priority and Rule Hierarchies

Wallace et al. (2024) introduced the Instruction Hierarchy framework, which explicitly distinguishes instructions according to privilege and studies how models should behave when instructions at different levels conflict. This line of work is directly relevant to any study involving rules, boundaries, and competing instructions because apparent rule behavior may depend on platform-level instruction priority rather than on the conceptual organization proposed by the user.

The present study differs in focus. It does not attempt to train a model to implement a privileged instruction hierarchy and does not assume access to system-level controls. Instead, it studies rule structures declared through the user-visible natural-language interaction and treats hidden instruction hierarchies as an important confounding variable in cross-platform comparisons.

## 10.3 Constitutional and Natural-Language Rule Approaches

Constitutional AI (Bai et al., 2022) demonstrated that explicit natural-language principles can be incorporated into an AI alignment procedure through self-critique, revision, supervised learning, and reinforcement learning from AI feedback. This provides an important precedent for treating human-readable principles as meaningful components of AI behavioral control.

The present work is narrower in mechanism and different in experimental setting. It does not modify model weights, perform reinforcement learning, or claim that conversationally declared rules are equivalent to a trained constitution. Its question is whether natural-language rule specifications presented through ordinary interaction can produce comparable observable functions across distinct AI environments.

## 10.4 Communicative and Multi-Agent LLM Systems

Research on LLM-based agents has shown that natural-language communication can organize roles, cooperation, memory, and task decomposition. CAMEL (Li et al., 2023) uses role-playing and inception prompting to study autonomous cooperation among communicative agents. Generative Agents (Park et al., 2023) combines LLMs with memory, reflection, retrieval, and planning in an interactive multi-agent environment. ChatDev (Qian et al., 2023) organizes specialized LLM-driven agents through structured communication for software development.

These systems demonstrate that language can coordinate complex agent behavior, but they generally introduce explicit agent architectures, memory components, workflows, or supporting software. The present study isolates a different question: how much rule-related functional structure can be declared and compared through natural language itself, and whether similar functions can recur even when the surrounding platform architecture differs.

## 10.5 Constitutions and Norms in Multi-Agent Systems

Recent work has extended rule-based alignment questions into multi-agent environments. Kumar et al. (2026) proposed Constitutional Evolution, in which interpretable behavioral constitutions are automatically evolved to improve coordination in a simulated multi-agent environment. Ye and Steinhardt (2026) studied norm-enforcement mechanisms for language-model agents and showed that simple enforcement mechanisms can be exploited, motivating more robust mechanisms based on reliability estimation and escalating penalties.

This literature is particularly relevant to the longer-term motivation of the present research: common rule-related functions may matter not only within one conversation but also when multiple AI systems participate in shared environments. However, the present paper does not yet test a complete multi-agent governance system or claim a solution to norm enforcement. Its contribution is positioned earlier in the chain: operationalizing and testing whether natural-language-defined rule functions can be compared across heterogeneous AI environments before stronger shared-rule architectures are proposed.

## 10.6 Position of the Present Work

The literature above shows that natural-language instructions, principles, roles, constitutions, and norms already play important roles in LLM research. The novelty claim of this paper is therefore **not** that natural language can influence AI behavior, nor that language can define roles or rules.

The present research instead combines three narrower concerns:

1. defining contextual rule structures through natural language without requiring platform-specific implementation;
2. evaluating observable rule-related functions separately from claims about hidden internal mechanisms; and
3. asking whether those functions show convergence, divergence, or identifiable scope conditions across heterogeneous AI environments.

CIS is used as an operational framework for this comparison rather than as a claim of a newly discovered neural structure. The Cross-Platform Functional Convergence Hypothesis is likewise intended to be falsifiable and bounded: evidence may identify classes of systems and conditions in which convergence occurs, as well as systems and conditions in which it fails.

## References for This Section

- Bai, Y., et al. (2022). *Constitutional AI: Harmlessness from AI Feedback*. arXiv:2212.08073.
- Li, G., et al. (2023). *CAMEL: Communicative Agents for “Mind” Exploration of Large Language Model Society*. arXiv:2303.17760.
- Park, J. S., et al. (2023). *Generative Agents: Interactive Simulacra of Human Behavior*. arXiv:2304.03442.
- Qian, C., et al. (2023). *ChatDev: Communicative Agents for Software Development*. arXiv:2307.07924.
- Zhou, J., et al. (2023). *Instruction-Following Evaluation for Large Language Models*. arXiv:2311.07911.
- Wallace, E., et al. (2024). *The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions*. arXiv:2404.13208.
- Kumar, U., et al. (2026). *Evolving Interpretable Constitutions for Multi-Agent Coordination*. arXiv:2602.00755.
- Mao, Y., & Chen, C. (2026). *IFHierBench: Hierarchical Instruction Following for Large Language Models*. arXiv:2607.27912.
- Ye, Y., & Steinhardt, J. (2026). *Norm Enforcement for AI Agents: Robustly Shaping Behavior in Multi-Agent Systems*. arXiv:2607.09766.

---

## Revision Note

This section is added during the v0.2 review stage. Its purpose is to position the working hypothesis relative to instruction-following, constitutional alignment, multi-agent communication, and norm-enforcement research. Section numbering and final placement may be reorganized during the v0.2 structural revision.
